#### Meta information
23-02-06, 12:01
Status: #idea
Tags: 





# MathematicalFormalismTermporalDifferenceMethods

- we reintorduce exploration and bootstrapping into our approximate function methods,
- we know that
$$
Q_\pi(s,a) = r + Q_\pi(s^`,\pi(s^`))
$$
- This is only exact for the action value function of the policy and no for the approximate action value function, 
- But we assume that it is relatively accurate for the approximate  ON POLICY action value function;
$$
Q_\psi(s, \pi(s)) \approx Q_\pi(s, \pi(s))
$$
- so we can say: 
$$
Q_\pi(s,a) \approx r + Q_\psi(s^`, \pi(s^`))
$$
- The graidnet then becomes:
$$
\nabla_\psi L(\psi) \approx \frac{1}{T-1}\sum_{t=0}^T[Q_\psi(s^`, \pi(s^`)) + r -Q_\psi(s,a)]\nabla_\psi Q_\psi(s_t, a_t)
$$

- Note: the square brackets contain the temporal-difference error. 
- Using the above equation we can run an epsilon greedy policy.
- we can also learn online:
$$
\delta_\psi L(\psi) = - \delta(s,a,\psi)\nabla_\psi Q_\psi(s,a)
$$
- Q-learning:
$$
\delta_Q(s,a,\psi) = \max_{a^`} Q_\psi(s^`, a^`) + r - Q_\psi(s,a)
$$

# References
