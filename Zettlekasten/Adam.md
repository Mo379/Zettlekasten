#### Meta information
22-09-21, 18:36
Status: #idea
Tags: [[Optimisers]]





# Adam


Adam is an optimisation algorithm that combines momentum Gradient Decent and RMSprop.

```ad-note
Initialise $V_{dw} =0$ , $S_{dw}=0$ , $V_{db}=0$ , $S_{db}=0$


On iteration t:
	$$\text{compute dw,db using current minibatch}$$
	$$V_{dw} = B1*Vdw + (1-B1)dw <- momentum$$
	$$V_{db} = B1*Vdb + (1-B1)db <- momentum$$
	$$S_{dw} = B2*Vdw + (1-B2)dw^2 <- RMSprop$$
	$$S_{db} = B2*Vdw + (1-B2)db^2 <- RMSprop$$
	$$V_{dw}^{corrected} = Vdw/(1-B1^t)$$
	$$V_{db}^{corrected} = Vdb/(1-B1^t)$$
	$$S_{dw}^{corrected} = Sdw/(1-B2^t)$$
	$$S_{db}^{corrected} = Sdb/(1-B2^t)$$
	$$W = W - alpha \frac{Vdw_corrected}{\sqrt{Sdw_corrected + \epsilon}}$$
	$$b = b - alpha \frac{Vdb_corrected}{\sqrt{Sdb_corrected + \epsilon}}$$
	
```


# References
