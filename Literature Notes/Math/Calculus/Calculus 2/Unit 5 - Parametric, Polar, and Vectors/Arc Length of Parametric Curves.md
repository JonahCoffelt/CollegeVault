#math #parametric
If we want to find the [[Arc Length]] of a parametric equation, we use a similar formula to the standard arc length equation: $$\boxed{\int_a^b\sqrt{x'(t)^2+y'(t)^2)}dt}$$
To derive this, we use similar steps as the arc length equation. First, construct a triangle with dx and dy. 
![[Pasted image 20230813144034.png]]
Now, to get the length of the line, simply use the Pythagorean theorem: 
$$\sqrt{dx^2+dy^2}$$
However, since we are in terms of $t$, we can express $dx$ as $dx=\frac{dx}{dt}dt=x'(t)dt$. Same applies to $dy$, giving us: $$\sqrt{(x'(t)dt)^2+(y'(t)dt)^2}=\sqrt{dt^2(x'(t)^2+y'(t)^2)}=\sqrt{x'(t)^2+y'(t)^2)}dt$$
Then, so sum all of the triangle hypotenuses on the line segment, simply integrate: $$\int_a^b\sqrt{x'(t)^2+y'(t)^2)}dt$$
# Example
Find the length of the curve defined by $x(t)=cos(t)$ and $y(t)=sin(t)$ from $t=0$ to $t=\frac\pi2$.

To do this, first find the derivative of $x(t)$ and $y(t)$: $$x'(t)=-sin(t)$$
$$y'(t)=cos(t)$$
Now, simply plug into the formula for parametric arc length: $$\int_0^\frac{\pi}2\sqrt{(sin^2t+cos^2t)}dt=\int_0^\frac{\pi}2dt=t\bigg|_0^\frac\pi2=\boxed{\frac\pi2}$$