# Problem Set: Differentiation

1F-3 Find $\frac{dy}{dx}$ for $y = x^{\frac{1}{n}}$ by implicit differentiation.

Solution:

$y = x^{\frac{1}{n}}$

$y^n =x$

We apply $\frac{d}{dx}$ to both sides and the equation still holds.

$n \cdot y^{n-1} \cdot \frac{dy}{dx} = 1$

$\frac{dy}{dx} = \frac{1}{n \cdot y^{n-1}}$

$\frac{dy}{dx} = \frac{1}{n} \cdot (x^{\frac{1}{n}})^{1-n}$

$\frac{dy}{dx} = \frac{1}{n} \cdot x^{\frac{1}{n}-1}$

1F-5 Find all points of the curve(s) $\sin x + \sin y = \frac{1}{2}$ with horizontal tangent lines. (This is a collection of curves with a periodic, repeated pattern because the equation is unchanged under the transformations $y \to y + 2\pi$ and $x \to x + 2\pi$.)

Solution:

Horizontal tangent lines mean the slope of the graph at those points is 0. Therefore, we need to calculate their derivatives.

$\sin x + \sin y = \frac{1}{2}$

We apply $\frac{d}{dx}$ to both sides and the equation still holds.

$\cos x + \cos y \cdot \frac{dy}{dx} = 0$

$\frac{dy}{dx} = -\frac{\cos x}{\cos y}$

Combined with $\frac{dy}{dx} = 0$, we get

$-\frac{\cos x}{\cos y} = 0$

That requires two conditions:

1. $\cos x = 0$, which means $x = \pm \frac{\pi}{2} + 2n\pi, n=0, \pm1, \pm2, ...$
2. $\cos y \ne 0$. At the above $x$ values, $\cos x = 0$, then $\sin x = 1$, and then $\sin y = \frac{1}{2} - \sin x = -\frac{1}{2}$, then we know $\cos y = \pm \sqrt{1 - \sin^2 y} \ne 0$.

Therefore, the points are $x = \pm \frac{\pi}{2} + 2n\pi, n=0, \pm1, \pm2, ...$

1F-8 Evaluate the derivative by implicit differentiation. Assume all letters represent constants, except for the independent and dependent variables occurring in the derivative.

a) $V = \frac{1}{3}\pi r^2h$, $\frac{dr}{dh}=?$

b) $PV^c = nRT$, $\frac{dP}{dV} = ?$

c) $c^2 = a^2 + b^2 - 2ab\cos \theta$, $\frac{da}{db} = ?$

Solution:

a) We apply $\frac{d}{dh}$ to both sides of the expression, then we get

$0 = \frac{1}{3}\pi(2r\frac{dr}{dh}h + r^2)$

$\frac{dr}{dh} = \frac{r}{2h}$

According to the original expression,

$V = \frac{1}{3}\pi r^2h$

$r^2 = \frac{3V}{\pi h}$

$r = \pm \sqrt{\frac{3V}{\pi h}}$

$\frac{dr}{dh} = \pm \frac{\sqrt{\frac{3V}{\pi h}}}{2h}$

$\frac{dr}{dh} = \pm \sqrt{\frac{3V}{4\pi h^3}}$

b) We apply $\frac{d}{dV}$ to both sides of the expression, then we get

$V^c \frac{dP}{dV} + PcV^{c-1} = 0$

$\frac{dP}{dV} = \frac{cP}{V}$

According to the original expression,

$PV^c = nRT$

$P = \frac{nRT}{V^c}$

$\frac{dP}{dV} = \frac{ncRT}{V^{c+1}}$

c) We apply $\frac{d}{db}$ to both sides of the expression, then we get

$0 = 2a \frac{da}{db} + 2b - 2\cos \theta (b\frac{da}{db}+a)$

$\frac{da}{db} = \frac{2a\cos\theta - 2b}{2a - 2b\cos\theta} = \frac{a \cos \theta - b}{a - b \cos \theta}$

1G-1 Calculate $y''$ for the following functions.

a) $3x^2+2x+4\sqrt{x}$

b) $\frac{x}{x+5}$

c) $\frac{-5}{x+5}$

d) $\frac{x^2+5x}{x+5}$

Solution:

a) $y' = \frac{d}{dx}(3x^2+2x+4\sqrt{x}) = 6x + 2 + \frac{2}{\sqrt{x}}$

$y'' = \frac{d}{dx}(6x+2+\frac{2}{\sqrt{x}}) = 6 - \frac{1}{\sqrt{x^3}}$

