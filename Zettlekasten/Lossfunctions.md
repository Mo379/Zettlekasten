#### Meta information
22-09-17, 22:08
Status: #idea
Tags: [[BackPropagation]]





# Lossfunctions
Loss functions are used to calculate how well the [[MachineLearning]] algorithm is performing for this current batch, they use a special and well crafted function in order to determine this scalar value, which is later used by the [[GradientDecent]] and [[Optimisers]] algorithms to obtain better parameters.

```ad-important
$$J(\theta) = \frac{1}{N} \sum_{i=1}^N l(h_{\theta}(x^i), \hat{y^i})$$

The loss function is a function that takes in the parameters of the network (theta), and spits out a value telling us how good those parameters are. 
```




# References
