#### Meta information
22-09-19, 08:33
Status: #idea
Tags: [[vectors]] [[parallisation]] 





# JaxVmap
```python
import jax
import jax.numpy as jnp
# foo deals with a single input
def foo(x: int): -> int
	return x**2 + 2
# parallise the first input and show it to me in the first output	
vfoo = jax.vmap(foo, 0, 0)(jnp.ndarray)
''' vectorised foo
vectorises foo
Args:
	x: jnp.ndarray
returns
	y: jnp.ndarray
'''


```

This is a vector mapping function, it allows you to take a function and compute its parallel output with respect to a defined input axis,

```ad-important
Instead of having to mess around with dimensions when creating a batch version of any function, we simply start by making a simple function that deals with a single input, and then we vmap that function to get our batch compatible version.
```




# References
