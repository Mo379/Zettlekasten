#### Meta information
22-09-20, 10:23
Status: #idea
Tags: [[Haiku]] [[HaikuLayer]]





# HaikuGetParams

```python

def __call__(self, inputs):
	mps_params = hk.get_parameter(
		"mps",
		shape=(
			inputs.shape[0],
			inputs.shape[1],
			# defined in the init func
			self.output_dim_size,
			self.contraction_dim_size,
			self.contraction_dim_size
		),
		dtype=inputs.dtype,
		# appropriate initalised
		init=initializer
	)
```

The Haiku get parameters function, allows you to obtain random parameters of a specific shape, those parameters can be given a name, type, and can be initialised using a specific initialiser.




# References
