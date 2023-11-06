#### Meta information
23-02-04, 18:58
Status: #idea
Tags: [[LearningValueThroughExperince]] [[MathematicalFormalismOfPolicyIteration]]





# MathematicalFormalismOfLearningThroughExperince

We no longer assume the agent has access to  a model of the environment, so the values of states cannot be used to make iterate the policy, so now, to iterate the policy we need direct access to the state-action value function, so we can construct a policy:
$$
\pi^`(s) = \arg\max_a Q_\pi (s,a)
$$
___
This only considers trajectories generated by the current policy, so we wont know anything about alternative actions,  so we need some form of exploration to allow the policy to find new actions, we introduce ($\epsilon$), a small probability called the exploration rate. so that the agent picks an action no under the current policy but a random one.
___
Given ($A(s)$) possible actions, then the probability of and action (a) given a state (s): 
$$
P_\epsilon (a|s) =

\begin{cases}
    1 - \epsilon + \frac{\epsilon}{A(s)},
    & a = \pi(s)
    
    \\

    \frac{\epsilon}{A(s)},
    & a \neq \pi(s)
\end{cases}
$$
where the distribution $P_\epsilon$, is reffered to as an epsilong greedy policy when $\pi$, is greedy WRT a value function.
___
It's key to note that we can only accurately calculate the value of the last exploratory step taken in a single trajectory, if we try doing that for the second to last step, then return we obtain for that state action will not be representative, beccause its future is not entirely generated by the policy. 

![[Pasted image 20230205150837.png]]

But it is very important to concider multiple exploratory steps,

![[Pasted image 20230205150851.png]]
___


# References