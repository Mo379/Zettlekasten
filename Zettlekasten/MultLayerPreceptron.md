#### Meta information
22-09-18, 07:47
Status: #idea
Tags: [[NeuralNetworks]]





# MultLayerPreceptron
The most basic type of neural network, where individual neuron like computational structures are connected in layers, to produce an output, along with the use of [[ActivationFunctions]], the neurons could represent highly complex non-linear distributions.

The MLP, is made of layers, with the first one names the [[InputLayer]],  the last one named [[OutputLayer]], and the intermidiate layers names [[HiddenLayers]]

```ad-quote
The first input cases specific activations to the next input and the next to the next and so on until the output layer 
```


```ad-note
Showing a very simple MLP, with two inputs, two outputs and two intermediate hidden layers.
![[MultLayerPreceptron 2022-09-18 10.37.25.excalidraw]]

Mathematically, 

$$
\text{output} = 
a(
	w_{11}^{l}i_{11}^{l-1} +
	w_{12}^{l}i_{12}^{l-1}...+
	w_{nm}^{l}i_{nm}^{l-1}
)
$$

Where (a) is the [[ActivationFunctions]], (w) is the weights matrix, for subscripts (neuron, weight) for layer (l), and (i) is the input from the previous layer for subscript (neuron, weight) 
```

# References
