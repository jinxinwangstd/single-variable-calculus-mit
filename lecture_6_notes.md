# Lecture 6: Exponential and Log

Exponential functions:

We have a base $a$. Then we have $a^0 = 1$, $a^1 = a$, $a^2 = a \cdot a$, and so on.

Then we know the following property for exponential functions:

$a^{x_1 + x_2} = a^{x_1} \cdot a^{x_2}$

$a^{x_1 \cdot x_2} = (a^{x_1})^{x_2} = (a^{x_2})^{x_1}$

With the above properties, the exponential function values with integer powers are defined.

For rational powers, we define their values as the following property:

$a^{\frac{m}{n}} = \sqrt[n]{a^m}$

For irrational powers, we define their values by "filling in" the gaps in the exponential function to maintain continuity.

Derivative of exponential function $a^x$.

According to the definition of derivatives,

$\frac{d}{dx}a^x = \lim_{\Delta x \to 0} \frac{a^{x + \Delta x} - a^x}{\Delta x}$

$\frac{d}{dx}a^x = \lim_{\Delta x \to 0} a^x \cdot \frac{a^{\Delta x} - 1}{\Delta x}$

$\frac{d}{dx}a^x = a^x \cdot \lim_{\Delta x \to 0} \frac{a^{\Delta x} - 1}{\Delta x}$

Apparently $\lim_{\Delta x \to 0} \frac{a^{\Delta x} - 1}{\Delta x}$ is a function of $a$, so we can write it as $M(a) = \lim_{\Delta x \to 0} \frac{a^{\Delta x} - 1}{\Delta x}$. Then the above expression turns into

$\frac{d}{dx}a^x = M(a) \cdot a^x$

Notice that the value of the derivative at $x = 0$ is $M(a)$ because

$\frac{d}{dx}a^x|_{x = 0} = M(a) \cdot a^0 = M(a)$

Therefore, $M(a)$ is the slope of the graph of the exponential function $a^x$ at $x = 0$. By figuring out the slope at $x = 0$, we can then calculate the slope at any point.

What is $M(a)$?

Define a number $e$ as the unique number so that $M(e) = 1$.

With that being said, we can deduce that $\frac{d}{dx}e^x = e^x$.

Why does $e$ exist?

Suppose $f(x)= 2^x$, then we know $\frac{d}{dx}f(x)|_{x=0} = f'(0) = M(2)$.

If we stretch the function horizontally by $k$, then

$f(kx) = 2^{kx} = (2^k)^x$

Suppose $b = 2^k$, then $f(kx) = b^x$. Its derivative

$\frac{d}{dx} b^x = \frac{d}{dx}f(kx) = k \cdot f'(kx)$

$\frac{d}{dx} b^x|_{x=0} = k \cdot f'(0) = k \cdot M(2)$

It tells us that when $k$ increases, we shrink the graph and the slope at $x = 0$ increases till infinity, and when k decreases, we expand the graph and the slope at $x = 0$ decreases till 0.

Therefore, there must be a value for $k$ to stretch the function as $e^x$. When $k = \frac{1}{M(2)}$, $b = e$.

Logarithmic functions:

Logarithmic functions are the inverse function of exponential functions.

$\log_a x_1 \cdot x_2 = \log_a x_1 + \log_a x_2$

$\log_a 1 = 0$

Notice that $x > 0$ must hold for all logarithmic functions.

Natural Log

Natural log $\ln$ is the inverse function of the exponential function $e^x$, in other words, it is the logarithmic function with the base as $e$.

$\ln e = 1$

Calculate the derivative of natural logarithmic function $y = \ln x$.

$y = \ln x$

$e^y = x$

Use implicit differentiation we can get

$\frac{d}{dx}e^y = \frac{d}{dx}x$

$e^y \cdot \frac{dy}{dx} = 1$

$\frac{dy}{dx} = \frac{1}{e^y}$

$\frac{dy}{dx} = \frac{1}{x}$

To differentiate any exponential functions, we have two methods:

Method 1: convert the function to base $e$.

$a^x = (e^{\ln a})^x = e^{x \cdot \ln a}$

$\frac{d}{dx} a^x = \frac{d}{dx} e^{x \cdot \ln a}$

According to the chain rule, since $a$ is a constant,

$\frac{d}{dx} e^{x \cdot \ln a} = e^{x \cdot \ln a} \frac{d}{dx}(x \cdot \ln a) = e^{x \cdot \ln a} \cdot \ln a = \ln a \cdot a^x$

Therefore, $M(a) = \ln a$.

Method 2: logarithmic differentiation. To calculate the derivative of an exponential function $f(x) = a^x$, we can first calculate the derivative of the function $\ln f$.

$\frac{d}{dx}\ln f(x) = \frac{1}{f(x)} \cdot \frac{d}{dx} f(x) = \frac{f'(x)}{f(x)}$

$\frac{d}{dx}\ln a^x = \frac{\frac{d}{dx}a^x}{a^x}$

$\frac{d}{dx}(x\ln a) = \frac{\frac{d}{dx}a^x}{a^x}$

$\ln a = \frac{\frac{d}{dx}a^x}{a^x}$

$\frac{d}{dx} a^x = \ln a \cdot a^x$

Therefore, $M(a) = \ln a$.

Example 1: calculate the derivative of the function $f(x) = x^x$. Such functions are called moving exponents.

$\ln f(x) = \ln x^x = x \cdot \ln x$

$\frac{d}{dx} \ln f(x) = \frac{d}{dx}(x \cdot \ln x) = 1 + \ln x$

As $\frac{d}{dx} \ln f(x) = \frac{f'(x)}{f(x)}$, we can get

$f'(x) = f(x) \cdot \frac{d}{dx} \ln f(x) = x^x \cdot (1 + \ln x)$

Example 2: calculate $\lim_{n \to \infty} (1 + \frac{1}{n})^n$. 

$\ln ((1+\frac{1}{n})^n) = n \cdot \ln (1+\frac{1}{n})$

Suppose $\Delta x = \frac{1}{n}$, when $n \to \infty$, $\Delta x \to 0$. Then we can rewrite the above expression as

$\lim_{n \to \infty} \ln((1+\frac{1}{n})^n) = \lim_{n \to \infty} n \cdot \ln(1+\frac{1}{n}) = \lim_{\Delta x \to 0} \frac{1}{\Delta x} \cdot \ln (1 + \Delta x)   = \lim_{\Delta x \to 0} \frac{1}{\Delta x} \cdot (\ln (1 + \Delta x) - \ln 1) = \lim_{\Delta x \to 0}\frac{\ln(1+\Delta x) - \ln 1}{\Delta x} = \frac{d}{dx}\ln x|_{x=1} = (\frac{1}{x})|_{x=1} = 1$

Since $\lim_{n \to \infty}\ln((1+\frac{1}{n})^n) = 1$, we can deduce that

$\lim_{n \to \infty} (1+\frac{1}{n})^n = e$

The above formula is one of the numerical approach to calculate or approximate the value of $e$.