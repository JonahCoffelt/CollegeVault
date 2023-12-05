#math #approximation
If we are unable to analytically solve a differential equation, then we can approximate it.  

Lets practice how to do that given the following information: $$\frac{dy}{dx}=y\mbox{, y(0)=1}$$
We will use the given point as a starting point, then use the slope at that point to linearly walk over 1 unit $x$, adjusting for $y$ according to the slope. This will be a our new point, and we do the same thing unit we are at the $x$ value we want to approximate. 
$\Delta x=1$

| x   | y   | $\frac{dy}{dx}$ |
| --- | --- | --------------- |
| 0   | 1   | 1               |
| 1   | 2   | 2               |
| 2   | 4   | 4               |
| 3   | 8   | 8                |

![[Pasted image 20230811112411.png]]

Now, this isn't a great approximation, but it was easy to compute. If we wanted to get a more accurate solution, then we could use smaller steps on the $x$ axis
$\Delta x=.5$

| x   | y    | $\frac{dy}{dx}$ |
| --- | ---- | --------------- |
| 0   | 1    | 1               |
| .5  | 1.5  | 1.5             |
| 1   | 2.25 | 2.25            |
| ... | ...  | ...                |

If we were to continue this, it would be a better approximation.