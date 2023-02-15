#### Meta information
23-02-04, 14:27
Status: #idea
Tags: [[MathematicalFormalismOfValueFunctioniteration]]





# MathematicalFormalismOfPolicyIteration

- Once we have obtained convergence of the value function, after value function iteration following the policy that we have,
- The goal becomes to find a new better policy using our found knowledge of the state value function.
- Here we follow the policy improvement theorem.
___
Reminder of the policy improvement theorem, from the mathematical formalism of optimality in RL:
$$
Q_\pi(s, \pi^`(s)) \ge V_\pi(s)\;\; \text{for all}\; s
$$
stating that if we construct a new policy and obtain a state action value function greater than the state value function of the old policy for all states, then the new policy is better than the old. (Note the new policy is constructed from the value function of the old policy.)
___
Given state value function estimates $V(s)$ after a sufficent number of sweeps, we can construct the new policy $\pi^`$ such that:
$$
r(f[s,\pi^`], \pi^`(s), s) + V(f[s, \pi^`(s)]) \ge V(s),
$$
Where the LHS follows from the state action bellman equation for the new policy:
$$
Q_\pi(s,a) = r(f[s, a], \;a,\;s) + V_\pi(f[s, a])
$$
___
The simpliest policy satisfying this is the greedy policy:
$$
\pi^`(s) = \arg\max_a \{r(f[s,a], a, s) + V_K(f[s, a])\}
$$
This is the action that maximises the LHS of the above inequality.
___
- If multiple action possess the same value, we can pick either. If the current action has maximum value we keep it, else we pick a new maximum at random if there are multiple maximums of the same value.
- From here we follow the policy optimisation rules, the new policy improves the value,
- The new improve values allow us to find a new better policy and so on and so forth, until we converge to optimality.
___



# References
