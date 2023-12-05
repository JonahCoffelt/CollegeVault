#math #volume
We have the function $y=x^2$
```desmos-graph
left=0;right=2.5;
bottom=-.5; top=6;
---
x^2
0<y<x^{2}\left\{0<x<2\right\}|purple
```
And we want to find the volume of the cone-like shape that would be produced if we were to rotate the function around the $x$-axis $360\degree$. We could view this as a lot of circles stacked on top of each other, getting bigger as $x$ increases. The radius of these circles would just be the height of the graph at that point. Thus, the area of the circle at any given $x$ value is: $$Area=\pi(x^2)^2=\pi x^4$$
Now we can integrate across our bounds, $[0,2]$, as this would take the sum of the area of all of our circles: $$\pi\int_0^2x^4dx=\pi(\frac15x^5)\bigg|_0^2=\boxed{\frac{32\pi}{5}}$$