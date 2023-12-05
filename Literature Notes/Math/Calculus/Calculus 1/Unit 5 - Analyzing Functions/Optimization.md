#math #derivative 
# Sum of Squares Problem
What is the smallest possible sum of squares of two numbers, if their product is -16?

Lets first assume the we have two numbers, $x$ and $y$, and that $x\cdot y=-16$
We are trying to minimize their sum, which can be represented as such: $$S=x^2+y^2$$Because $S$ is in the terms of two variables, we should try to represent it using only one. Luckily, we can use our first equation, $x\cdot y=-16$, to substitute for y, as $y=\frac{-16}{x}$. Thus, our sum can now be defined as: $$S(x)=x^2+(\frac{-16}{x})^2=x^2+256x^{-2}$$
Now we can differentiate this function: $$S'(x)=2x+-512x^{-3}$$
Let's use the second derivative test for this problem, so set $S'(x)=0$: $$0=2x-512x^{-3}=2x(1-256x^{-4})$$ $$x=0$$
and $$1=\frac{256}{x^4}$$
$$x=\sqrt[4]{256}=\pm4$$
lets try $x=4$, by checking that the function is concave up at that point: $$S''(x)=2+1536x^{-4}$$
$$S''(4)=2+1536(4)^{-4}$$
This is positive, so we have a minimum at x=4. Thus:
$$x=4 \mbox{ and }y=-4$$
Therefore:
$$S=4^2+4^2=\boxed{32}$$