#### Meta information
22-09-20, 10:04
Status: #idea
Tags: [[PRNGkey]] [[Haiku]] [[HaikuLayer]]





# HaikuRandom
Within haiku there is support for randomisation, this utilises the PRNGKey given to the initialisation and apply functions obtained from the [[HaikuTransform]] function as a global key, from which all other keys within the network are sequentialy [[KeySplit]] and and used to generate random factors.

```ad-note
If the newtwork doesnt use random behaviour, this can be disabled, by wrapping the transform function with another fucntion.
```






# References
