A vector is a list of "things", though commonly it is a list of numbers.

The vector (4, 2) is a vector which moves 4 units $x$ and 2 units $y$. This can start at the origin as so: 
![[Pasted image 20230814001020.png]]
Or, it could start at some other point, like (0, 2), but the vector would remain the same. 
![[Pasted image 20230814001115.png]]

# Notation
There are many ways to notate a vector: $$\vec{v}=(1, 2, 3)=\begin{bmatrix} 1\\2\\3\end{bmatrix}=1i+2j+3k$$
The last notation uses the $i, j, k$ symbols as unit vectors, so $$i=(1, 0, 0), j=(0, 1, 0), k=(0, 0, 1)$$
# Addition
When we add two vectors, we simply add their corresponding components: $$(a, b, c)+(A, B, C)=(a+A,b+B,c+C)$$
We can imagine that we put the tail of the second vector on the tip of the first vector like so:
![[Pasted image 20230814002336.png]]

# Scalar Multiplication
A scalar multiplies an entire vector by one number: $$x\vec a=x(a, b, c)=(xa, xb, xc)$$
Here are some examples of this: $$\vec b=(1,2,3)$$
$$2\vec b=(2,4,6)$$
$$-\vec b=(-1,-2,-3)$$
this makes the vector look either stretched or shrunk:
![[Pasted image 20230814002740.png]]
# Magnitude
Magnitude is just how long the vector is. We notate magnitude with one or two bars: $|\vec a|$ or $||\vec a||$. This is easy to calculate with the Pythagorean Theorem:
![[Pasted image 20230814003001.png]]
