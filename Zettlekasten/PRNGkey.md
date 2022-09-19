#### Meta information
22-09-18, 21:22
Status: #idea
Tags: [[Jax]] [[jax-syntax]]





# PRNGkey

```python
import jax
seed = 0
key = jax.random.PRNGKey(seed)
```

The psudo random number generator function allows you to create a key that can be used to generate information deterministically, therefore, allows you to easily reporduce your code however you like.



# References
