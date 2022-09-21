#### Meta information
22-09-20, 11:05
Status: #idea
Tags: [[HaikuRandom]] [[HaikuTransform]] [[HaikuPRNGSequence]]





# HaikuWithoutKey

```python
import haiku as hk
init, apply = \
	hk.without_apply_rng(
		hk.transform(NetworkDefiner)
	)
```

The haiku.without_apply_rng function, wraps the transform function, and removes the otherwise compulsory RNG argument, making network work without a psudo randomisation factor.






# References
