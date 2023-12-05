#math #derivative 
Some relationships cannot be represented by an explicit function. For example, the function $x^2+y^2=1$ :
```desmos-graph
left=-2.5;right=2.5;
bottom=-1.75;top=1.75;
---
x^2+y^2=1
```
Thus for us to find the derivative of this relationship, we must use implicit differentiation. In reality, this is just an application of the [[Chain Rule]]

To do this, we apply derivative operators to each side of this function: $$\frac{d}{dx}[x^2+y^2]=\frac{d}{dx}[1]$$
$$\rightarrow \frac{d}{dx}[x^2]+\frac{d}{dx}[y^2]=0$$
$$\rightarrow 2x+\frac{d(y^2)}{dy}\cdot\frac{dy}{dx}=0$$
That last step is where the chain rule comes in. Because we cannot differentiate $y^2$ with respect to $x$, we use the chain rule, first, differentiating the given function, $y^2$, with respect to $y$, then differentiating $y$ with respect to $x$. To make it a bit more clear how exactly we are using the chain rule, we can write the term like this: $\frac{d}{dx}[(y(x))^2]$. In this we can clearly see our two functions, $y(x)$ and $y^2$ , and their relation to x. If we do this, we get the following: $$2x+2y\cdot\frac{dy}{dx}=0$$Now, we have our derivative in the function, we just have to solve for $\frac{dy}{dx}$: $$2y\cdot\frac{dy}{dx}=-2x$$
$$\rightarrow \frac{dy}{dx}=-\frac{x}{y}$$
Using this, we can find the slope of the relationship at any point. For example, to find the slope of the tangent line at the point $(\frac{\sqrt{2}}{2}, \frac{\sqrt{2}}{2})$, we simply plug in our $x$ and $y$ values: $$\frac{dy}{dx}=-\frac{\frac{\sqrt{2}}{2}}{\frac{\sqrt{2}}{2}}=-1$$
And if we plot this to the graph:
```desmos-graph
left=-2.5;right=2.5;
bottom=-1.75;top=1.75;
---
x^2+y^2=1
-x+\sqrt2
(\sqrt2/2, \sqrt2/2)|black
```
We see that we have the tangent line. 