#### Meta information
22-09-20, 09:27
Status: #idea
Tags: [[Jax]] [[JaxNetworks]]





# JaxInit

```python
import jax
raw_network = [layer1,layer2,layer3]
init_fn, apply_fn = \
	combinator(raw_network)
```

```python
params = init_fn(key, example_input)
apply = apply_fn(params, key, batch)
```


```ad-note
In jax you need to initialise your parameters manually, this is done using some sort of a combinator function, that takes a set of functional [[JaxLayers]] and outpouts two function an initialisation and apply function, those funcitons utilise sub functions form each layers to determine the pytree structure of the parameters and randomly initialise them.
```










# References
