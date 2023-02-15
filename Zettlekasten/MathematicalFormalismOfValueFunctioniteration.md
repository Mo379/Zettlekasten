#### Meta information
23-02-04, 11:34
Status: #idea
Tags: [[MathematicalFormalismOfOptimalityInRL]]


# MathematicalFormalismOfPolicyEvaluation

 - We need an efficent approach forevaluating the current policy, 
 - We can do that by estimating the state and/or state-action values to help us guide our policy updates.
 - we could calculate values iteratively from the start but that is inefficent,
 - and due to environemnt complexity, using the bellman equations for a backwards pass to calculate the values isnt possible, (for toy problems we knew the terminal state and which other states lead to this, this is not the same for complex envs)
 - so we settle for an iterative approach that utilises the bellman equations.
___
We need to estimate the state value function of the policy, so we start with a random one $V_0(s)$ and uptate it iteratively unti we reach $V_\pi(s)$ , we iterate until states occuring at $t=T$ where the values for those states is zero.

We update the values of all states according to:

$$
V_{k+1}(s) = 
r(f[s, \pi(s)], \pi(s), s) +
V_k(f[s, \pi(s)])
$$
$V_0,\;V_1,\;V_2 \ldots$  can be proven to converge to $V_\pi$ in a finite number of steps. This process can be understood as later states, accurately propagating their values back through time.

The maximum number of vaue function updates ($V_0,\;V_1,\;V_2 \ldots$) is the largest end time for a given initial state. (This is for problems where the trajetory ends at some finite time)
___

![[Pasted image 20230204142703.png]]


# References
