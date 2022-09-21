#### Meta information
22-09-20, 10:32
Status: #idea
Tags: [[HaikuNetworkDefiner]] [[HaikuLayer]] [[Haiku]]





# HaikuLayerDefiner
```python
# Tensor Policy network
def tn_policy_net(x):
	x = ActorCriticTensorNet(
			32, 3,
			is_actor=True,
			name='policy_network_1'
		)(x)
	# normilsation and sigmoid activation
	return x
```


The layer definer, takes the layer and calls bother the initialiser and the call fuctions of the haiku layer,  depending on an input (x).

```ad-important
The layer definer allows you to define the specifics of this layer, those are hyperparameters unique to how this layer is constructed and is different for each layer
```







# References
