# Lecture 3: Derivatives

There are two kinds of derivative formulas:

1. Specific formulas: derivative formulas for a specific function, like $y = x^n, n=1,2,3,...$
2. General formulas: derivative formulas for expressions, like $(u + v)'= u' + v'$.

Derivative formula for the function $\sin x$:

$\frac{d}{dx}\sin x = \lim_{\Delta x \to 0}\frac{\sin(x+\Delta x) - \sin(x)}{\Delta x} \\ = \lim_{\Delta x \to 0} \frac{\sin x\cos \Delta x + \cos x \sin \Delta x - \sin x}{\Delta x} \\ = \lim_{\Delta x \to 0} \sin x (\frac{1 - \cos \Delta x}{\Delta x}) + \cos x (\frac{\sin \Delta x}{\Delta x})$

Since $\lim_{\Delta x \to 0} \frac{1 - \cos \Delta x}{\Delta x} = 0$, $\lim_{\Delta x \to 0} \frac{\sin \Delta x}{\Delta x} = 1$, then

$\frac{d}{dx}\sin x = \lim_{\Delta x \to 0} \sin x (\frac{1 - \cos \Delta x}{\Delta x}) + \cos x (\frac{\sin \Delta x}{\Delta x}) = \cos x$

Derivative formula for the function $\cos x$:

$\frac{d}{dx} \cos x = \lim_{\Delta x \to 0} \frac{\cos(x + \Delta x) - \cos x}{\Delta x} \\ = \lim_{\Delta x \to 0} \frac{\cos x \cos \Delta x - \sin x \sin \Delta x - \cos x}{\Delta x} \\ = \lim_{\Delta x \to 0} \cos x (\frac{1-\cos \Delta x}{\Delta x}) - \sin x (\frac{\sin \Delta x}{\Delta x})$

Since $\lim_{\Delta x \to 0} \frac{1 - \cos \Delta x}{\Delta x} = 0$, $\lim_{\Delta x \to 0} \frac{\sin \Delta x}{\Delta x} = 1$, then

$\frac{d}{dx} \cos x = \lim_{\Delta x \to 0} \cos x (\frac{1-\cos \Delta x}{\Delta x}) - \sin x (\frac{\sin \Delta x}{\Delta x}) = - \sin x$

Notice:

$\frac{d}{dx} \cos x |_{x = 0} = \lim_{\Delta x \to 0} \frac{\cos \Delta x - \cos 0}{\Delta x} = \lim_{\Delta x \to 0} \frac{\cos \Delta x - 1}{\Delta x}$

$\frac{d}{dx} \sin x |_{x = 0} = \lim_{\Delta x \to 0} \frac{\sin \Delta x - \sin 0}{\Delta x} = \lim_{\Delta x \to 0} \frac{\sin \Delta x}{\Delta x}$

We can observe that: derivatives of sine and cosine functions at $x = 0$ give all values of derivatives of sine and cosine functions.

Proof of $\lim_{\Delta x \to 0} \frac{\sin \Delta x}{\Delta x} = 1$:

We'll prove it from the geometric point of view. In geometry, we'll change the $\Delta x$ to $\Delta \theta$. In a unit circle, the $\sin \Delta \theta$ is the edge length, and the $\Delta \theta$ is the arc length, and $\frac{\sin \Delta \theta}{\Delta \theta}$ is the ratio of the edge length to the arc length. When the $\Delta \theta$ becomes closer to 0 radians, the arc becomes more like straight lines, therefore $\lim_{\Delta \theta \to 0} \frac{\sin \Delta \theta}{\Delta \theta} = 1$.

Principle: short pieces of curves are nearly straight.

Proof of $\lim_{\Delta x \to 0} \frac{1 - \cos \Delta x}{\Delta x} = 0$:

We'll prove it from the geometric point of view. In geometry, we'll change the $\Delta x$ to $\Delta \theta$. In a unit circle, the $\cos \Delta \theta$ is the cast edge length, so the $1 - \cos \Delta \theta$ is the length of the remainder of the cast edge, and the $\Delta \theta$ is the arc length. Therefore, $\frac{1 - \cos \Delta \theta}{\Delta \theta}$ is the ratio of the length of the remainder of the cast edge to the arc length. When the $\Delta \theta$ becomes closer to 0 radians, the edge and the arc becomes more and more alike, so the remainder shrinks to smaller and smaller. The remainder becomes smaller much quicker than the arc, therefore $\lim_{\Delta \theta \to 0} \frac{1- \cos \Delta \theta}{\Delta \theta} = 0$.

Geometric proof of $\frac{d}{d \theta}\sin \theta = \cos \theta$ for all $\theta$: