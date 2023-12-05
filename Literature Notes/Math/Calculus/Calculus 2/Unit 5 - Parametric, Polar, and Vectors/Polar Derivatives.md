#math #polar #derivative 
Taking a polar derivative is very similar to taking a parametric derivative, as both have x and y expressed in the terms of some third variable: $$\frac{dy}{dx}=\frac{\frac{dy}{d\theta}}{\frac{dx}{d\theta}}$$

Let's say we have the following polar equation: $$r=sin(2\theta)$$
We could just say that the derivative of $r$ in terms of $\theta$ is $r'(\theta)=2cos(2\theta)$. However, to get $\frac{dy}{dx}$ we have to dig a little deeper. 

First, we should define functions for $x$ and $y$ in terms of $\theta$ using the rules of [[Polar Coordinates]]: $$y=sin(2\theta)sin(\theta)$$
$$x=sin(2\theta)cos(\theta)$$
Now we can use the [[Product Rule]] to take the derivative of both of these in terms of $\theta$: $$y'(\theta)=2cos(2\theta)sin(\theta)+sin(2\theta)cos(\theta)$$
$$x'(\theta)=2cos(2\theta)cos(\theta)-sin(2\theta)sin(\theta)$$
Thus: $$\frac{dy}{dx}=\frac{2cos(2\theta)sin(\theta)+sin(2\theta)cos(\theta)}{2cos(2\theta)cos(\theta)-sin(2\theta)sin(\theta)}$$