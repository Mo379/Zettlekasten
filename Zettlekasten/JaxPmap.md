#### Meta information
22-09-19, 08:45
Status: #idea
Tags: [[JaxVmap]] [[Jax]]  [[parallisation]]





# JaxPmap
```python
import jax
def foo(x):
	return x**2 
pmap_foo = jax.pmap(foo)(jnp.arange(8))[0**2,1**2,2**2,3**2,4**2,5**2,6**2,7**2]
```
This is a function transformation that allows you to parallise your compuration across many devices, this simply adds another dimension for the number of devices you have.

```ad-important
[[JaxVmap]] vectorises using primitive functions on the same device, pmap replication the function on each device and runs them in parallel.
```






# References
