#math #inverse #trig
# Derivatives of Inverse Trigonometric Functions

## Derivative of $sin^{-1}x$
Given the function: $$y=sin^{-1}x$$ How do we find $y'$?

To start, let's rewrite using the property of inverse functions: $$sin(y)=x$$ Now, we can implicitly differentiate: $$cos(y)\frac{dy}{dx}=1$$
$$\frac{dy}{dx}=\frac1{cos(y)}$$
Now, we can use a trig identity as follows: $$sin^2y+cos^2y=1$$
$$cos^2y=1-sin^2y$$
$$cos(y)=\sqrt{1-sin^2y}$$
With this, we can rewrite our derivative solution: $$\frac{dy}{dx}=\frac{1}{\sqrt{1-sin^2y}}$$
And since we know that $sin(y)=x$, we can simply substitute $x$ back in so that our derivative is in terms of $x$: $$\frac{dy}{dx}=\frac{1}{\sqrt{1-x^2}}$$
Now we know that:
$$\boxed{\frac{d}{dx}[sin^{-1}x]=\frac{1}{\sqrt{1-x^2}}}$$
### My Weird Trig Solution (It does actually work lol, but not what you're supposed to do)
To start, we use the rules of the [[Derivatives of Inverse Functions]], which states that, assuming $f(x)$ and $g(x)$ are inverses: $$f'(x)=\frac{1}{g'(f(x))}$$
Next, we can define $g(x)=sinx$ and $f(x)=sin^{-1}x$. Furthermore we know that $\frac{d}{dx}[sinx]=cosx \therefore g'(x)=cosx$. Using this, we can substitute the functions into the previously mentioned functions for inverse derivatives like so: $$\frac{d}{dx}[sin^{-1}x]=f'(x)=\frac{1}{cos(sin^{-1}x)}$$
## Derivative of $cos^{-1}x$
Find the derivative of the following: $$y=cos^{-1}x$$
To start, let's rewrite using the inverse function rules: $$x=cos(y)$$
Differentiate both sides and solve for $\frac{dy}{dx}$: $$1=-sin(y)\frac{dy}{dx}$$
$$\frac{dy}{dx}=\frac{-1}{sin(y)}$$
Then let's manipulate the trig identity for and sub in when we can: $$sin^2y+cos^2y=1$$
$$sin^2y=1-cos^2y$$
$$sin(y)=\sqrt{1-cos^2y}$$
$$sin(y)=\sqrt{1-x^2}$$
Thus our final solution is: $$\boxed{\frac{d}{dx}[cos^{-1}x]=\frac{-1}{\sqrt{1-x^2}}}$$
## Derivative of $tan^{-1}x$
Find the derivative of the following: $$y=tan^{-1}x$$
First, rewrite using inverse property:
$$x=tan(y)$$
Differentiate both sides and solve for $\frac{dy}{dx}$: $$1=sec^2(y)\frac{dy}{dx}$$
$$\frac{dy}{dx}=\frac1{sec^2y}=cos^2y$$
Now use trig identities to rewrite: $$cos^2y=\frac{cos^2y}{cos^2y+sin^2y}\cdot\frac{\frac{1}{cos^2y}}{\frac{1}{cos^2y}}=\frac{1}{1+\frac{sin^2y}{cos^2y}}=\frac{1}{1+tan^2y}=\frac{1}{1+x^2}$$
Thus: $$\boxed{\frac{d}{dx}[tan^{-1}x]=\frac1{1+x^2}}$$
