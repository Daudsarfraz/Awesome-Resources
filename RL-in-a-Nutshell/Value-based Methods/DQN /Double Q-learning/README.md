# Deep Reinforcement Learning with Double Q-learning
+ **Authors**: Hado van Hasselt, Arthur Guez, David Silver.
+ **Tags**: Double DQN, Atari, Experience Replay.
+ **Year**: 2016

## Table of contents
+ The Problem
+ The Solution
+ Contributions

## The Problem

Q-learning is one of the most popular reinforcement learning algorithms, but it's
known to sometimes learn unrealistically high action values because it includes a 
maximization step over estimated action values, which tends to prefer overestimated 
to underestimated values.

In previous work, overestimations have been attributed to insufficienlty flexible 
function approximation and noise. This paper unifies these views and shows that 
overestimations can occur when the action values are inaccurate, irrespective of the
source of approximation error. Overoptimistic value estimates are not necessarily a
problem in and of themselves. If all values would be uniformly higher then the relative
action preferences are preserved and we'd not expect the resulting policy to be any 
worse.

Optimism in the face of uncertainty is a well-known exploration technique. If, however,
the overestimations are not uniform and not concentrated at states about which we wish
to learn more, then they might negetivly affect the quality of the resulting policy

DQN is used to test whether overestimations occur in practice and at scale. This setting
is the best-case scenario for Q-learning, because the deep neural network provides
flexible function approximation with the potential for low asymptotic approximation
error, and the determinism of the environments prevents the harmful effects of noise.
Even in this comparatively favourable setting, DQN sometimes substantially overestimates the
values of the actions.

## The solution

In the reinforcement learning settings, the agent's sole purpose is to learn estimates
for the optimal value of each action, defined as expected sum of future rewards when
taking that action and following the optimal policy thereafter. Under a given policy
, the true value of action *a* in state *s* is,

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/45774418-27bcfa00-bc4d-11e8-8dd7-35bcf5cb904f.png"/>
</p>

An optimal policy is easily derived from the optimal values by selecting the highest
valued action in each state. Estimates for the optimal action values can be learned
using Q-learning. We can use a parametrized value function Q(s, a; θ) instead of tabular one
to solve really large and interesting problems. The standard Q-learning update for the
parameteres after taking an action in current state and observing the immediate reward
and the resulting state is,

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/45774810-466fc080-bc4e-11e8-8600-83edb03c8c3c.png"/>
</p>

where α is a scalar step size and the target Yt is defined as,

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/46223338-63457b80-c353-11e8-8c77-6a6d8fb7148e.png"/>
</p>

Two important ingredients of the DQN algorithm  are the use of a target network, and
the use of experience replay. The target network, with parameters minused θ, is the
same as the onine network except that its parameters are copied every τ steps from the online
network, and kept fixed on all other steps. The target used by DQN is then,

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/46223436-aa337100-c353-11e8-9773-7d12c872227f.png"/>
</p>

For experience replay, observed transitions are stored for some time and sampled uniformly
from this memory bank to update  the network. For more details on the DQN, you can read the [summary](https://github.com/Neo-47/RL-in-a-Nutshell/tree/master/DQN%20/Human%20level%20control%20through%20deep%20RL) of the original paper.

The max operator in standard Q-learning and DQN, in (2) and (3), uses the same values
both to select and to evaluate an action. This makes it more likely to select overestimated
values, resulting in overoptimistic value estimates. To prevent this we can decouple
the selection from the evaluation and this is the main idea behind Double Q-learning.

The Double Q-learnig target can then be written as:
<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/46223521-e961c200-c353-11e8-8765-d2dfbf6a9cd9.png"/>
</p>

Notice that the selection of the action, in the argmax, is still due to the online 
weights θt. This means that, as in Q-learning, we are still estimating the value of
the greedy policy according to the current values, as defined by θt. However, we 
use the second set of weights minused θt to fairly evaluate the value of this policy.
This second set of weights can be updated symmetrically by switching the roles of θ and minused θ.

This version of Double DQN is perhaps the minimal possible change to DQN towards 
Double Q-learning. The goal is to get most of the benefit of Double Q-learning, while
keeping the rest of the DQN algorithm intact for a fair comparison, and with minimal
computational overhead.

## Contributions

The following figure shows that on several games the improvements from DQN to Double 
DQN are striking, in some cases bringing scores much closer to human, or even surpassing these.

<p align="center">
<img src ="https://user-images.githubusercontent.com/19307995/46909919-d7c70f80-cf3a-11e8-9ccc-4834a25e09e5.png"/>
</p>

This paper presented five contributions. First, it's  showen why Q-learning can be
overoptimistic in large-scale problems, even if these are deterministic, due to the
inherent estimation errors of learning. Second, by analyzing the value estimates on
Atari games it's clear that these overestimations are more common and severe in practice
than previously acknowledged. Thrid, it's shown that Double Q-learning can be used at
scale to successfully reduce this overoptimism, resulting in more stable and reliable
learning. Fourth, the authors proposed a specific implementation called Double DQN, that
uses the existing architecture and deep neural networks of the DQN algorithm without
requiring additional networks or parameters. Finally, the authors have shown that 
Double DQN finds better policies, obtaining new state-of-the-art results on the Atari 2600 domain.

For more details on the experiments and plots illustrating the contributions, head straight to the paper.








