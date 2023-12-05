#math #continuous #discontinuous
$f(x)\mbox{ is continuous at x=c if and only if } lim_{x\rightarrow c}f(x)=f(c)$
# Point / Removable Discontinuity
```desmos-graph
left=-5;right=5;
bottom=-1;top=5;
---
x^2|blue
(2, 4)|blue|open
(2, 2)|blue
```
Although $lim_{x\rightarrow 2}f(x)=4 \mbox{, } f(2) = 2$, therefore it is not continuous
# Jump Discontinuity
```desmos-graph
left=-6;right=6;
bottom=-1;top=10;
---
x^2\left\{x<2\right\}|purple
\log(x)+2\left\{x>2\right\}|purple
(2, 4)|purple|open
```
Both $lim_{x\rightarrow 2^-}f(x)$ and $lim_{x\rightarrow 2^+}f(x)$ exist, but they are different values
# Asymptotic Discontinuity
```desmos-graph
left=-6;right=6;
bottom=-1;top=10;
---
1/(x-2) + 5
x=2|dashed|orange
```
There is an asymptote. f(x) increases/decreases without bounds as x approaches 2