b) $y'=\frac{d}{dx}(\frac{x}{x+5}) = \frac{d}{dx}(1 + \frac{-5}{x+5}) = \frac{5}{(x+5)^2}$

$y''=\frac{d}{dx}(\frac{5}{(x+5)^2}) = -\frac{10}{(x+5)^3}$

c) $y'=\frac{d}{dx}(\frac{-5}{x+5}) = \frac{5}{(x+5)^2}$

$y''=\frac{d}{dx}(\frac{5}{(x+5)^2}) = -\frac{10}{(x+5)^3}$

d) $y' = \frac{d}{dx}(\frac{x^2+5x}{x+5}) = \frac{d}{dx}x = 1$

$y'' = \frac{d}{dx}1 = 0$

1G-2 Find all functions $f(x)$ whose third derivative $f'''(x)$ is identically zero. ("Identically" is math jargon for "always" or "for every value of x".)

Solution: According to the problem description, we have

$f'''(x) = 0$ always holds.

Therefore, we can deduce that

$f''(x) = a$, where $a$ is a constant.

Hence, $f'(x) = ax+b$, where $a$ and $b$ are constants. So

$f(x) = ax^2+bx+c$, where $a$, $b$, and $c$ are constants.

1G-3 Calculate $y''$ using implicit differentiation and simplify as much as possible.

$x^2a^2+y^2b^2=1$

Solution: Apply $\frac{d}{dx}$ to both sides of the expression, then we get

$2a^2x + 2b^2y\cdot\frac{dy}{dx} = 0$

$\frac{dy}{dx}=-\frac{a^2x}{b^2y}$

Apply $\frac{d}{dx}$ to both sides of the above expression, then we get

$\frac{d^2y}{dx^2}= -\frac{a^2\cdot b^2y - a^2x \cdot b^2\frac{dy}{dx}}{b^4y^2}$

Substitute $\frac{dy}{dx}$ with the corresponding expression, then we get

$\frac{d^2y}{dx^2} = \frac{a^2b^2(x\cdot \frac{-a^2x}{b^2y} - y)}{b^4y^2} = -\frac{a^2b^2(a^2x^2+b^2y^2)}{b^4y^2} = -\frac{a^2b^2}{b^4y^2} = -\frac{a^2}{b^2y^2} = \frac{a^2}{a^2x^2 - 1}$

1G-4 Find the formula for the nth derivative $y^{(n)}$ of $y = \frac{1}{x+1}$.

Solution:

$y' = \frac{d}{dx}(\frac{1}{x+1}) = \frac{0 \cdot (x+1) - 1 \cdot 1}{(x+1)^2} = -\frac{1}{(x+1)^2}$

$y'' = \frac{d}{dx}(-\frac{1}{(x+1)^2}) = -\frac{0 \cdot (x+1)^2 - 1 \cdot 2(x+1)}{(x+1)^4} = \frac{2}{(x+1)^3}$

$y''' = \frac{d}{dx}(\frac{2}{(x+1)^3}) = \frac{0 \cdot (x+1)^3 - 2 \cdot 3(x+1)^2}{(x+1)^6} = -\frac{6}{(x+1)^4}$

We can see that $y^{(n)} = (-1)^n \cdot \frac{n!}{(x+1)^{n+1}}$ holds for $n = 1, 2, 3$

Suppose $y^{(n-1)} = (-1)^{n-1} \cdot \frac{(n-1)!}{(x+1)^n}$, then we can get

$y^{(n)} = \frac{d}{dx}y^{(n-1)} = \frac{d}{dx}((-1)^{n-1} \cdot \frac{(n-1)!}{(x+1)^n}) = (-1)^{n-1} \cdot \frac{0 \cdot (x+1)^n - (n-1)! \cdot n(x+1)^{n-1}}{(x+1)^{2n}} = (-1)^n \frac{n!}{(x+1)^{n+1}}$

Therefore, $y^{(n)} = (-1)^n \cdot \frac{n!}{(x+1)^{n+1}}$ holds for all non-negative integers.

1G-5 Let $y = u(x)v(x)$.

a) Find $y'$, $y''$, and $y'''$.

Solution:

$y' = \frac{d}{dx}(u(x)v(x)) = u'\cdot v + u \cdot v'$

$y'' = \frac{d}{dx}y' = \frac{d}{dx}(u' \cdot v + u \cdot v') = u'' \cdot v + u' \cdot v' + u' \cdot v' + u \cdot v'' = u'' \cdot v + 2u' \cdot v' + u \cdot v''$

