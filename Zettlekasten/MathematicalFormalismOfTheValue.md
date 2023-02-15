#### Meta information
23-02-01, 19:53
Status: #idea
Tags: [[MathematicalFormalismOfRLBasics]]





# MathematicalFormalismOfTheValueFunction

- If you want the value function to tell you how good the current state or state action pair is.
- It must be related to how well the goal is achieved under the decisions made in the future under the current policy, and the changes they make in the environemnt.
- The Return is the concept we need: "we need to calculate the return that will result following that state or state-action pair, under the current policy and environment dynamics"
___
We define the return for a subset of the trajectory: 
$$
\omega_t^t = \{(s_{t^`}, a_{t^`}, r_{t^`})\}_{t^` = t}^{T}
$$
understand that the return for a subset, is the cumilative sum from some point until the end, not from some point until another point that is not the end.
___
we define the return for the sub trajectory as: 
$$
R(\omega_t^T) = \sum_{t^`=t+1}^T r_{t^`}
$$
Note: the reward at time is is not included because it is the reward for a step outside of our sub-trajectory.
___
We generalise the value function to yet ungenerated states, those states are generated according to a policy, hence we write:
$$
V_\pi (s) = R(\omega_t^T)|_{s_t =s,\;\pi,\;f}
$$
So we obtain the return according to the current state, policy and dynamics of the environment.
___
We can also define the value of an action in a particular state as: 
$$
Q_\pi(s, a) = R(\omega_t^T)|_{s_t =s,\; a_t=a,\;\pi,\;f}
$$
evaluated with the following known variables; state, action, policy and dynamics function. with the rest of the states and actions following the output of the policy and dynamics as indicated by the evaluation.

The two functions above are called the state value and state-action value functions respectively. 
___


# References
