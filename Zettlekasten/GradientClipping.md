#### Meta information
22-09-20, 17:03
Status: #idea
Tags: [[PPOAlgorithm]] [[RunningEstimate]] [[ExponentialMovingAverage]] [[MovingAverage]]





# GradientClipping
```ad-quote
So the first moment is mean, and the second moment is **uncentered variance** (meaning we don’t subtract the mean during variance calculation), intuitively, clipping the gradients by moving average of its standard deviation wrt zero make sense.
```






# References
https://stackoverflow.com/questions/65243290/how-to-get-the-second-moment-of-the-gradient