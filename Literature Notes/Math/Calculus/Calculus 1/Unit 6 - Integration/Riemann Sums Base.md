#math #riemann
Lets assume we have the following curve:
```desmos-graph
left=0;right=4;
bottom=0;top=5;
---
-(x-2)^2+4
```
And we would like to know the area underneath it on the interval $[a, b]$, how would we do that?

To start, we could approximate it using rectangles at subintervals. For our example, we could use 5 rectangles, each of width .5, and with a height that is equal to the $y$ value of the function on the right side of the rectangle. It would look something like this:
```desmos-graph
left=0;right=4;
bottom=0;top=5;
---
-(x-2)^2+4
y-(1.75-1)<\left\{0<x<.5\right\}|red
y-(3-1)<\left\{.5<x<1\right\}|blue
y-(3.75-1)<\left\{1<x<1.5\right\}|red
y-(4-1)<\left\{1.5<x<2\right\}|blue
y-(3.75-1)<\left\{2<x<2.5\right\}|red
y-(3-1)<\left\{2.5<x<3\right\}|blue
y-(1.75-1)<\left\{3<x<3.5\right\}|red
y-(0-1)<\left\{3.5<x<4\right\}|blue
```
(It is hard to see the last rectangle, because the $y$ value that its based on is 0, thus its height is 0)

If we were to sum up the area of all these rectangles, then we would have an approximation for the area under the curve: $$\sum^n_{i=1}f(x_i)\Delta x_i$$