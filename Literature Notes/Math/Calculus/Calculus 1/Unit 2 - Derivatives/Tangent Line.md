#math #rateofchange #tangent 
# Tangent Line
A tangent line only intersects a function at one point:
```desmos-graph
left=-3;right=3;
bottom=-1;top=5;
---
x^2
2x-1
(1, 1)|black
```
The slope of the tangent is equivalent to the derivative of the function at the point of intersection
## Example
Given the function: $$f(x)=\frac{e^x}{2+x^3}$$
Find the equation of the tangent line at the point $(1, \frac{e}{3})$
To do this, we must find the derivative of $f(x)$: $$f'(x)=\frac{e^x(2+x^3)-3x^2e^x}{(2+x^3)^2}$$
Then, to find the slope of the tangent: $$f'(1)=\frac{e^1(2+(1)^3)-3(1)^2e^1}{(2+(1)^3)^2}=\frac{3e-3e}{9}=0$$
We can use the [[Point Slope]] formula to find the tangent equation now, given $m=0$: $$y-\frac{e}{3}=0(x-1) \rightarrow y=\frac{e}{3}$$
```desmos-graph
left=0;right=2;
bottom=0;top=2;
---
y=(e^x)/(2+x^3)
y=e/3
(1, e/3)
```

