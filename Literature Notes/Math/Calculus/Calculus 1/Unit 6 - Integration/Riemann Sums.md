#math 
# Rectangle Sum
To get an even more accurate approximation of the area, we can use a trap
![[Riemann Sums Base]]

In the above example, we can see that if we over estimate on the left, and underestimate on the left. This is important to consider, and something we get into more detail with soon. 

We could also take the sum from the left side, which would look like this:
```desmos-graph
left=0;right=4;
bottom=0;top=5;
---
-(x-2)^2+4
y-(0-1)<\left\{0<x<.5\right\}|blue
y-(1.75-1)<\left\{.5<x<1\right\}|red
y-(3-1)<\left\{1<x<1.5\right\}|blue
y-(3.75-1)<\left\{1.5<x<2\right\}|red
y-(4-1)<\left\{2<x<2.5\right\}|blue
y-(3.75-1)<\left\{2.5<x<3\right\}|red
y-(3-1)<\left\{3<x<3.5\right\}|blue
y-(1.75-1)<\left\{3.5<x<4\right\}|red
```

If we want to know if the sum will over or under approximate the actual area, we can use this table:

|           | Decreasing | Increasing |
| --------- | ---------- | ---------- |
| Right Sum  | Under      | Over       |
| Left Sum | Over       | Under      |

And finally, we could take the sum from the middle, which would look like this:
```desmos-graph
left=0;right=4;
bottom=0;top=5;
---
-(x-2)^2+4
y-(.938-1)<\left\{0<x<.5\right\}|blue
y-(2.438-1)<\left\{.5<x<1\right\}|red
y-(3.438-1)<\left\{1<x<1.5\right\}|blue
y-(3.938-1)<\left\{1.5<x<2\right\}|red
y-(3.938-1)<\left\{2<x<2.5\right\}|blue
y-(3.438-1)<\left\{2.5<x<3\right\}|red
y-(2.438-1)<\left\{3<x<3.5\right\}|blue
y-(.938-1)<\left\{3.5<x<4\right\}|red
```

# Trapezoidal Sum
For a more accurate approximation, we could use trapezoids instead of rectangles. As an example, let's take the function $f(x)=\sqrt{x-1}$:
```desmos-graph
left=.5;right=6.5;
bottom=0;top=2.5;
---
y=\sqrt{x-1}
```
Lets make 5 trapezoids of equal base as such:
```desmos-graph
left=.5;right=6.5;
bottom=0;top=2.5;
---
y=\sqrt{x-1}
\operatorname{polygon}\left(\left(1,\ 0\right),\left(2,\ 0\right),\left(2,\ 1\right),\left(1,\ 0\right)\right)|red
\operatorname{polygon}\left(\left(2,\ 0\right),\left(3,\ 0\right),\left(3,\ 1.414\right),\left(2,\ 1\right)\right)|blue
\operatorname{polygon}\left(\left(3,\ 0\right),\left(4,\ 0\right),\left(4,\ 1.732\right),\left(3,\ 1.414\right)\right)|red
\operatorname{polygon}\left(\left(4,\ 0\right),\left(5,\ 0\right),\left(5,\ 2\right),\left(4,\ 1.732\right)\right)|blue
\operatorname{polygon}\left(\left(5,\ 0\right),\left(6,\ 0\right),\left(6,\ 2.236\right),\left(5,\ 2\right)\right)|red
```
This is a much better approximation of the area under the curve than the rectangular sum provided. 

We can calculate this area by adding the area of each trapezoid as such: $$Area\approx\frac{f(1)+f(2)}{2}\Delta x+\frac{f(2)+f(3)}{2}\Delta x+...+\frac{f(5)+f(6)}{2}\Delta x$$
or, we can combine like terms and factor into this, much more simple, form: $$Area\approx\frac{\Delta x}{2}(f(1)+2f(2)+2f(3)+2f(4)+2f(5)+f(6))$$
