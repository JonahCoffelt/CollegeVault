#math #volume
# Square and Rectangle Cross Section

![[Pasted image 20230810164328.png]]
**Visual of this type of problem, though the picture is of a different problem**

The base of a solid is the region enclosed by the graphs of $y=-x^2+6x-1$ and $y=4$ Cross sections of the solid perpendicular to the $x$-axis are rectangles whose height is $x$. 

**Express the volume of the solid with a definite integral.**

To start, we should find the bounds that we are going to be working with in this problem by setting the functions equal to each other to find their intersections: $$0=x^2-6x+5$$
$$0=(x-1)(x-5)$$
$$x=1, 5$$

We should also consider what equation we will be using for the cross section shapes. For a rectangle, it is simply: $$Area=base\cdot height$$
For the height, we already know it to be $x$. To find the base, we simply take the vatical length of the base of the solid at that x value. In other words, we want the difference between the top function and the bottom function. To find which one is on the top, we can simply plug in one value in the bounds: $$-(2)^2+6(2)-1>4$$
Thus, the base of the rectangles will be: $$base=(-x^2+6x-1)-(4)=-x^2+6x-5$$
Now we have everything we need to find the area of a cross section rectangle: $$A=(-x^2+6x-5)\cdot x$$
Finally, to get the volume of the solid, we integrate across the base of the solid: $$Volume=\int_1^5(-x^3+6x^2-5x)dx$$
# Semicircle Cross Section
Let's say we have a solid whose base is the region under the function of $y=-x+1$, and we know that a cross section of this shape, perpendicular to the $x$-axis, will be a semicircle. How can we find the volume of this figure. 
![[Pasted image 20230810163407.png]]
To start, we should consider the equation for the area of a semicircle: $$Area=\frac12\pi r^2$$
So all we need to find is $r$. We know that the circumference each cross section is just equal to the height of the base, thus the radius is just half of that: $$r=\frac12(-x+1)=\frac{-x+1}2$$
Thus the area of each cross section is: $$Area=\frac12\pi(\frac{-x+1}2)^2$$ Finally, integrate over the entire solid's base: $$\frac{\pi}2\int_0^1(\frac{-x+1}2)^2dx$$
Now, I will show the steps to evaluate this integral: $$\frac{\pi}2\int_0^1(\frac{x^2-2x+1}4)dx=\frac{\pi}8\int_0^1(x^2-2x+1)dx=\frac{\pi}8(\frac13x^3-x^2+x)\bigg|_0^1$$
$$\frac{\pi}8(\frac13(1)^3-(1)^2+(1))-\frac{\pi}8(\frac13(0)^3-(0)^2+(0))=\boxed{\frac{\pi}{24}}$$
