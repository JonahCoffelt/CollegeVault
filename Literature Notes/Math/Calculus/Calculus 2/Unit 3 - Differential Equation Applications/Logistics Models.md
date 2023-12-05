#math
Although we often use an [[Exponential Model]] to model a population, this is often unrealistically, because the environment cannot support an unbounded population. Because of this, it is important to consider the population capacity, $k$, of the environment. 

Thus, instead of the normal Exponential Model: $$\frac{dP}{dt}=rP$$
Which only considers the population size, we can use the logistics model which dampens the growth near the capacity, while still maintain exponential-like growth early on: $$\frac{dP}{dt}=rP(1-\frac{P}{k})$$
Which would look something like this:
![[Pasted image 20230811113954.png]]

