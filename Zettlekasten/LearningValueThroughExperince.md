#### Meta information
23-02-04, 17:54
Status: #idea
Tags: [[TheStateRelevanceProblem]]





# LearningValueThroughExperince

- In biology we learn through experince, i.e we learn directly from the seuqnce of events in a trajectory.
- This approach has an additional advantage,
- Sampling the experince or episode has the advantage that the model does'nt need to know the inner working of the environment,
- this means that this approach is model free,
- While the previous approach (dynamic programming) in the algorithm of policy optimiation is a model based approach, because we know the inner dynamics of the environment as we iterate the value and policy,
___
- E.g of model free learning, is an animal that doesnt know about a model for gravity or friction and is still able to learn how to apply forces to balance,
- Even if a model is present in the form of a computer simulation, sampling experince is still advantageous as it will help us adress the relevancy of state, because this automatically prioritises states that matter.
___
To understand why this stated approach works concider the following definitions that we previously saw: 
$$
V_\pi (s) = R(\omega_t^T)|_{s_t =s,\;\pi,\;f}
$$
$$
Q_\pi(s, a) = R(\omega_t^T)|_{s_t =s,\; a_t=a,\;\pi,\;f}
$$
Here we see that if we want to obtain the value we simply need the power to interact with the environment, but we do not need to know how it behaves.
___
so for a trajectory: 
$$(s_0, a_0) \rightarrow (s_1, r_1, a_1) \rightarrow (s_2, r_2, a_2) \rightarrow \ldots \rightarrow (s_T, r_T)$$
we can calculate the value as:
$$
V_\pi(s_t) = \sum_{t^`=t+1}^T r_{t^`}
$$



# References
