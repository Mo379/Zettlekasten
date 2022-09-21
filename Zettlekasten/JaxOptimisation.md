#### Meta information
22-09-20, 14:25
Status: #idea
Tags: [[jax]] [[Optimisers]] [[JaxGrad]] [[TreeMap]] [[JaxUpdateFunction]] [[Lossfunctions]]





# JaxOptimisation
In jax to optimise a model, the parameters have to be updated accordingly, this is done throught the [[TreeMap]] function.

After calculating the gradient of the loss function with respect to the pytree parameters of the model, we can use those gradients along with the their moments (gradient moments), to cleverly update the parameters.

[[GradientDecent]], [[StochasticGradientDecent]], [[RMSPROP]], and [[Adam]] are the most popular [[Optimisers]].






# References
