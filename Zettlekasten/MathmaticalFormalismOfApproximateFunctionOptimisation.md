#### Meta information
23-02-06, 11:29
Status: #idea
Tags: [[MathematicalFormalismOfFunctionApproximationMethods]]





# MathmaticalFormalismOfApproximateFunctionOptimisation

- We can optimise the Loss function of value action approximation functions and optimise it using gradient decent
$$
\nabla_\psi L(\psi) = - \sum_{s,a}P(s,a)[Q_\pi(s,a) - Q_\psi(s,a)]\nabla_\psi Q_\psi(s,a)
$$
- We can update that using:
$$
\psi_{n+1} = \psi_n + \alpha_n \nabla_\psi L(\psi)|_{\psi=\psi_n}
$$
___
- The issue with this is that we have too many (s,a) pair and P(s,a) is too difficult to calculate, 
- so to solve this, instead of using simple gradient decent we use stochastic gradient decent,
- where we sample a subset of the trajectory and optimise it, instead of optimising a full trajectory at once, this si similar to batching in supervised learning,
- given one greedy trajectory we get a set of $(s_t,a_t)$ and along with it we get a return.
$$
 R_t = \sum_{t^`= t+1}^T r_t^`
$$

- and so we get the gradient fo the loss function:
$$
\nabla_\psi L(\psi) \approx \frac{1}{T-1}\sum_{t=0}^T[R_t-Q_\psi(s_t,a_t)]\nabla_\psi Q_\psi(s_t, a_t)
$$
___
This gives information about value of actions taken by the current policy, so we need to reintroduce exploration to obtain the value of alternative actions not takinen by the current policy. 

# References
