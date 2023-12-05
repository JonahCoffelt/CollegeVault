#math #limit #derivative 

Traditionally, we use [[Limits]] to figure out [[_Derivatives]], however, we can use derivatives to find a limit that seems to be [[Undefined]]. To do that, we use L'Hopital's rule.

# L'Hopital's Rule
If: $$lim_{x\rightarrow c}f(x)=0 \mbox{ and } lim_{x\rightarrow c}g(x)=0 \mbox{ and } lim_{x\rightarrow c}\frac{lim_{x\rightarrow c}f'(x)}{lim_{x\rightarrow c}g'(x)} =L \mbox{ (exists)}$$
Then: $$lim_{x\rightarrow c}\frac{lim_{x\rightarrow c}f(x)}{lim_{x\rightarrow c}g(x)} =L$$
This may also apply if the first to limits are unbounded ($\pm\infty$)
In other words, we can take the derivative of the top and the bottom of a limit, and it will give us the same answer. 

## Example:
Given the limit: $$lim_{x\rightarrow0}\frac{sin(x)}{x}$$
We get $\frac00$, so we can use L'Hopital's rule as so: $$lim_{x\rightarrow0}\frac{sin(x)}{x}=lim_{x\rightarrow0}\frac{cos(x)}{1}=\frac{cos(0)}{1}=1$$
Therefore: $$lim_{x\rightarrow0}\frac{sin(x)}{x}=1$$