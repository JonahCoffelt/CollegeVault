#math #derivative 
Let's say we want to find the particular solution that passes through the point $(0, 1)$ of the following differential equation: $$\frac{dy}{dx}=\frac{-x}{ye^{x^2}}$$
First, we should separate all of the x variables and y variables. Put x on one side, and y on the other: $$ydy=-xe^{-x^2}dx$$Then, we can integrate both sides with respect to their respective variable: $$\int ydy=\int-xe^{-x^2}dx$$
$$\frac12y^2+C_1=\frac12e^{-x^2}+C_2$$
$$\frac12y^2=\frac12e^{-x^2}+C$$
Now, we should use the given point to solve for $C$: $$\frac12(1)^2=\frac12e^{-(0)^2}+C$$
$$\frac12=\frac12(1)+C$$
$$C=0$$
Now, we can solve for $y$ in our particular solution: $$y^2=e^{-x^2}$$
$$y=\sqrt{e^{-x^2}}$$
$$\boxed{y={e^{\frac{-x^2}2}}}$$
