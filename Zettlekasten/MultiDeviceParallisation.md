#### Meta information
22-09-21, 16:54
Status: #idea
Tags: [[parallisation]] [[JaxPmap]]





# JaxParallisation

```ad-important
This is a general checklist for multi device parallisation, however there is much fluid knowledge to be obtained to reach a master lever, where this kind of thinking comes without much thought.
```
1) Get the number of devices available to jax locally
2) Initialise the parameters of the network for a single device
3) Replicate the parameters for the number of devices in a list using [[TreeMap]].
4) Reshape the data for the number of devices, accounting for a non divisible number of samples with the number of devices.
5) Create the loss and forward functions for a single device
6) Create the update function, wrapped with [[JaxPmap]], and with the use of other functions to execture the parallel computation.






# References
