# Lecture 2: Limits

What is derivatives?
$\frac{\Delta y}{\Delta x}$ is the average rate of change.
When $\Delta x$ approaching 0, $\frac{\Delta y}{\Delta x} = \frac{dy}{dx}$ is the instantaneous rate of change.

Examples:

1. $q = charge$, $\frac{dq}{dt}=current$.
2. $s = distance$, $\frac{ds}{dt}=speed$.
3. $T = temperature$, $\frac{dT}{dx}=temperature gradient$.
4. Sensitivity of measurements. For example, in a simplified GPS model, the GPS satellite measures the location of a GPS device by measuring the distance $h$ between the satellite and the device and then based on the distance $h$ calculating the distance $l$ between the device and the base station. Therefore, the error rate $\frac{\Delta l}{\Delta h} \approx \frac{dl}{dh}$ is the sensitivity of the measurement. 

Notions:

1. left-hand limits = $\lim_{x \to x_0^-} f(x)$. $\lim_{x \to x_0^-}$ means $x \to x_0$ and $x < x_0$.
2. right-hand limits = $\lim_{x \to x_0^+} f(x)$. $\lim_{x \to x_0^+}$ means $x \to x_0$ and $x > x_0$.

Example:

$f(x) = \begin{cases}
   x + 1 & x > 0 \\
   -x + 2 & x < 0
\end{cases}$

$\lim_{x \to 0^+}f(x) = \lim_{x \to 0} (x + 1) = 1$ 

$\lim_{x \to 0^-} f(x) = \lim_{x \to 0} (-x + 2) = 2$

Notice that in calculating the left-hand limits and right-hand limits at $x_0 = 0$, we don't need $f(0)$.  

Definition:

$f$ is continuous at $x_0$ means $\lim_{x \to x_0} f(x) = f(x_0)$. It can be expanded into the following statements:

1. $\lim_{x \to x_0} f(x)$ exists, which means $\lim_{x \to x_0^-} f(x)$ exists, $\lim_{x \to x_0^+} f(x)$ exists, and $\lim_{x \to x_0^-} f(x) = \lim_{x \to x_0^+} f(x)$.
2. $f(x_0)$ is defined.
3. $\lim_{x \to x_0} f(x) = f(x_0)$.

Notice that $\lim_{x \to x_0} f(x)$ is completely independent from $f(x_0)$. $\lim_{x \to x_0} f(x)$ is evaluated by a procedure not involved with $f(x_0)$.

Discontinuity:

Jump discontinuity: left-hand limits and right-hand limits exist but they are not equal.

Removable discontinuity: left-hand limits and right-hand limits are equal, but the function value at that point is either undefined or not equal to the limits. Example: $y = \frac{\sin(x)}{x}$ at $x_0 = 0$, and $y = \frac{1 - \cos(x)}{x}$ at $x_0 = 0$ where both of these functions are undefined at $x_0 = 0$.

Infinite discontinuity: either or both of left-hand limits and right-hand limits go towards infinity. Example: $y = \frac{1}{x}$ at $x_0 = 0$, where both left-hand limits and right-hand limits go towards infinity.

Other (ugly) discontinuity: all kinds of other discontinuity. Example: $y=\sin(\frac{1}{x})$ at $x_0 = 0$, where left-hand limits and right-hand limits don't exist.

Theorem:

If $f$ is differentiable at $x_0$, then $f$ is continuous at $x_0$.

Proof:

As f is differentiable at $x_0$, we have

$f'(x_0) = \lim_{x \to x_0}\frac{f(x) - f(x_0)}{x - x_0} = c$

$\lim_{x \to x_0} \frac{f(x) - f(x_0)}{x - x_0}(x - x0) = c \times \lim_{x \to x_0} x - x_0 = 0$

$\lim_{x \to x_0} f(x) - f(x_0) = 0$

Therefore, $f$ is continuous at $x_0$.

TODO: does the production rule hold for limits?
