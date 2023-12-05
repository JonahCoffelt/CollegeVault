#math #theorem 
Lets assume we have a function $f$ that is continuous over the closed interval $[a, b]$. It is also differentiable over the open interval $(a, b)$
```desmos-graph
left=.5; right=4.5;
bottom=-1;top=4;
---
-(x-3)^3-2(x-3)^2+3\ \left\{1<x<4\right\}
(1, 3)|black
(4, 0)|black
```

What the Mean Value Theorem tells us is that at some point over the open interval (at least once) the instantaneous [[Rate of Change]] will be equal to the average rate of change. The average rate of change is just the slope of the secant line from $a$ to $b$:
```desmos-graph
left=.5; right=4.5;
bottom=-1;top=4;
---
-(x-3)^3-2(x-3)^2+3\ \left\{1<x<4\right\}
-x+4
(1, 3)|black
(4, 0)|black
```
So, lets calculate this slope: $$m=\frac{\Delta y}{\Delta x}=\frac{f(b)-f(a)}{b-a}$$
Thus, by the mean value theorem, there is some $c$ such that  $a<c<b$, where the instantaneous rate of change is equal to the instantaneous rate of change. If we look at the graph, these points could be our $c$:
```desmos-graph
left=.5; right=4.5;
bottom=-1;top=4;
---
-(x-3)^3-2(x-3)^2+3\ \left\{1<x<4\right\}
-x+4
-(x-1.451) + 1.918|blue|dashed
-(x-3.215) + 2.898|blue|dashed
(1, 3)|black
(4, 0)|black
(3.215, 2.898)|blue
(1.451, 1.918)|blue
```
