#math #trig #substitution 
Let's try to evaluate the indefinite integral: $$\int\frac{1}{\sqrt{4-x^2}}dx$$
We can notice that the bottom looks like something we would see when using the Pythagorean Theorem:
![[Pasted image 20230810192106.png]]
From this, we know that: $$sin\theta=\frac x2$$
$$x=2sin\theta$$
$$dx=2cos(\theta) d\theta$$
And: $$cos\theta=\frac{\sqrt{4-x^2}}{2}$$
$$\sqrt{4-x^2}=2cos\theta$$
Now, we can substitute the original integral: $$\int\frac{2cos\theta}{2cos\theta}d\theta=\int d\theta=\theta+C$$ Now we should solve for $\theta$: $$x=2sin\theta$$
$$\frac x2=sin\theta$$
$$\theta=sin^{-1}\frac x2$$
So our final answer is: $$\boxed{sin^{-1}\frac x2+C}$$