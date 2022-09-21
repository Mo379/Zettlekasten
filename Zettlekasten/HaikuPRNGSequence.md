#### Meta information
22-09-20, 11:00
Status: #idea
Tags: [[Haiku]] [[HaikuRandom]]





# HaikuPRNGSequence
```python
import haiku
rng = hk.PRNGSequence(jax.random.PRNGKey(42))
key = next(rng)
key2 = next(rng)
```

The PRNGSequence allows you to generate many keys from a single seed key, this is done by creating an iterator.

```ad-important
This is used in haiku to make the creation of keys more efficent, resulting in cleaner and clearer code.
```




# References
