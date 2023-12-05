#math #theorem #squeeze
# Squeeze Theorem (Sandwich Theorem)

- Used to find the limit of tricky functions.

Given 3 functions with the following inequality:$$f(x)\le g(x)\le h(x)$$If $f(c)=h(c)$ then both are equal to $g(c)$
## Example 1
$f(x)=x^2$
$g(x) = x^2sin(\frac{1}{x})$
$h(x)=-x^2$
```desmos-graph
left=-.5;right=.5;
bottom=-.25;top=.25;
---
x^2
-x^2
x^2*\sin(1/x)
(0, 0)
```
Because $f(0)=h(0)$, $g(0)$ is also equal.

This can be used to find tricky limits, such as $lim_{x\rightarrow 0}g(x)$ by "squishing" it between to easier functions. In this example, $$lim_{x\rightarrow 0}f(x)=0 \mbox{ and }lim_{x\rightarrow 0}h(x)=0 \therefore lim_{x\rightarrow 0}g(x)=0$$
## Example 2
<iframe width="560" height="315" src="https://www.youtube.com/embed/5xitzTutKqM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
