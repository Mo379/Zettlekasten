#### Meta information
23-02-05, 18:26
Status: #idea
Tags: [[AlgorithmOfMonteCarloPolicyIteration]]





# BootstrapingMonteCarlo

- Montecarlo algorithm: looks at the relevant states but offers limited updating, (we cannot update multiple exploratory steps unless we use a replay buffer)
- Instead of using a replay buffer, we bootstrap the monte carlo method with the bellman equation for the state action value function under the current policy
- since this function only depends on (s,a,r, s+1), thus no dependence on future actions,
- it means we can do online learning, where we immeadietly make updates
___
- Take the current Q table
- sample (s,a,r,s+1)
- update using bellman's equations

![[Pasted image 20230206080824.png]]






# References
