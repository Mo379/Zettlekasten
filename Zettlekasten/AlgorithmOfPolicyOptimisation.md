#### Meta information
23-02-04, 15:05
Status: #idea
Tags: [[MathematicalFormalismOfPolicyIteration]] [[MathematicalFormalismOfValueFunctioniteration]] [[AStateValueUpdateSweep]]





# AlgorithmOfPolicyOptimisation

- We initialise the policy $\pi$ and value function V.
- Choose a sweep order for this evaluation.
	- Perform a sweep over the state space, calculating the value using 
	- $$
V_{k+1}(s) = 
r(f[s, \pi(s)], \pi(s), s) +
V_k(f[s, \pi(s)])
$$
	- Repeat until the value function remains the same after a sweep
- Construct the greedy policy following: 
- $$
\pi^`(s) = \arg\max_a \{r(f[s,a], a, s) + V_K(f[s, a])\}
$$
- If $\pi^` = \pi$, terminate. ELse, repreat steps 2 and 3 with $\pi = \pi^`$, beginning evaluation from the final values of the previous evaluation.





# References
