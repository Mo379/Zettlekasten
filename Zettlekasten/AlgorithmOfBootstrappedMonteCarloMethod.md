#### Meta information
23-02-05, 18:24
Status: #idea
Tags: [[BootstrapingMonteCarloMethods]]





# AlgorithmWaltkinsQLearning

- In this algorithm we alays assume that the current policy is greedy
$$
\pi(s^`) = \arg\max_a Q(s,a)
$$
- The updates are done online
- because of the above two, we can simplify the update, where Q is the Q table, and is not Q for the current policy, so we dont have to concider what the policy is currently taking: 
$$
Q = r + \max_a Q(s,a)
$$

- We only need to store Q and not $\pi$, since $\pi$ is defined directly be Q. 
- We need to limit exploration to focus on relevant states, we still have exploration but not too much.
___
- Initialise Q to zeros, or anything viable,
- Chose number of trajectories, $N_T$, index n=0
- for each trajectory
	- start at $s_0$ at $t=0$
	- choose $a_t$ for $s_t$ $\epsilon$- greedy
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
	- Observe ($r_{t+1}$) and ($s_{t+1}$)
	- Update the Q table with
	- $$
Q(s_t, a_t) = r_{t+1} + \max_a Q(s_{t+1},a)
$$
	- set $t=t+1$, end if state is terminal
- $n=n+1$, repeat the above loop until $n=N_T$ times
___
In this algorithm we cannot know if we converged, unlike mote carlo algorithms where we notice that the value do not change, this is not possible here.
___
If the state space is too large, then this algorithm is limited, we need a way to solve that problem.

# References
