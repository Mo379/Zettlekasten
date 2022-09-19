#### Meta information
22-09-18, 16:45
Status: #idea
Tags: [[Optimisers]]





# TaylorPolynomial
The taylor series is used to approximate non polynomial functions using polynomials, the idea is, for a specific region of this function, we will find a polynomial that approximates it.

```ad-warning
The polynomial outside of this range, deviates away from the function it is trying to approximate
```

```ad-note
![[TaylorSeries 2022-09-18 16.53.24.excalidraw]]

This idea of creating a polynomial to fit the function, based on it's derivatives is the basis for the taylor series expansion, and this can be further generalised.
```
```ad-note
There is a pattern that emerges, due to the us taking many derivatives, we come to notice that if we want to match the value of the targe function's derivative then we have to divide our  function nth derivative by the factorial of n
```
```ad-note
If we're approximating at a value other than zero then we adjust our taylor equation to make that point behave like zero, this is so that we can allow each coeffiecent to be controlled by a single derivative
```

```ad-important
The taylor series is defined as 
$$
T_n(x) = 
\sum_{k=0}^n \frac{f^k x_0}{k!}
(x-x_0)^k
$$

Where $f^k(x_0)$ is the kth derivative of f at $x_0$. To generalise, for a smooth function this simply sums to infinity, when you do that it's called a taylor series
```


# References
