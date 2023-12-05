#math #integral 
Let's take a look at this integral that initially looks difficult and complicated by unwinding the [[Chain Rule]]. This is our integral: $$\int(3x^2+2x)e^{(x^3+x^2)}dx$$ This first thing to notice is that $(3x^2+2x)$ is the derivative of $(x^3+x^2)$, which means we can use U-Substitution. So what we do here is define $u$ as $(x^3+x^2)$: $$u=(x^3+x^2)$$
Additionally, we can define the derivative of $u$: $$\frac{du}{dx}=(3x^2+2x)$$ With this, we can define $du$: $$du=(3x^2+2x)dx$$
Given these, we can actually rewrite the integral in terms of $u$ (I boxed off $u$ and $du$): $$\int e^{\boxed{(x^3+x^2)}}\cdot \boxed{(3x^2+2x)dx}=\int e^udu$$
Already, we can see that this is *much* simpler. We can easily integrate in terms of $u$ as such: $$\int e^udu=e^u+C$$
Finally, we can put it back in terms of $x$ by replacing all instances of $u$ with $(x^3+x^2)$: $$e^u+C=\boxed{e^{(x^3+x^2)}+C}$$
# Multiplying by a Constant
We are given the integral: $$\int\sqrt{7x+9}dx$$
If we try to use U-Substitution, these are the values we have to work with: $$u=7x+9$$
$$\frac{du}{dx}=7$$
$$du=7dx$$
Because we don't have a $7dx$ in our integral, you need to manipulate the constants. There are many ways to do this, but I prefer to solve for $dx$ in terms of $du$, and just use that:
$$dx=\frac17du$$
Now, we have something we can put in place of $dx$ to fully put the integral in terms of $u$: $$\int\sqrt{7x+9}dx=\int\sqrt{u}\cdot\frac17du$$By using properties of [[Definite Integrals]] (which, when applicable, work for indefinite integrals), we can rewrite the integral as such: $$\frac17\int\sqrt udu=\frac17\int u^{\frac12}du$$
To antidifferentiate, use the [[Reverse Power Rule]]: $$\frac17\int u^{\frac12}du=\frac17\cdot \frac23u^{\frac32}+C=\frac{2}{21}u^{\frac32}+C$$
Finally, put it back in terms of $x$: $$\frac{2}{21}u^{\frac32}+C=\frac{2}{21}(7x+9)^{\frac32}+C$$
