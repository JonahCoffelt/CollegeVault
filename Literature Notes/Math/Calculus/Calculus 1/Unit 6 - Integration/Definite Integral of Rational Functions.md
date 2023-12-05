#math #integral 
How do we evaluate the integral of the following function: $$\int_{-1}^{-2}(\frac{16-x^3}{x^3})dx$$
To start, we should rewrite the function so that it is easier to integrate: $$\int_{-1}^{-2}(\frac{16-x^3}{x^3})dx=\int_{-1}^{-2}(\frac{16}{x^3}-\frac{x^3}{x^3})dx=\int_{-1}^{-2}(\frac{16}{x^3}-1)dx$$
This is much easier, as we can integrate each term separately: $$\int_{-1}^{-2}(\frac{16}{x^3}-1)dx=\frac{16x^{-2}}{-2}-x\bigg|_{-1}^{-2}=\frac{-8}{x^2}-x\bigg|_{-1}^{-2}$$
Now we can evaluate this: $$(\frac{-8}{(-2)^2}-(-2))-(\frac{-8}{(-1)^2}-(-1))=(0)-(-7)=\boxed{7}$$