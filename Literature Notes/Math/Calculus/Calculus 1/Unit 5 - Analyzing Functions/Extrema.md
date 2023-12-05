#math 
# Relative Extrema
```desmos-graph
left=.5; right=4.5;
bottom=-1;top=5;
---
-(x-3)^3-2(x-3)^2+3\ \left\{.75<x<4\right\}
```
In the above function, we can see that the maximum and minimum points are the two ends. However, in-between them there are also to relative maximum and relative minimum points. These points look like little hills or valleys. Although we can clearly see these points, we could also fund these points by taking the derivative of the function and setting it equal to 0: $$f'(x)=0$$
This makes sense, as at these points, the function levels out and become flat (think about throwing an object in the air, before it starts falling down, there is a brief period where it is not moving), thus the derivative, or the instantaneous rate of change, is equal to 0. Here is a quick example: 
``` desmos-graph
left=-3; right=3;
bottom=0; top=8;
---
x^2 + 1
y=1
```
You can see that when the derivative is equal to 0, we have a local minimum. However, this will not always be the case.

# First Derivative Test
To start, yes, we take the derivative of the function, and set it equal to 0. This point is called a [[critical point]]. However, for this point to be a maximum, $f(x)$ must change from increasing to decreasing, and for this point to be a minimum, $f(x)$ must change from decreasing to increasing. In the above example, we can see that that $f'(0)=0$ thus it is a critical point. It also changes from decreasing to increasing at this point, so it is also a relative (and in this case absolute) minimum. 

![[First Derivative Test]]

# Second Derivative Test
![[Second Derivative Test]]
# Absolute Extrema
To find the absolute extrema of a function on a closed interval, simply find all the relative extrema and find the most extreme of those points and the end points of the interval. 