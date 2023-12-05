#math #polar #integral 
When we thought about taking an integral in rectangular coordinates, we used the sum a lot of small rectangles to find the area. With polar, that doesn't make sense, so instead, we use a lot of tiny circle sectors like so:
![[Pasted image 20230813153819.png]]
The radius of a sector is: $$A_{sector}=\frac12r^2\theta$$
In this use, the $\theta$ is getting really really small, so we can write it as such: $$A_{sector}=\frac12r^2d\theta$$
Now, we just integrate of of these areas together like so: $$\int_\alpha^\beta\frac12r^2d\theta=\frac12\int_\alpha^\beta r^2d\theta$$