#### Meta information
22-09-20, 10:03
Status: #idea
Tags: [[Haiku]] [[HaikuLayer]]





# HaikuNetworkDefiner
```python
# actor critic nature cnn model

def my_model(x):
	features = feature_extractor(x)
	#
	values = value_net(features)
	action_mean = policy_net(features)
	#
	actions, log_sd = \
		log_std(name='log_std')(action_mean)
	#
	return actions, values,
```

The network definer builds on top of the  [[HaikuLayerDefiner]], where it takes the haiku layer definer funciton (eature_extractor, value_net, policy_net), and builds a complete network





# References
