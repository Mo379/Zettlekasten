#### Meta information
22-09-20, 10:03
Status: #idea
Tags: [[Haiku]]





# HaikuLayer

```python
import haiku as hk

class layer(hk.Module):
	def __init__(self, *args, **kwargs):
	'''
	Define the hyperparameters of the
	layer, this is unique and general
	 for each layer.
	'''	
		pass
	def __call__(self, inputs):
	''' 
	Define the behaviour of the network,
	both the parameters to be created
	and the dynamics of the layer
	'''
		pass
	def _helper_function(self):
	'''
	Defines intermediate functions that
	can help organise the code, this is to 
	be used in the call funciton
	'''
		pass
```

A haiku layer, is a class that inherits from hk.moduel, and  contains both an __init__() and a __call__() function, , see the docstrings above for what each of theose does



# References
