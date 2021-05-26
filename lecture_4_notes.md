# Lecture 4: Chain Rule

General rules for derivatives:

$(c \cdot u)' = c \cdot u'$

$(u + v)' = u' + v'$

Production Rule: $(u \cdot v)' = u' \cdot v + u \cdot  v'$.

Proof:

$\Delta(uv) \\ = u(x + \Delta x)v(x + \Delta x) - u(x)v(x) \\ = u(x + \Delta x)v(x + \Delta x) - u(x)v(x + \Delta x) + u(x)v(x + \Delta x) - u(x)v(x) \\ = v(x + \Delta x)[u(x + \Delta x) - u(x)] + u(x)[v(x + \Delta x) - v(x)]$

$\lim_{\Delta x \to 0} \frac{\Delta(uv)}{\Delta x} \\ = \lim_{\Delta x \to 0} \frac{v(x + \Delta x)[u(x + \Delta x) - u(x)] + u(x)[v(x + \Delta x) - v(x)]}{\Delta x} \\ = \lim_{\Delta x \to 0} v(x + \Delta x)\lim_{\Delta x \to 0} \frac{u(x + \Delta x) - u(x)}{\Delta x} + \lim_{\Delta x \to 0}u(x)\lim_{\Delta x \to 0}\frac{v(x+\Delta x) - v(x)}{\Delta x} \\ = u' \cdot v + u \cdot v'$

The last step uses the continuity of the function $v$, and it can be concluded from that the function $v$ is differentiable.

Quotient Rule: $(\frac{u}{v})' = \frac{u' \cdot v - u \cdot v'}{v^2}$.

Proof:

$\Delta(\frac{u}{v}) \\ = \frac{u(x + \Delta x)}{v(x + \Delta x)} - \frac{u(x)}{v(x)} \\ = \frac{u(x + \Delta x)v(x) - u(x)v(x + \Delta x)}{v(x + \Delta x)v(x)} \\ = \frac{u(x + \Delta x)v(x) - u(x)v(x) - u(x)v(x + \Delta x) + u(x)v(x)}{v(x + \Delta x)v(x)} \\ = \frac{\Delta u \cdot v(x) - u(x) \cdot \Delta v}{v(x + \Delta x)v(x)}$

$\lim_{\Delta x \to 0}\frac{\Delta(\frac{u}{v})}{\Delta x} \\ = \lim_{\Delta x \to 0}\frac{\frac{\Delta u \cdot v(x) - u(x) \cdot \Delta v}{v(x + \Delta x)v(x)}}{\Delta x} \\ = \frac{\lim_{\Delta x \to 0}\frac{\Delta u}{\Delta x}v(x) - \lim_{\Delta x \to 0}u(x)\frac{\Delta v}{\Delta x}}{\lim_{\Delta x \to 0}v(x + \Delta x)v(x)} \\ = \frac{u'(x)v(x) - u(x)v'(x)}{v(x)^2}$

The last step uses the continuity of the function $v$, and it can be concluded from that the function $v$ is differentiable.