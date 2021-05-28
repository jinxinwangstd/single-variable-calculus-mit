# Lecture 4: Chain Rule

General rules for derivatives:

$(c \cdot u)' = c \cdot u'$

$(u + v)' = u' + v'$

Production Rule: $(u \cdot v)' = u' \cdot v + u \cdot  v'$.

Proof:

$\Delta(uv) \\ = u(x + \Delta x)v(x + \Delta x) - u(x)v(x) \\ = u(x + \Delta x)v(x + \Delta x) - u(x)v(x + \Delta x) + u(x)v(x + \Delta x) - u(x)v(x) \\ = v(x + \Delta x)[u(x + \Delta x) - u(x)] + u(x)[v(x + \Delta x) - v(x)]$

$\lim_{\Delta x \to 0} \frac{\Delta(uv)}{\Delta x} \\ = \lim_{\Delta x \to 0} \frac{v(x + \Delta x)[u(x + \Delta x) - u(x)] + u(x)[v(x + \Delta x) - v(x)]}{\Delta x} \\ = \lim_{\Delta x \to 0} v(x + \Delta x)\lim_{\Delta x \to 0} \frac{u(x + \Delta x) - u(x)}{\Delta x} + \lim_{\Delta x \to 0}u(x)\lim_{\Delta x \to 0}\frac{v(x+\Delta x) - v(x)}{\Delta x} \\ = u' \cdot v + u \cdot v'$

The last step uses the continuity of the function $v$, and it can be derived from that the function $v$ is differentiable.

Quotient Rule: $(\frac{u}{v})' = \frac{u' \cdot v - u \cdot v'}{v^2}$.

Proof:

$\Delta(\frac{u}{v}) \\ = \frac{u(x + \Delta x)}{v(x + \Delta x)} - \frac{u(x)}{v(x)} \\ = \frac{u(x + \Delta x)v(x) - u(x)v(x + \Delta x)}{v(x + \Delta x)v(x)} \\ = \frac{u(x + \Delta x)v(x) - u(x)v(x) - u(x)v(x + \Delta x) + u(x)v(x)}{v(x + \Delta x)v(x)} \\ = \frac{\Delta u \cdot v(x) - u(x) \cdot \Delta v}{v(x + \Delta x)v(x)}$

$\lim_{\Delta x \to 0}\frac{\Delta(\frac{u}{v})}{\Delta x} \\ = \lim_{\Delta x \to 0}\frac{\frac{\Delta u \cdot v(x) - u(x) \cdot \Delta v}{v(x + \Delta x)v(x)}}{\Delta x} \\ = \frac{\lim_{\Delta x \to 0}\frac{\Delta u}{\Delta x}v(x) - \lim_{\Delta x \to 0}u(x)\frac{\Delta v}{\Delta x}}{\lim_{\Delta x \to 0}v(x + \Delta x)v(x)} \\ = \frac{u'(x)v(x) - u(x)v'(x)}{v(x)^2}$

The last step uses the continuity of the function $v$, and it can be derived from that the function $v$ is differentiable.

Example 1: calculate the derivative of the function $y = \frac{1}{x}$.

We can view the function as $y = \frac{u(x)}{v(x)}$ where $u(x) = 1$, and $v(x) = x$.

According to the quotient rule,

$\frac{dy}{dx} = (\frac{u(x)}{v(x)})' \\ = \frac{u' \cdot v - u \cdot v'}{v^2} \\ = \frac{0 \cdot x - 1 \cdot 1}{x^2} \\ = -\frac{1}{x^2}$

Example 2: calculate the derivative of the function $y = \frac{1}{x^n}$.

We can view the function as $y = \frac{u(x)}{v(x)}$ where $u(x) = 1$, and $v(x) = x^n$.

According to the quotient rule,

