#math
Lets say we have the function $y=\frac{15}x$ and we want to find the area between the y-axis and the function in the bounds $y=e$ and $y=e^3$. This is just like solving a normal integral, except we are in terms of y.
```desmos-graph
left=0; right=7;
bottom=0;top=23;
---
15/x
x+1>\left\{e<y<e^{3}\right\}\left\{0<x<\frac{15}{y}\right\}|purple
y=e|black|dashed
y=e^3|black|dashed
```

To do this, lets write our function in terms of y: $$x=\frac{15}y$$
We can now integrate using this function: $$15\int_e^{e^3}\frac1ydy=15ln|y|\bigg|_e^{e^3}$$
$$15ln|e^3| - 15ln|e|=45-15=\boxed{30}$$
If we wanted to do this between two curves, not the y-axis, we would do the same thing that we do in [[Area Between Curves]], but in terms of y. However, instead of doing top minus bottom, we do right minus left. 