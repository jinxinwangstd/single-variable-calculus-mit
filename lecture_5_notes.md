# Lecture 5: Implicit Differentiation

Implicit differentiation is a method that can expand our ability to differentiate functions. To use this method, we apply $\frac{d}{dx}$ to both sides of the function expression and according to the chain rule, the derivative is a factor inside the expression. Then we can get the derivative without calculating the explicit function expression. In lots of cases, using implicit differentiation is simpler than explicit differentiation.

Example 1: we already know that $\frac{d}{dx}x^a = a \cdot x^{a - 1}, a = 0, \pm1, \pm2, ...$. Let's explore the differentiation of $\frac{d}{dx}x^a$ when $a = \frac{m}{n}$ and $m, n$ are integers.

$y = x^{\frac{m}{n}}$

$y^n = x^m$

Apply $\frac{d}{dx}$ to both sides and the equation still holds.

$\frac{d}{dx}y^n = \frac{d}{dx}x^m$

According to the chain rule, we can get

$\frac{d}{dy}y^n \cdot \frac{dy}{dx} = \frac{d}{dx}x^m$

$ny^{n-1}\frac{dy}{dx} = mx^{m - 1}$

$nx^{\frac{m(n-1)}{n}}\frac{dy}{dx} = m x^{m-1}$

$\frac{dy}{dx}=\frac{m}{n}x^{m - 1 - \frac{mn - m}{n}}$

$\frac{dy}{dx}=\frac{m}{n}x^{\frac{m}{n}-1}$

Therefore, $\frac{d}{dx}x^a = a \cdot x^{a - 1}$ still holds when $a$ is a fraction.

Example 2: calculate the differentiation of $x^2 + y^2 = 1$ (positive branch). The explicit formula of the function is $y = \sqrt{1-x^2}$.

Explicit solution:

The explicit formula can be transformed to $y=(1-x^2)^{\frac{1}{2}}$

According to the chain rule, we can get

$\frac{dy}{dx}=\frac{1}{2}(1-x^2)^{-\frac{1}{2}} \cdot(-2x)$

$\frac{dy}{dx}=-x \cdot (1-x^2)^{-\frac{1}{2}}$

$\frac{dy}{dx}=-\frac{x}{\sqrt{1-x^2}}$

Implicit solution:

We apply $\frac{d}{dx}$ to both sides and the equation still holds.

$2x+2y\frac{dy}{dx}=0$

$\frac{dy}{dx}=-\frac{x}{y}$

$\frac{dy}{dx}=-\frac{x}{\sqrt{1-x^2}}$

Example 3: calculate the differentiation of $y^4 + xy^2 - 2 = 0$.

Explicit solution:

We need to calculate the explicit function expression first.

$y^2 = \frac{-x \pm \sqrt{x^2 - 4 \cdot(-2)}}{2} = \frac{-x \pm \sqrt{x^2 + 8}}{2}$

$y = \pm \sqrt{\frac{-x \pm \sqrt{x^2 + 8}}{2}}$

Implicit solution:

We apply $\frac{d}{dx}$ to both sides and the equation still holds.

$4y^3\frac{dy}{dx} + y^2 + x \cdot 2y\frac{dy}{dx} = 0$

$\frac{dy}{dx}=-\frac{y^2}{4y^3 + 2xy}$

Notice that the above formula is not a explicit derivative, but it enables us to calculate the derivative value at any given point on the function.

If we don't know the explicit function, we may not be able to calculate its explicit derivative. The point of implicit differentiation is to avoid differentiating the explicit function expression, therefore saving lots of effort. 

Inverse functions: in general, for $y=f(x)$ and $x = g(y)$. If $g(f(x)) = x$, then we say that the functions $f$ and $g$ are inverse functions, written as $f = g^{-1}$ and $g = f^{-1}$.

Implicit differentiation allows us to find the derivative of any inverse function provided that we know the derivative of the function.

Example 1: calculate the differentiation of $y=\tan^{-1}x$.

$y=\tan^{-1}x$

$\tan y = x$

We apply $\frac{d}{dx}$ to both sides and the equation still holds.

$\frac{d}{dy}\tan y \cdot \frac{dy}{dx} = \frac{d}{dx}x$

$\frac{dy}{dx}=\frac{1}{\frac{d}{dy}\tan y}$

Calculate the derivative of $\tan x$:

$\frac{d}{dx}\tan x = \frac{d}{dx}(\frac{\sin x}{\cos x})$

According to the quotient rule,

$\frac{d}{dx}(\frac{\sin x}{\cos x}) = \frac{\cos x \cdot \cos x - \sin x \cdot (-\sin x)}{\cos^2 x} = \frac{1}{\cos^2 x}$

$\frac{d}{dx}\tan x = \frac{1}{\cos^2 x}$

Therefore,

$\frac{dy}{dx}=\frac{1}{\frac{d}{dy}\tan y} = \frac{1}{\frac{1}{\cos^2 y}} = \cos^2 y$

$\frac{dy}{dx} = (\tan^{-1} x)^2$

If we construct a right triangle with an acute angle is $y$, and its opposite side is $x$, and adjacent side is $1$, then its hypotenuse is $\sqrt{1+x^2}$, and $\cos y = \frac{1}{\sqrt{1+x^2}}$. Therefore,

$\frac{dy}{dx} = \cos^2 y = (\frac{1}{\sqrt{1+x^2}})^2 = \frac{1}{1+x^2}$

数形结合

Example 2: calculate the differentiation of $y=\sin^{-1}x$.

$y=\sin^{-1}x$

$\sin y = x$

We apply $\frac{d}{dx}$ to both sides and the equation still holds.

$\frac{d}{dy}\sin y \cdot \frac{dy}{dx} = \frac{d}{dx}x$

$\frac{dy}{dx}=\frac{1}{\cos y} = \frac{1}{\sqrt{1-\sin^2y}} = \frac{1}{\sqrt{1-x^2}}$

数形结合