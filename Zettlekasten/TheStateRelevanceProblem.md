#### Meta information
23-02-04, 16:14
Status: #idea
Tags: [[AlgorithmOfPolicyOptimisation]]





# TheStateRelevanceProblem
- Our policy optimisation so far treats each state equally,
- But the vast majority of states in the statespace are irrelevant for the solution,
- this can be inefficent,
___
- 1) because if we restric the number of possible staring positions, we will find that there are states which our system cannot access,
- this is because there is no set of actions that we can take to reach that particular state, we have diverged from it, 
- so calculating the value for it is irrelevant.

```ad-note
![[Pasted image 20230204162434.png]]
```
___
- 2) and because, In the above sketch we notice that the relevant states are substantially fewer than the possible states, 
- so for a given initial policy, only a small amount of the state space will be visited,
- so if we only evaluate/iterate the values of states around the green corridor in the above sketch, then we will update our policy such that,
- the actions stay the same, or change to somthing close to our goal, so the resulting trajectories will stay in the green corridor regardless,
- even though we only interated the policy with respect to those small number of relevant states.
- However, with complex problems, we may not know which states are relevant and which are not!
- So we want an approach that naturally favours relevant states from which it learns the values using value iteration before running policy iteration





# References
