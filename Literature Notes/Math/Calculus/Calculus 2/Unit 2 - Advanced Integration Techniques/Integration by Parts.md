#math #integral 
We know by the [[Product Rule]] that: $$\frac{d}{dx}[f(x)g(x)]=f'(x)g(x)+f(x)g'(x)$$
If we integrate both sides, then we will get: $$\int\frac{d}{dx}[f(x)g(x)]dx=\int f'(x)g(x)+f(x)g'(x)dx$$
$$f(x)g(x)=\int f'(x)g(x)dx+\int f(x)g'(x)dx$$
With this, we get the equation for integration by parts: $$\int f(x)g'(x)dx=f(x)g(x)-\int f'(x)g(x)dx$$
This helps us to solve integrals with two functions in them

# Example
Lets use integration by parts to solve the following integral: $$\int xcos(x)dx$$
We can identify our two functions and their derivatives: $$f(x)=x$$
$$f'(x)=1$$
$$g'(x)=cos(x)$$
$$g(x)=sin(x)$$
Now, we can just plug into the integration by parts equation: $$\int xcos(x)dx=xsin(x)-\int sin(x)dx=\boxed{xsin(x)+cos(x)+C}$$