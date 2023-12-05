#math 
![[Pasted image 20230811114157.png]]
Arc Length gives us the length of a non-linear portion of a function. 

To do this, we can sum a lot of really small linear lines along the curve. 
![[Pasted image 20230811114457.png]]
Thus our arc length would be: $$\int ds$$
However, we can use the Pythagorean theorem to express it like so: $$\int\sqrt{dx^2+dy^2}$$
Then we can factor out $dx^2$: $$\int\sqrt{dx^2(1+(\frac{dy}{dx})^2)}=\int\sqrt{1+(\frac{dy}{dx})^2}\mbox{ }dx$$
Thus the formula for Arc Length is: $$\int_a^b\sqrt{1+(f'(x))^2}\mbox{ }dx$$