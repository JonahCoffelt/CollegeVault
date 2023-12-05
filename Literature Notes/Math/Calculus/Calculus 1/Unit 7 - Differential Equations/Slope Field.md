#math #derivative 
Lets say we are given the differential equation: $$\frac{dy}{dx}=\frac{-x}{y}$$And we don't know the solution, but we want to get an idea of what the solutions might look like. 

What we can do is plot a bunch of points like so:
```desmos-graph
left=-7.5;right=7.5;
bottom=-5;top=5;
---
m\left(x,\ y\right)=\frac{-x}{y}
l=\frac{1}{3}
w=10
p=\left[0...w^{2}-1\right]

\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5,\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)|blue
```
and begin to find the slope at that point, given our differential equation.

To do this, we can make a table like so:

| x   | y   | $\frac{dy}{dx}$ |
| --- | --- | --------------- |
| 0   | 1   | 0               |
| 1   | 1   | -1              |
| 1   | 0   | undefined       |
| -1  | -1  |  -1               |
| 1   | -1  | 1                |

Then, with this information, we can make a little line with the slope that we found on each point. If we do this enough, we can get a sense of what a solution might be:
```desmos-graph
left=-7.5;right=7.5;
bottom=-5;top=5;
---
m\left(x,\ y\right)=\frac{-x}{y}
l=\frac{1}{3}
w=10
p=\left[0...w^{2}-1\right]

\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5,\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)|blue

y-\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)=m\left(\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right),\ \left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)\right)\left(x-\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)\right)\left\{\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)-l<x<\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)+l\right\}\left\{\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)-l<y<\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)+l\right\}|black
```

But even with this, we still don't have any particular solution. What we can do to graph one is simply pick a point, and follow the lines. I like to think of it like a leaf in a stream, as it will just flow with the waters motion. Here is an example of on possible place we could drop our leaf (red dot):
```desmos-graph
left=-7.5;right=7.5;
bottom=-5;top=5;
---
m\left(x,\ y\right)=\frac{-x}{y}
l=\frac{1}{3}
w=10
p=\left[0...w^{2}-1\right]

\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5,\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)|blue

y-\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)=m\left(\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right),\ \left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)\right)\left(x-\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)\right)\left\{\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)-l<x<\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)+l\right\}\left\{\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)-l<y<\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)+l\right\}|black

(2, 2)|red
```
Then if, we follow the lines, this is the particular solution we get:
```desmos-graph
left=-7.5;right=7.5;
bottom=-5;top=5;
---
m\left(x,\ y\right)=\frac{-x}{y}
l=\frac{1}{3}
w=10
p=\left[0...w^{2}-1\right]

\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5,\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)|blue

y-\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)=m\left(\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right),\ \left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)\right)\left(x-\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)\right)\left\{\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)-l<x<\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)+l\right\}\left\{\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)-l<y<\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)+l\right\}|black

(2, 2)|red
x^{2}+y^{2}=8|red
```
Here, we can see that this is a circle. But remember, there are infinite solutions, not just this one, all of which are valid. 
```desmos-graph
left=-7.5;right=7.5;
bottom=-5;top=5;
---
m\left(x,\ y\right)=\frac{-x}{y}
l=\frac{1}{3}
w=10
p=\left[0...w^{2}-1\right]

\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5,\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)|blue

y-\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)=m\left(\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right),\ \left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)\right)\left(x-\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)\right)\left\{\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)-l<x<\left(\operatorname{mod}\left(p,\ w\right)-\frac{w}{2}+.5\right)+l\right\}\left\{\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)-l<y<\left(\frac{p-\operatorname{mod}\left(p,w\right)}{w}-\frac{w}{2}+.5\right)+l\right\}|black

(2, 2)|red
(-1, -1)|red
(4.5, 0)|red
x^{2}+y^{2}=8|red
x^{2}+y^{2}=2|red
x^{2}+y^{2}=20|red
```
