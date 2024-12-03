# Horde: A Scalable Real-time Architecture for Learning Knowledge from Unsupervised Sensorimotor Interaction
+ **Authors**: Richard Sutton, Joseph Modayil, Michael Delp, Thomas Degris, Patrick Pilarski, Adam White, Doina Precup
+ **Tags**: knowledge representation, robotics, reinforcement learning, off-policy, temporal difference learning, value function approximation
+ **Year**: 2011

## Table of contents
+ The Problem
+ Why Learn Value Functions
+ General Value Functions
+ The Horde Architecture

## The Problem
How to learn, represent, and use knowledge of the world in a general sense remains a key open problem in AI. There are high-level representation languages based on first-order predicate logic and Bayes networks that are very expressive, but in these languages knowledge is difficult to learn and computationally expensive to use.

There are also low-level languages such as differential equations and state-transition matrices that can be learned from data without supervision, but these are much less expressive. There remains rooms for exploring alternate formats for knowledge that are expressive yet learnable from unsupervised sensorimotor data.


Horde is an architecture that consists of a large number of independant reinforcement learning sub-agents, or demons. Each demon is responsible for answering a single predictive or goal-oriented question about the world, thereby contributing in a factored, modular way to the system's overall knowledge. The questions are in the form of a value function, but each demon has its own policy, reward function, termination function, and terminal-reward function unrelated to those of the base problem. In this approach, the knowledge is represented as a large number of approximate value functions learned in parallel, each with its own policy, pseudo-reward function, pseudo-termination function, and pseudo-terminal-reward function.

## Why Learn Value Functions

A distinctive, appealing feature of approximate value functions as a knowledge representation language is that they have an explicit semantics, a clear notion of truth grounded in sensorimotor interaction. A bit of knowledge expressed as an approximate value function is said to be true, or more precisely accurate, to the extent that its numerical values match those of the mathematically defined value function that it's approximating. 

A value function asks a question, what will the cumulative future reward be?. An approximate value function provides an answer to that question. The approximate value function is the knowledge, and its match to the value function, to the actual future reward, defines what it means for the knowledge to be accurate.

A problem may have both a reward function as known in the reinforcement learning framework, and also a terminal reward function z: S --> R, where z(s) is the terminal reward received if termination occurs upon arrival in state s. It's common to discount rewards by a factor of γ ∈ [0, 1] for each step of delay. One way to think about discounting is as a constant probability of termination, of 1 - γ, together with a terminal reward that is always zero.

More generally, we can consider there to be an arbitrary termination function, γ: S --> [0, 1], with 1 - γ(s) representing the probability of terminating upon arrival in state s, at which time a corresponding terminal reward z(s) would be registered. The overall return for the trajectory starting at time t, is then the sum of the per-step rewards received up until termination occurs, say at time T, plus the final terminal reward received in ST,

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/48232278-c1856580-e3b9-11e8-8894-07a68e44d087.png"/>
</p>

The conventional action-value function Q is then defined as the expected return for a trajectory starting from the given state and action and selecting actions according to policy π until termination according to γ (thus determining the time of termination, T),

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/48232441-47a1ac00-e3ba-11e8-96e3-6beb73fb17ab.png"/>
</p>

The value function is the exact numerical answer to the precise, grounded question 'What would the return be from each state-action pair if policy π were followed?', and the approximate value function offers an approximate numerical answer. In this precise sense the value function provides a semantics for the knowledge represented by the AI agent's approximate value function.

## General Value Functions

The action-value function Q is equally dependant on the reward and the terminal-reward functions, r and z. These functions could equally well have been considered inputs to the value function in the same way that π is. We might have defined a more general value function, which might be denoted,

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/48233054-7c166780-e3bc-11e8-9099-3eb54bb6410d.png"/>
</p>

that would use returns from eqn(1) defined with arbitrary functions r and z acting as pseudo-reward function and pseudo-terminal reward function. Suppose we are playing a game, for which the base terminal rewards are z = +1 for winning and z = -1 for losing (with per-step reward r = 0). In addition to this, we might pose an independent question about how many more moves the game will last. This could be posed as a general value function with pseudo-reward function r = 1 and pseudo-terminal-reward function z = 0.

The second step from value functions to general value functions (GVFs) is to convert the termination function γ to a pseudo form as well. Formally, we define a general value function, or GVFs, as a function q: S x A --> R with four auxiliary functional inputs π, γ, r, and z, defined over the same domains and ranges as specified earlier, but now taken to be arbitrary and with no necessary relationship to the base problem's reward, terminal-reward, and termination functions:

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/48294757-06c79700-e48f-11e8-9fe2-f3323aad3fe3.png"/>
</p>

where Gt is still defined by (1) but now with respect to the given functions. The four functions, π, γ, r, and z, are referred to collectively as the GVF's question functions; they define the question or semantics of the GVF.

## The Horde Architecture

The Horde architecture consists of an overall agent composed of many sub-agents, called demons. Each demon is an independent reinforcement learning agent responsible for learning on small piece of knowledge about the base agent's interaction with its environment. Each demon learns an approximation, q̂, to the GVF, q, that corresponds to the demon's setting of the four question functions, π, γ, r, and z.

To learn the weights of the approximate GVF, the authors used gradient-descent termporal-difference algorithms. These algorithms are unique in their ability to learn stably and efficiently with function approximation from off-policy experience. Off-policy experience means experience generated by a policy, called the behavior policy, that is different from that being learned about, called the target policy. To learn knowledge efficiently from unsupervised interaction one seems inherently to face such a situation because one wants to learn in parallel about many policies, the different target policies π of each GVF, but of course one can only be behaving according to one policy at a time.

If learning can be done off-policy from incomplete snippets of experience then it can be massively parallel and potentially much faster than on-policy learning. Specifically, GQ(λ) algorithm was used. This algorithm maintains for each GVF, a second set of weights ω ∈ ℝ in addition to θ and an eligibility-trace vector e ∈ ℝ. All three vectors are initialized to zero. Then, on each step, GQ(λ) computes two temporary quantities, Φ̅t ∈ ℝ and δt ∈ ℝ, 

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/48319768-b11ff580-e61a-11e8-9063-67e2b031d2df.png"/>
</p>

where b : S x A --> [0, 1] is the behavior policy and λ : S --> [0, 1] is an eligibility-trace function which determines the rate of decay of the eligibility traces as in the TD(λ) algorithm. The approximation that will be found asymptotically by the GQ(λ) algorithm depends on the feature vectors Φ, the behavior policy b, and the eligibility-trace function λ. These three are collectively referred to as the answer functions. 

We can think of the demons as being of two kinds. A demon with a given target policy, π, is called a prediction demon, whereas a demon whose target policy is the greedy policy with respect to its own approximate GVF (i.e., π = greedy(q̂)) is called a control demon. Control demons can learn and represent how to achieve goals, whereas the knowledge in prediction demons is better thought of as declarative facts. One way in which the demons are not completely independent is that a prediction demon can reference the target policy of a control demon.











































