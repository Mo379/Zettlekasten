#### Meta information
23-02-02, 09:49
Status: #idea
Tags: [[TheStateActionValueFunction]]



# InterpretingTheStateActionValueFunction

- How we interpret the state action value function is a key piece of understanding of RL.
- The policy reccomends a specific action in a state.
- If we consider a different action to that which the policy suggests, for one step and then follow the policy from there,
- this would be useful because we can estimate the effect of changing the policy in the current state.
- After the end of the episode, if we calculate that the value of the new action and find it better than the one suggested by the policy,
- then this is an indication that we could improve the policy by changing it so that it recommends the new action.
- Furthermore, because we changed the policy, the values of states and state-action pairs also change,
- this may cause further difference between the current policy actions and the objective most valuable action in each state.
- we can repeat this iterative procedure until we converge torwards the best policy.




# References