$y''' = \frac{d}{dx}y'' = \frac{d}{dx}(u'' \cdot v + 2u' \cdot v' + u \cdot v'') = u''' \cdot v + u'' \cdot v' + 2u'' \cdot v' + 2u' \cdot v'' + u' \cdot v'' + u \cdot v''' = u''' \cdot v + 3 u'' \cdot v' + 3 u' \cdot v'' + u \cdot v'''$

b) The general formula for $y^{(n)}$, the n-th derivative, is called Leibniz' formula: it uses the same coefficients as the binomial theorem, and looks like

$y^{(n)} = u^{(n)}v+\binom{n}{1}u^{(n-1)}v^{(1)} + \binom{n}{2}u^{(n-2)}v^{(2)}+...+uv^{(n)}$

Use this to check your answers in part (a), and use it to calculate $y^{(p+q)}$, if $y = x^p(1+x)^q$.

Solution:

$y = u(x)v(x) = x^p(1+x)^q$

$u(x)=x^p$

$u^{(n)} = \frac{p!}{(p-n)!}x^{p-n}, n = 1, 2, 3, ..., p$

$u^{(n)} = 0, n = p+1, p+2, ...$

$v(x) = (1+x)^q$

$v^{(n)} = \frac{q!}{(q-n)!}(1+x)^{q-n}, n = 1, 2, 3, ..., q$

$v^{(n)} = 0, n = q+1, q+2, ...$

Therefore,

$y^{(p+q)} = u^{(p+q)}v + \binom{p+q}{1}u^{(p+q-1)}v{(1)} + ... + \binom{p+q}{p}u^{(p)}v^{(q)} + ... + \binom{p+q}{p+q-1}u^{(1)}v^{(p+q-1)} + \binom{p+q}{p+q}uv^{(p+q)}$

The factors before $\binom{p+q}{p}u^{(p)}v^{(q)}$ are all 0 because they contain $u^{(n)}$ where $n > p$. The factors after $\binom{p+q}{p}u^{(p)}v^{(q)}$ are all 0 because they contain $v^{(n)}$ where $n > q$.

Therefore,

$y^{(p+q)} = \binom{p+q}{p}u^{(p)}v^{(q)} = \binom{p+q}{p} \cdot p! \cdot q!$

1H-1 The half-life $\lambda$ of a radioactive substance decaying according to the law $y=y_0e^{-kt}$ is defined to be the time it takes the amount to decrease to $\frac{1}{2}$ of the initial amount $y_0$.

a) Express the half-life $\lambda$ in terms of $k$. (Do this from scratch).

Solution:

According to the problem description, $\lambda$ is the value of $t$ when $y = y_0e^{-kt} = \frac{1}{2}y_0$.

$e^{-k\lambda} = \frac{1}{2}$

$-k\lambda = \ln(\frac{1}{2})$

$\lambda = - \frac{\ln(\frac{1}{2})}{k}$

b) Show using your expression for $\lambda$ that if at time $t_1$ the amount is $y_1$, then at time $t_1 + \lambda$ it will be $\frac{y_1}{2}$, no matter what $t_1$ is.

Solution:

At time $t_1$ the amount is $y_1$, so we get

$y_1 = y_0e^{-kt_1}$

At time $t_1 + \lambda$, the amount

$y = y_0e^{-k(t_1 + \lambda)} = y_0e^{-kt_1}e^{-k\lambda} = \frac{1}{2}y_0e^{-kt_1} = \frac{1}{2}y_1$

Since we just randomly pick the $t_1$, we know that at time $t_1 + \lambda$, the amount will be $\frac{y_1}{2}$, no matter what $t_1$ is.

1H-2 If a solution containing a heavy concentration of hydrogen ions (i.e., a strong acid) is diluted with an equal volume of water, by approximately how much is its pH changed? (Express $(pH)_{diluted}$ in terms of $(pH)_{original}$.

Solution: According to the problem description, after diluted with an equal volume of water, the concentration of hydrogen ions becomes half as before, i.e.

$[H^+]_{diluted} = \frac{1}{2}[H^+]_{original}$

The pH value is calculated by the formula $pH = -\lg[H^+]$. Therefore,

$(pH)_{diluted} = -\lg[H^+]_{diluted} = -\lg(\frac{1}{2}\cdot[H^+]_{original}) = -\lg(\frac{1}{2}) + (-\lg[H^+]_{original}) = -\lg(\frac{1}{2}) + (pH)_{original}$

$-\lg(\frac{1}{2}) \approx 0.3$

Hence, the pH value goes up by approximately 0.3.