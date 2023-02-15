#### Meta information
23-02-01, 15:08
Status: #idea
Tags: [[ConceptOfTimeInRL]] [[TheEpisode]] [[TheState]] [[TheActions]] [[TheRewards]] [[ThePolicy]] [[EnvironmentDeterminism]] [[TheReturn]]





# MathmaticalFormalismOfRLBasics

We formalise RL here.

The discrete time step is labelled as (t).
The state of the environment at time (t) is ($s_t$).
The action taken by the agent at time (t) is ($a_t$).
The reward recieved by the agent at time (t) is ($r_t$).
The episode ends at time (T).
___
The episode is defined as the whole of the following sequence: $$(s_0, a_0) \rightarrow (s_1, r_1, a_1) \rightarrow (s_2, r_2, a_2) \rightarrow \ldots \rightarrow (s_T, r_T)$$
Where the reward for any action in a particular state is give in the next time step not in the same time step.
___
The episode is generalised as $$\omega_0^T = \{(s_t, a_t, r_t)\}_{t=0}^T$$
where $w_0^T$ represents the set of tuples of state, action, and reward for each time step between and including (t=0) and (t=T). (note: the first reward and last action dont occur in reality and are a side effect of generalisation, they are Null values.)
___
The policy is defined as: 
$$
a_t = \pi(s_t)
$$where ($\pi$) is the policy.
___
The possible transitions given an action in a particular state can be given by the dynamics function (f), If the environment is deterministic, then transitions in the state of the environment can simply as the following:
$$
s_{t+1} = f(s_t, a_t)
$$
(f) is reffered to as the environment dynamics, note: if the environment is non-deterministic then we will obtain a set of probabilities for each state instead of the above single state.
___
The reward at each time step, must only depend on the tuples of time steps (aka: the events) around that time step in the trajectory.
$$
r_{t+1} = r(s_{t+1}, a_t, s_t)
$$
where punishments are negative values and rewards are positive.
___
Given some initial state ($s_0$), the functions ($\pi$), ($f$) and ($r$) completely determine the trajectory ($\omega_0^T$), the goal of reinforcemnet learning is to find a policy which maximizes the total reward or return from  any given initial state such that: 
$$
R(\omega_0^T) = \sum_{t=1}^{T}r_t
$$

# References
