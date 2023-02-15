#### Meta information
23-02-06, 11:02
Status: #idea
Tags: [[BootstrapingMonteCarloMethods]] [[MathematicalFormalismOfLearningThroughExperince]]





# FunctionApproximationMethods

- When calculating values independantly using Q learning methods, such as MC methods and boostrapped MC methods,
- We utilise high memory to save those tables,
- We get no generalisation, since similar states should be treaded with similar action, this trick is not used in tabular methods
___
- So instead we can utilise function approximations, instead of tabe based methods,
- Instead we prameterise the value function, with weights $\psi$, and weite the value function as $Q_\psi(s,a)$,
- We assume the gradient of $Q_\psi(s,a)$, is differentiable WRT ($\psi$), this is essential for efficent optimisation.
- $$
\nabla_\psi Q_\psi(s,a)
$$
- Examples of easily differentiable functions include polynomial expansions and nural networks...obviously.
___
- We can train the paramaters of those functions to estimate the the function Q,
- We need a loss function:$$
L(\psi| s,a) = \frac{1}{2}(Q_\psi(s,a) - Q_\pi(s,a))^2
$$
___
- We need to prioritise how we will be optimising the errors given by the loss function for each state action value pair, we do this using; $$
P(s,a) \ge 0 
$$
___
- We do this so we can focus on relevant states, if we simply sum the values of the losses then that focuses on irrelevant future states more than relevant states, 
- we can prioritise according to a greedy policy:$$
P(s, \pi(s)) \propto P(s_A) + P(s_B)
$$
___
- therefore we get full loss function for all states actions paris as: $$
§L(\psi) = \sum_{s,a}P(s,a)L(\psi|s,a)
$$
![[Pasted image 20230206112747.png]]




# References
