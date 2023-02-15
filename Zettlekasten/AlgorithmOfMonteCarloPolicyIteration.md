#### Meta information
23-02-05, 15:12
Status: #idea
Tags: [[MathematicalFormalismOfLearningThroughExperince]]





# AlgorithmOfMonteCarloPolicyIteration

- Now we implement an actual learning algorithm based on learning from experince, called Monte-Carlo policy iteration.
- producing experince and exploring alternative through randomness is an example of a monte-carlo method.
___
- This algorithm has two alternating steps, value iteration and policy iteration,
- We also define a number of trajectories to execute before a policy iteration can take place,
- this is because there are many trajectories that provide no information that will allow us to update the values, and so we trigger a false termination, having many trajecties run is a solution.
___
- once we run enough trajectories we use the following to make the new policy:
 $$
\pi^`(s) = \arg\max_a Q_\pi (s,a)
$$
- to get the greedy policy after value iteration, we store two value functions ($Q$) and ($Q^`$), 
- after a value iteration ($Q$) is replaced by the valuated values of  ($Q^`$).
- After policy iteration we repeat again with 
___

$$
\pi^`(s) = \arg\max_a Q_\pi (s,a) \;\; \text(eqn. 11)
$$
$$
P_\epsilon (a|s) =

\begin{cases}
    1 - \epsilon + \frac{\epsilon}{A(s)},
    & a = \pi(s)
    
    \\

    \frac{\epsilon}{A(s)},
    & a \neq \pi(s)
\end{cases}
\;\; \text(eqn. 12)
$$
![[Pasted image 20230205154834.png]]
# References
