#### Meta information
22-12-16, 11:01
Status: #idea
Tags: [[Optimisers]]





# MonmentumOptimisation

```ad-note
Initialise $V_{dw} =0$ , $S_{dw}=0$ , $V_{db}=0$ , $S_{db}=0$


On iteration t:
	$$\text{compute dw,db using current minibatch}$$
	$$V_{dw} = B1*Vdw + (1-B1)dw <- momentum$$
	$$V_{db} = B1*Vdb + (1-B1)db <- momentum$$
	$$W = W - alpha V_{dw}$$
	$$b = b - alpha V_{db}$$
	
```

This smoothes out the oscillation on gradient decent.

Allows you to mantain the horizontal movement since the average momentum in that direction is greater than the vertical, the vertical momentum converges to zero.



# References
