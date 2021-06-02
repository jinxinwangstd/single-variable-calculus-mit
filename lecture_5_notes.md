# Lecture 5: Implicit Differentiation

Implicit differentiation is a method used to extend the differentiation we can calculate.

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

Inverse functions: in general, for $y=f(x)$ and $x = g(y)$. If $g(f(x)) = x$, then we say that the functions $f$ and $g$ are inverse functions, written as $f = g^{-1}$ and $g = f^{-1}$.

Implicit differentiation allows us to find the derivative of any inverse function provided that we know the derivative of the function.

Example 1: calculate the differentiation of $y=\tan^{-1}x$.

The inverse function of the above function is $y=\tan x$.

According to the quotient rule, the derivative of the function $y = \tan x$ is

$\frac{dy}{dx}=\frac{d}{dx}\frac{\sin x}{\cos x} = \frac{\cos x \cdot \cos x - \sin x \cdot (-\sin x)}{\cos^2 x} = \frac{1}{\cos^2 x}$