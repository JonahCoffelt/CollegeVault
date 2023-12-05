#math #derivative 

# Straight-line Motion
Given the following function for position: $$x(t)=t^3-3t^2+5\mbox{, }t\ge0$$
To understand this, we can set up a table:

| $t$ ($seconds$) | $x$ |
| --------------- | --- |
| 0               | 5   |
| 1               | 3   |
| 2               | 1   |
| 3               | 5    |

Additionally, we can graph the function:
```desmos-graph
left=0;right=3;
bottom=-6;top=6;
---
x^3-3x^2+5
(0,5)|black|label
(1,3)|black|label
(2,1)|black|label
(3,5)|black|label
```

Now, if we wanted to find our velocity as a function of time, $v(t)$, all we need to do is take the derivative of the function for position: $$v(t)=x'(t)=3t^2-6t\mbox{, }t\ge0$$
```desmos-graph
left=0;right=3;
bottom=-6;top=6;
---
x^3-3x^2+5
3x^2-6x
```

When we compare the two graphs, it intuitively makes sense at any given point. Specifically, when it changes from going down to up, the velocity changes from negative to positive. 

In addition to this, we can find the acceleration with respect to time, $a(t)$, by taking the derivative of the velocity: $$a(t)=v'(t)=x''(t)=6t-6t\mbox{, }t\ge0$$
```desmos-graph
left=0;right=3;
bottom=-6;top=6;
---
x^3-3x^2+5
3x^2-6x
6x-6
```
