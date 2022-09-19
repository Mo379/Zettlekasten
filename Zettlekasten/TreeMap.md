#### Meta information
22-09-18, 21:34
Status: #idea
Tags: [[Jax]] [[pytrees]]





# TreeMap
```python
import jax
import jax.numpy as jnp

arr = jnp.array([0,1,2,3])
types = jax.tree_map(lambda x: type(x), arr)
types -> jnp.array([int,int,int,int])	
```

The tree map, traverses the pytree given to it, down to its individual leaves and carries out the specified functions. 

```ad-info
This is used in [[Optimisers]], to manipulate individual parameters of our neural network.

```




# References
