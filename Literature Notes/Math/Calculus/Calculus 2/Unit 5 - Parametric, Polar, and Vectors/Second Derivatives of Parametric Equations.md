#math #derivative 
We know from [[Derivatives of Parametric Equations]] that in a parametric equation: $$\frac{dy}{dx}=\frac{\frac{dy}{dt}}{\frac{dx}{dt}}$$
If we extend this, then we can get the following equation for the second derivative:  $$\frac{d^2y}{dx^2}=\frac{\frac{d}{dt}[\frac{dy}{dx}]}{\frac{dx}{dt}}$$
# Example
Find the second derivative of the following parametric equation: $$y(t)=e^{3t}-1$$
$$x(t)=3e^{2t}$$
To start, take the first derivative: $$\frac{dy}{dx}=\frac{3e^{3t}}{6e^{2t}}=\frac12e^t$$
Now, use the equation above for the second derivative: $$\frac{d^2y}{dx^2}=\frac{\frac{d}{dt}[\frac12e^t]}{6e^{2t}}=\frac{e^t}{12e^{2t}}=\boxed{\frac{1}{12e^{t}}}$$
