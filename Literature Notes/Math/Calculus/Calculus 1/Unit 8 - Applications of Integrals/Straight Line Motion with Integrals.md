#math #motion

Let's say we have a function for velocity: $\vec v=5-t$: 
```desmos-graph
left=0; right=10;
bottom=-5; top=5;
---
5-x
```
We can see that at time $t=0$ the object is traveling at a velocity of $+5 \frac m s$. We can also see that at $t=5$ the object has no velocity and it changes direction. 

So Lets think about what the [[Displacement]] of the object in the first 5 seconds. To do this, we can find the area under the line. To do this, we can take the integral $\int_0^5\vec v(t)dt$, or we can recognize that it is a triangle, thus the area is: $$\frac125\cdot5=12.5m$$
But, what would be the displacement over the first 10 seconds?

In this scenario, the object actually goes back $12.5 m$, as its velocity becomes negative. Thus the positive and negative area will exactly cancel out, leaving a total displacement of $0m$. If you don't believe this, we can take the integral to prove it: $$\int_0^{10}(5-t)dt=5t-\frac12t^2\bigg|_0^{10}=(5(10)-\frac{(10)^2}{2})-(5(0)=\frac{0^2}{2})=0-0=\boxed{0m}$$
If you are still not convinced, let's think about how this differs from total [[distance traveled]]. Displacement references the change in position, and the objects position at $t=10$ is the same as its position at $t=0$. However, the total distance traveled will not be 0, as the object has moved. To get the distance traveled, we take the integral of the absolute value of the function, so that the positive and negative areas do not cancel out: 
$$speed=|\vec v(t)|$$
```desmos-graph
left=0; right=10;
bottom=-5; top=5;
---
\abs(5-x)
```
$$\int_0^{10}|5-t|dt=25m$$