#math 
A definite integral gives the area under a function between two $x$ values, $a$ and $b$: $$\int_a^bf(x)dx$$
# Properties of Definite Integrals
## Negative Integrals
Given a function that goes bellow the x axis, the area bellow will be negative. The area above remain positive.
![[Pasted image 20230809103551.png]]
This may seem counter intuitive, as area cannot be negative, however, the accumulation of change can be positive. For example, if a particle was moving at a rate of $3\frac ms$ for 4 seconds, it would have moved 12 meters in the positive direction. By contrast, a particle moving $-3\frac ms$ for 4 seconds would have moved 12 meters in the *negative* direction. 
## Definite Integral over a Single Point
$$\boxed{\int_a^af(x)dx=0}$$This makes sense, as the base is equal to 0, thus there is no area.

## Integration of a Scaled Function (Constant Coefficient Rule)
Lets assume we have a function $f(x)$ and a scaled version of it: $$y=c\cdot f(x)$$
Then: $$\boxed{\int_a^bc\cdot f(x)=c\int_a^bf(x)}$$

## Switching Bounds of Definite Integrals
$$\boxed{\int_b^af(x)dx=-\int_a^bf(x)dx}$$

## Integrating Sums of Functions
$$\boxed{\int_a^bf(x)dx+\int_a^bg(x)dx=\int_a^b(f(x)+g(x))dx}$$

## Definite Integrals on Adjacent Intervals
Where $a\le c\le b$ 
```desmos-graph
left=-.5;right=2.5;
bottom=0;top=5;
---
x^2|black
0<y<x^{2}\left\{0<x<1\right\}
0<y<x^{2}\left\{1<x<2\right\}
x=0|dashed|red
x=2|dashed|red
(0, 0)|black|label:A
(1, 0)|black|label:C
(2, 0)|black|label:B
```
$$\boxed{\int_a^bf(x)dx=\int_a^c f(x)dx+\int_c^bf(x)dx}$$
