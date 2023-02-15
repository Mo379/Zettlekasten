#### Meta information
23-02-02, 11:31
Status: #idea
Tags: [[MathematicalFormalismOfTheBellmanEquations]]





# MathematicalFormalismOfOptimalityInRL

We can use the value functions to order policies, where a policy is greater than another; $\pi^` \ge \pi$, if it provides an equal or greater value for every state,
$$
V_{\pi^`}(s) \ge V_{\pi}(s)
$$
This is partial ordering, because in a subset of states each one could be a greater policy than the other, for that we use a different method.
___
Therefore by chaining, for at least one special policy, the above must be true for all other policies, this is defines as the optimal policy, formally written as: 
$$
\pi_* \ge \pi \;\;,\text{for all} \;\pi
$$
___
If there are multiple optimal states, then they still share the same optimal state and state-value function pairs:
$$
V_*(s) = \max_\pi V_\pi(s) \;\; \text{for all} \;\; s,
$$
$$
Q_*(s,a) = \max_\pi Q_\pi(s, a) \;\; \text{for all} \; s \; \text{and} \; a
$$
___
The chaining nature of the bellman equations have to be satisfied by the optimal policy too. We can write the optimal value functions as the chaining sum of reward and value for the optimal policy without referencing the policy it self, this is because the optimal action is the ouput of the optimal policy so we use a max function: 

$$
V_*(s) = \max_a \{ r(f[s,a], \;a,\;s) + V_*(f[s,a])\}
$$
$$
Q_*(s,a) = \max_a\{r(f[s, a], \;a,\;s) + V_*(f[s, a])\}
$$
these are the bellman optimality equations. and it has a unique solution any reward function r and environmenal dynamics f.
___
If we are given the values of some policy, we can use the bellman optimiality equations to check if that policy is the optimal one.
___
The value function is linked to the policy, if we improve the policy we improve the value function and thus imporve the returns and move closer to our goal.
___
We need the current policy value functions, then we simply choose a new policy in which the value of every state is equal or greater than the current one, we can do this by improving the policy to a new policy according to a state-action value function for the first policy.
$$
Q_\pi(s, \pi^`(s)) \ge V_\pi(s)\;\; \text{for all}\; s
$$
This is the policy improvement theorem.


# References
