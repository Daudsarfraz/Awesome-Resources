# High-Dimensional Continuous Control Using Generalized Advantage Estimation

Authors: John Schulman, Philipp Moritz, Sergey Levine, Michael I. Jordan, Pieter Abeel

Year: 2017

Algorithm: GAE

(Note: The summary here omits deduction processes of each formula. For greater details, please refer to the original paper. A clear explanation of GAE can also be found in the blog post [here](https://danieltakeshi.github.io/2017/04/02/notes-on-the-generalized-advantage-estimation-paper/).)

- Problems
  - Two main challenges for policy gradient methods:
    - The large number of sample required
    - Difficulty in obtaining stable and steady improvement
  - High bias is more harmful than high variance - it can cause the algorithm to fail to converge, or  converge to a poor solution.

- Proposed solution
  - For the first challenge: Use value functions to reduce the variance of policy gradient estimates with an estimator of the advantage function.
  - For the second challenge: Use Trust Region Optimization (TRPO) Procedure for both the policy and the value function.

- GAE (Generalized Advantage Estimator)
  - What it is: A family of policy gradient estimators

  - Goal: Significantly reduce variance while maintaining a tolerable level of bias

  - (This algorithm reduces policy gradient's variance at the cost of introducing bias)

  - A general summary of policy gradient methods

    ![img](https://github.com/RPC2/DRL_paper_summary/blob/master/imgs/009_1.png)

  - Define gamma-just for an estimator

    ![img](https://github.com/RPC2/DRL_paper_summary/blob/master/imgs/009_2.png)

  - Producing an accurate estimator

    ![img](https://github.com/RPC2/DRL_paper_summary/blob/master/imgs/009_3.png)

    - 0 < lambda < 1, and thus adjusting the value of lambda is making a tradeoff between bias and variance

      ![img](https://github.com/RPC2/DRL_paper_summary/blob/master/imgs/009_4.png)

  - Using the generalized advantage estimator, the discounted policy gradient is thus:

    ![img](https://github.com/RPC2/DRL_paper_summary/blob/master/imgs/009_5.png)


- Value function estimation

  - Use TRPO for adjusting policy network

    ![img](https://github.com/RPC2/DRL_paper_summary/blob/master/imgs/009_5.png)

    (For details about TRPO, please refer to the summary [here](https://github.com/RPC2/DRL_paper_summary/blob/master/01%20Model-Free%20RL/008%20Trust%20Region%20Policy%20Optimization.md))

  

