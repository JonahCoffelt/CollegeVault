#math
An improper integral has one or two boundaries which are unbounded. For example, if we wanted to take the integral: $$\int_1^\infty\frac{1}{x^2}dx$$Then we would use this technique.

But first, lets take a look at what we are integrating in the first place:
```desmos-graph
left=0;right=6;
bottom=0;top=4;
---
1/x^2
0<y<\frac{1}{x^{2}}\left\{1<x\right\}|purple
```
We can see that this function nears the $x$ axis. In fact $lim_{x\rightarrow \infty}\frac{1}{x^2}=0$, so the area will actually converge to a real value. 

For us to do this, we should first make our integral proper by expressing it in the terms of a limit: $$lim_{b\rightarrow\infty}\int_1^b\frac1{x^2}dx$$This integral is actually completely valid, we just have to keep that [limit](Limits) attached. So lets evaluate with the normal techniques: $$lim_{b\rightarrow\infty}\int_1^bx^{-2}dx=lim_{b\rightarrow\infty}\frac{-1}{x}\bigg|_1^b$$
$$lim_{b\rightarrow\infty}(\frac{-1}{b}-\frac{-1}{1})$$
We can think about what will happen to the first fraction as b approaches infinity. It will get really really small, so small that we can say it is equal to 0. Thus we get a final answer of: $$\boxed{\int_1^\infty\frac{1}{x^2}dx=1}$$
Because it is a real number, we can say that this improper integral is convergent. 