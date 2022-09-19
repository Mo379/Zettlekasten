#### Meta information
22-09-18, 21:39
Status: #idea
Tags: [[PRNGkey]]





# KeySplit

```python
import jax
seed = 0
key = jax.random.PRNGKey(seed)
k1,k2,k3 = jax.random.split(key, num=3)
```

The split function in jax, splits the key into multiple keys specified by the num parameter, this allows us to generate new psudorandom information on the fly.

```ad-note
due to the deterministic nature of jax, this is needed because if otherwise, a number generator will only produce the same output.

Output variables is key for sampling and generating random variables, this is key for initialisation and other key machine learning concepts
```



# References
