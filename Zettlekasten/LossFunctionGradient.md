#### Meta information
22-09-18, 12:51
Status: #idea
Tags: [[Lossfunctions]] [[GradientDecent]] [[PartialDerivatives]]





# LossFunctionGradient
This is the  gradient of the loss function, with respect to the parameters of the [[NeuralNetworks]].

```ad-quote
This tells us how the small nudges (partial derivatives) on the parameters, change the value of the loss function.
```
```ad-info
If you compare two gradient values, then their ratios is the relative change that each of them has on the loss function, meaning thatif the ratio is 10, then the first value has 10x greater effect than the second value.
```

This works for every neuron in the deep neural network, and is  enabled by [[TheChainRule]].





# References
