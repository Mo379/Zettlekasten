#### Meta information
23-02-02, 10:22
Status: #idea
Tags: [[MathematicalFormalismOfTheValue]]





# MathematicalFormalismOfTheBellmanEquations

- If we follow the iterative process of updating the policy by calcualting the state value and state-action value pair, then it would be a very inefficent process as we have to carry out an exploding number of calculations.
- We can improve this by realising that the values of the state and state-action value pairs are closely related by a chain,
- The value of the current state is simply the sum between the value of the next state (under the current policy and dynamics) and the reward obtained in the transition,
- The value of an action in the current state, is the sum between value of the following state (under the current policy and dynamics) and the reward obtained in the transition using this specific action (not picked by the policy).
 ___
The bellman equations encodes the above, and are formally written as follows, for the state value: 
$$
V_\pi(s) = r(f[s, \pi(s)], \;\pi(s),\;s) + V_\pi(f[s, \pi(s)])
$$
and for the state-action value:
$$
Q_\pi(s,a) = r(f[s, a], \;a,\;s) + V_\pi(f[s, a])
$$
```ad-important
- The subequent state is written as the actions of the policy or the randomly picked actions (f[s,pi] and f[s,a] respectively)
- the reward function asks the environment a very important question, think about it and the layering of that with respect to exploration.
```



# References
