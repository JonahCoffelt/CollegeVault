#math
The goal of Integration Using Linear Partial Fractions is to split one tricky ration function into the sum of two. Let's take a look at an example: $$\int\frac{x-5}{(2x-3)(x-1)}$$
Now, we split the rational function: $$\frac{x-5}{(2x-3)(x-1)}=\frac{A}{(2x-3)}+\frac{B}{(x-1)}=\frac{A(x-1)}{(2x-3)(x-1)}+\frac{B(2x-3)}{(2x-3)(x-1)}$$
Thus: $$x-5=A(x-1)+B(2x-3)$$
To solve for each value, we will use strategic $x$ values which will get rid of one variable: $$(1)-5=A((1)-1)+B(2(1)-3)$$
$$-4=-B$$
$$B=4$$ $$(\frac32)-5=A((\frac32)-1)+B(2(\frac32)-3)$$
$$\frac{-7}2=\frac12A$$
$$A=-7$$
Now, we can rewrite our initial integral as such: $$4\int\frac{1}{x-1}dx-\frac72\int\frac{2}{2x-3}dx$$
When evaluated, we get: $$\boxed{4ln|x-1|-\frac72ln|2x-3|+C}$$