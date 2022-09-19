22-09-17, 20:19

Status: #idea
Tags:  [[MachineLearning]]

# BackPropagation
Backpropagation is the method by which [[MachineLearning]] algorithms learn to change their parameters so they make better decisions in the future. Using the [[TheChainRule]], the error of the [[Lossfunctions]], could be traced back to every neuron in the model, and so by utilising [[GradientDecent]], the parameters defining each neuron are slightly changes, such that the error of the loss function decreases.

This process relies on [[Optimisers]], which are methods that calculate the best possible gradients.

```ad-note
![[BackPropagation 2022-09-18 13.42.57.excalidraw]]

Following this, we calculate each of the partial derivatives present within the chain rule to obtain the loss gradient of the loss funciton wrt any parameter.
```
# References
