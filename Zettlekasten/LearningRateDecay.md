#### Meta information
22-12-16, 12:41
Status: #idea
Tags:  [[Optimisers]] [[GradientDecent]]





# LearningRateDecay

- Your algorithm or network may not converge
-  If you slowly reduce alpha, your learning rate slows down as you approach the minima, and you have a better chance to converge.
```ad-note
1 epoch = 1 pass through all of the data.

$$ 
\alpha = \frac{1}{1 + \text{decay rate} \times \text{epoch num}} \times \alpha_0
$$

where you can initialise alpha_zero to be 0.9, and the decay rate to be 0.1.

$$ \alpha = 0.9^{epoch num} \times \alpha_0 \text{<-- Exponential} $$

There are other decays methods, e.g discrete decay
	
```





# References
