#math #derivative #parametric
We are given the parametric equation: $$x=2sin(1+3t)$$
$$y=2t^3$$
And we want to find the derivative $\frac{dy}{dx}$ when $t=-\frac13$.

The most important thing to realize in this type of problem is the following: $$\frac{dy}{dx}=\frac{\frac{dy}{dt}}{\frac{dx}{dt}}$$
So lets differentiate the two parts of the parametric equation with respect to $t$: $$\frac{dy}{dt}=6t^2$$
$$\frac{dx}{dy}=6cos(1+3t)$$
Thus: $$\frac{\frac{dy}{dt}}{\frac{dx}{dt}}=\frac{6t^2}{6cos(1+3t)}=\frac{t^2}{cos(1+3t)}$$
Now, we plug in our t value: $$\frac{(-\frac13)^2}{cos(1+3(-\frac13))}=\frac{\frac19}{cos(0)}=\frac19$$
We can find the equation of the tangent line if we also know the coordinates:

| t          | x   | y             |
| ---------- | --- | ------------- |
| $-\frac13$ | 0   | $-\frac2{27}$ |

$$y+\frac2{27}=\frac19(x)$$
$$\boxed{y=\frac19x-\frac2{27}}$$