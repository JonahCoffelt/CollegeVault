#math #rule #derivative #composite 
# Chain Rule (Derivative of a Composite Function)
$$\boxed{\frac{d}{dx}[f(g(x))]=f'(g(x))\cdot g'(x)}$$
Take the derivative of the outside, and leave the inside as is, then multiply by the derivative of the inside.
## Example
$$h(x)=(sin(x))^2$$
The inside function is $sin(x)$, and the outside function $u^2$. First, take the derivative of the outside function with respect to the inner (treating $sin(x)$ as $x$ itself): $$\frac{d}{d(sin(x))}[(sin(x))^2]=2(sin(x))$$
Second, multiply this by the derivative of the inside function, which is: $\frac{d}{dx}[sin(x)]=cos(x)$ to get the final solution: $$2sin(x)\cdot cos(x)$$
## Example 2
Find the derivative of the following function: $$y=7^{x^2-x}$$
This can be broken into the inside ($u(x)$) and outside ($v(u)$) functions, and their derivatives: $$\mbox{outside: }v(u)=7^u \mbox{ derivative: }v'(u)=\frac{d}{du}[7^u]=ln(7)7^u$$
$$\mbox{indide: }v(x)=x^2-x \mbox{ derivative: }u'(x)=\frac{d}{dx}[x^2-x]=2x-1$$
Thus, using the chain rule, the solution is: $$v'(u(x))\cdot u'(x)=ln(7)7^{x^2-x}\cdot(2x-1)$$