$\frac{dy}{dx} = (\frac{u(x)}{v(x)})' \\ = \frac{u' \cdot v - u \cdot v'}{v^2} \\ = \frac{0 \cdot x^n - 1 \cdot nx^{n - 1}}{x^{2n}} \\ = -nx^{-n - 1}$

The result conforms with the specific rule for the function $y = x^n, n=0,1,2,...$. Therefore, the specific rule also holds for negative $n$ values.

Composition Rule: a function $y = f(g(t))$ can be expressed as $y = f(x), x = g(t)$ by using a new variable name $x$.

Chain Rule: Differentiation of a composition is a product.

Proof: Suppose we have a function $y=f(g(t))$, and we can express it as $y=f(x),x=g(t)$.

$\lim_{\Delta t \to 0}\frac{\Delta y}{\Delta t} = \lim_{\Delta t \to 0}\frac{\Delta y}{\Delta x} \cdot \frac{\Delta x}{\Delta t} = \lim_{\Delta t \to 0}\frac{\Delta y}{\Delta x} \cdot \lim_{\Delta t \to 0}\frac{\Delta x}{\Delta t}$

Since $x=g(t)$ is differentiable, when $\Delta t \to 0$, $\Delta x \to 0$ holds.

Therefore, $\lim_{\Delta t \to 0}\frac{\Delta y}{\Delta x} = \frac{dy}{dx}$, $\lim_{\Delta t \to 0}\frac{\Delta x}{\Delta t} = \frac{dx}{dt}$.

Hence, $\frac{dy}{dt} = \frac{dy}{dx} \cdot \frac{dx}{dt}$.

Example 1: calculate the derivative of the function $y = \sin^{10}(t)$.

We can express the function as $x = \sin(t)$, $y = x^{10}$.

According to the chain rule,

$\frac{dy}{dt}=\frac{dy}{dx} \cdot \frac{dx}{dt} = 10x^9 \cdot \cos(t) = 10\sin^9(t)\cos(t)$.

Example 2: calculate the derivative of the function $y = \sin(10t)$.

We can express the function as $x = 10t$, $y = \sin(x)$.

According to the chain rule,

$\frac{dy}{dt} = \frac{dy}{dx} \cdot \frac{dx}{dt} = \cos(x) \cdot 10 = 10\cos(10t)$.

Higher Derivatives: derivatives over derivative functions.

Example: $u(x)=\sin(x)$, $u'(x) = (u(x))' = \cos(x)$, $u''(x) = (u'(x))' = -\sin(x)$, $u'''(x) = (u''(x))' = -\cos(x)$, $u^4(x) = (u'''(x))' = \sin(x)$.

Anther notation: $u'(x) = \frac{d}{dx} u(x)$. If we view $\frac{d}{dx}$ as an operator that is applied to $u(x)$ and use $D$ to represent it, then we have

$u'(x) = \frac{d}{dx}u(x) = \frac{du}{dx} = Du$

$u''(x)=\frac{d}{dx} \frac{d}{dx} u(x) = (\frac{d}{dx})^2 u(x) = \frac{d^2}{d x^2} u(x) = \frac{d^2 u}{d x^2} = D^2 u$

$u'''(x) = \frac{d}{dx} \frac{d}{dx} \frac{d}{dx} u(x) = (\frac{d}{dx})^3 u(x) = \frac{d^3}{d x^3} u(x) = \frac{d^3 u}{d x^3} = D^3 u$

Example 1: calculate $D^n x^n$.

$D x^n = n x^{n-1}$

$D^2 x^n = n(n-1)x^{n -2}$

$D^3 x^n = n (n-1) (n-2) x^{n-3}$

...

$D^{n-1} x^n = n (n-1) (n-2) ... 3 \cdot 2 \cdot x$

$D^n x^n = n (n-1) (n-2) ... 2 \cdot 1 \cdot x^0 = n (n-1) (n-2) ... 3 \cdot 2 \cdot 1 = n!$

$D^{n+1} x^n = 0$