#math 
We have already talked about the area between a curve and the x-axis, but we can also take the area between two curves.

Let's say we have two functions, $f(x)$ and $g(x)$, we can find the difference between the heights of the two functions at a point $x=a$ by simply subtracting: $$height(a)=f(a)-g(a)$$
Thus we can use this to integrate for the area between the curves, as we know the distance between them at any given point: $$\int(f(x)-g(x))dx$$
One way to think about this is just taking the integral of the top function, minus the bottom function. Let's take a look at an example.

# Example
We have two functions: $y=x^2-3$ and $y=x^4-4x^2+1$:
```desmos-graph
left=-2;right=2;
bottom=-3.25;top=1.25;
---
x^2-3
x^4-4x^2+1
(-1, -2)|label|black
(1, -2)|label|black
y<\left\{-1\le x\le1\right\}\left\{x^{2}-3<y<x^{4}-4x^{2}+1\right\}
```
Here, the points of intersection are easy to see, but if you ever need to find them, simply set the functions equal to each other. You would end up with $x=-2,-1,1,2$, and you would just use the two that you wanted to use. 

Now, to get the area, we simply integrate top minus bottom: $$\int_{-1}^{1}(x^4-4x^2+1)-(x^2-3)dx$$Now, all we have to do is evaluate this definite integral: $$\int_{-1}^{1}(x^4-5x^2+4)dx=\frac15x^5-\frac53x^3+4x\bigg|_{-1}^1$$
$$(\frac15-\frac53+4)-(\frac{-1}5+\frac53-4)=\boxed{5\frac1{15}}$$