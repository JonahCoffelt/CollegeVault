#math #derivative 
To model something like population, we would use an exponential model. Using differential equations, we can see where this comes from. 

Lets say $P=population$, $t=time(days)$, and $k=growth\mbox{ }constant$. Now lets define the rate of growth of the population with respect to time: $$\frac{dP}{dt}=kP$$This makes sense, as the larger the population is, the faster it is able to grow. Now, we should try to solve this differential equation. This is a [[Separable Differential Equations]], so lets separate the variables: $$\frac1P=kdt$$
Then integrate both sides: $$\int\frac1P=\int kdt$$
$$ln|P|=kt+C_1$$
To solve for P, exponentiate both sides (I removed the absolute value on P because the population is positve): $$P=e^{kt+C_1}$$
$$P=e^{kt}\cdot e^{C_1}$$ And since C is just some constant, and $e^{C_1}$ is *some* constant, we can rewrite as so: $$\boxed{P=Ce^{kt}}$$