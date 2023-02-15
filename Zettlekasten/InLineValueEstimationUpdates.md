#### Meta information
23-02-04, 12:15
Status: #idea
Tags: [[MathematicalFormalismOfValueFunctioniteration]]





# InLinePolicyUpdates

- When estimating the state value function of a policy using a computer,
-  we can implement the iterative approach using two array, one containing the current values and one filling in the values as we iterate,
- this be made efficent using inline updates, where a single array is used, and we update the values in that array as we iterate,
- a problem with this is that values which have already been iterated now, could be updated in the next steps, this depends on the order in which the values are updates for each state,
- But so long as this order includes every state at least once,
- the inline updates can still converge to the policy value function.

each time every state is updated once is called a sweep





# References
