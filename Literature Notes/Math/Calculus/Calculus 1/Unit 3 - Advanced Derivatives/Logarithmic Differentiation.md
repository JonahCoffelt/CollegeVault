#math #derivative 

# Derivative of $log_ax$ 
$$\frac{d}{dx}[log_ax]=\frac{1}{x\cdot ln(a)}$$
## Proof:
We know that $\frac{d}{dx}[ln(x)]=\frac{1}{x}$, but how do we do $log_ax$?
To start, we, can rewrite the function using change of base formula as the following: $$log_ax=\frac{log_cx}{log_ca}$$
Since we know the derivative of $lnx$ we can use $e$ in place of $c$ as our base so that we are working with natural logs: $$\frac{d}{dx}[log_ax]=\frac{d}{dx}[\frac{ln(x)}{ln(a)}]$$
We can break this down further, by taking out $lna$, since it is just a constant: $$\frac{d}{dx}[log_ax]=\frac{1}{ln(a)}\cdot\frac{d}{dx}[ln(x)]$$
Using $\frac{d}{dx}ln(x)=\frac{1}{x}$ ([[Derivatives with e]]) we get: $$\frac{d}{dx}[log_ax]=\frac{1}{x\cdot ln(a)}$$
