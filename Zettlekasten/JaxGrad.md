#### Meta information
22-09-18, 21:53
Status: #idea
Tags: [[Jax]] [[AutomaticDifferentiation]] [[Optimisers]] [[BackPropagation]]





# JaxGrad
```python
import jax
def foo(x):
	return x**2
grad_foo = jax.grad(foo)
val = grad_foo(2) -> 2x = 2*2 = 4
```

The gradient function allows you to automaticall differentiate a compatible funtion.




# References
