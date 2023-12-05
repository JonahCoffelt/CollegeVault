#math #limit #continuity #DNE #undefined
# Limits
- Idea that most of Calculus is based upon
- Describes the behavior of a function as it approaches a point. Therefore, it says nothing of the value of a function at a given point

The following [[Equation]] may seem to simplify easily, but there must be the constraint because the f(1) is [[Undefined]] 
$$f(x) = \frac{x-1}{x-1} \rightarrow f(x)=1, x\neq1$$
```desmos-graph
left=-.5; right=1.5;
top=1.5; bottom=-.5
---
y=(x-1)/(x-1)|blue
(1, 1)|blue|open
```
Therefore, $lim_{x\to 1}f(x)=1$ Because that is what the function approaches as we get closer and closer to x=1 on either side
```desmos-graph
left=.5; right=5;
top=8; bottom=-.5
---
x+1\left\{x<3\right\}|#37871F
x+3\left\{x>3\right\}|#37871F
(3, 4)|open|#37871F
(3, 6)|#37871F
```
If a function approaches different values from either side, then the limit DNE (does not exist)
Therefore, $lim_{x\to 3}f(x)=DNE$ because it approaches different values from either side

```desmos-graph
left=-4; right=6;
top=12; bottom=-.25
---
y=1/x^2|red
x=0|dotted|black
```
In this example, $lim_{x\to 0}f(x)=\infty$  because f(x) increases without bounds as x approaches 0 from both sides. This may also be said to be unbounded
# One-Sided Limits
Instead of evaluating the limit from both sides, we can evaluate the limit from either side:
- '+' means approaching from the right
- '-' means approaching from the left
```desmos-graph
left=.5; right=5;
top=8; bottom=-.5
---
x+1\left\{x<3\right\}|#37871F
x+3\left\{x>3\right\}|#37871F
(3, 4)|open|#37871F
(3, 6)|#37871F
```
In this example, $lim_{x\to 3^-}f(x)=4$ because f(x) gets closer to 4 as x approaches 3 from the negative (left) side
furthermore, $lim_{x\to 3^+}f(x)=6$ because f(x) gets closer to 6 as x approaches 3 from the positive (right) side
# Limits with Tables

$$f(x)=\frac{x^3-3x^2}{5x-15}$$
Given the function f(x) what is the limit as x approaches 3? If we try to find the value at 3, the function is [[undefined]]:
$$f(3)=\frac{(3)^3-3(3)^2}{5(3)-15}=\frac{0}{0}$$
Therefore, we must use a table (or graph as shown above) in order to find the limit:

| x | $\frac{x^3-3x^2}{5x-15}$ |
| - | - |
| 2.9 | 1.682 |
| 2.99 | 1.788 |
| 2.999 | 1.7988 |
| 3.001 | 1.801 |
| 3.01 | 1.812 |
| 3.1 | 1.922 |

From this table, it can be that $lim_{x\to 3}f(x)=1.8$