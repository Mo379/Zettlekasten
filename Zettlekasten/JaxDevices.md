#### Meta information
22-09-20, 09:25
Status: #idea
Tags: [[JaxPmap]]





# JaxDevices
```python
import jax
jax.devices()
```

This funciton indicates the names of devies available for jax to use, those accelerators are either cpus, gpus or tpu cores.

```ad-important
This is used with pmap to orchistrate parallel computations, allowing you to correctly braodcaset your dimensions.
```




# References
