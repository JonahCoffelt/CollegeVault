#math #derivative #inverse 
# General Inverse Function Rule
$$f(x)$$
$$g(x)=f^{-1}(x)$$
$$g(f(x))=x$$
# Apply Derivative
Differentiate each side of the equation above: $$\frac{d}{dx}[g(f(x))]=\frac{d}{dx}[x]$$
Apply the [[Chain Rule]] as follows: $$g'(f(x))\cdot f'(x)=1$$
$$\boxed{f'(x)=\frac{1}{g'(f(x))}}$$
or$$\boxed{f'(x)=\frac{1}{f^{-1'}(f(x))}}$$
## Example
Given the following function:
$$f(x)=e^x$$ We can define $g(x)$ to be it's inverse:
$$g(x)=f^{-1}(x)=ln(x)$$ And define $f'(x)$ and $g'(x)$
$$f'(x)=e^x$$
$$g'(x)=\frac1x$$
Then, we can verify using the equation found in the previous section

$$f'(x)=\frac{1}{g'(f(x))}$$
$$e^x=\frac{1}{\frac1{e^x}}=e^x$$