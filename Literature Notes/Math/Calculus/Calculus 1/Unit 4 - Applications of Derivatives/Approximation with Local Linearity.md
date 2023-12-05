#math #tangent #derivative 
Assume we want to approximate the value of $\sqrt{4.36}$. We could say that is will be a little bit more than $\sqrt4$, so a little more than $2$. However, we could get a more accurate result if we were to approximate with local linearity. 

To do this, we should define a function $f$ as $f(x)=\sqrt x=x^{\frac12}$. As stated earlier, $f(4)=2$, and we want to find $f(4.36)$. So, lets take a look at our function:
```desmos-graph
left=0;right=6;
bottom=0;top=3;
---
\sqrt x
x=4.36|dashed|label
(4, 2)|black|label
```
Here, we are trying to find the y value of the function at 4.36.

Now lets imagine that we create a line tangent to the graph at x=4, and use that to approximate the value of $f(4.36)$

We can do this by taking the derivative of $f(x)$ at $x=4$ (we are using this point because it is easy to compute, and it is close to our desired point), then use [[Point Slope]] form to get the equation of the line, $L(x)$:
$$f'(x)=\frac{1}{2x^{\frac{1}{2}}}$$
$$f'(4)=\frac{1}{2(4)^{\frac12}}=\frac{1}{2(2)}=\frac14$$
$$L(x)-2=\frac14(x-4)$$
$$L(x)=\frac14x+1$$
```desmos-graph
left=0;right=6;
bottom=0;top=3;
---
\sqrt x
x=4.36|dashed|label
(1/4)x+1
```
Now we can see that our line, at $x=4.36$ is really close to the value of the actual function we are trying to find. Thus: $$f(4.36)\approx L(4.36)=\frac{4.36}{4}+1=2.09$$
Therefore: $$\boxed{\sqrt{4.36}\approx 2.09}$$
This also makes sense with our intuitive guess at the beginning, as our final answer is just a little larger than 2.

It is worth noting that this value is an over approximation. We can see this if we look at the graph, as the line is always above the real function. If the function we are approximating is concave down, then the approximation will always be too high, and if the function id concave up, the approximation will be too low.

To prove this point, the actual value of $\sqrt{4.36}$ is $2.088$, thus we were really close, but a couple hundredths too high.