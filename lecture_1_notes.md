# Differentiation

Definition 1: $f'(x_0)$, the derivative of $f$ at $x_0$, is the slope of the tangent line to $y=f(x)$ at $(x_0, f(x_0))$.

Analytically, we need to figure out the expression of the tangent line, i.e. $y - y_0 = m \times (x - x_0)$. We already know $x_0$ and $y_0$, so the rest thing is to figure out the slope $m$.

From geometry we have the conclusion: the tangent line is equal to the limit of secant line $PQ$ as $Q \rightarrow P$ ($P$ is fixed). Therefore, we can calculate the slope of the tangent line as:

$m = \lim_{\Delta x \to 0} \frac{\Delta f}{\Delta x}$

$f'(x_0) = \lim_{\Delta x \to 0} \frac{f(x_0+\Delta x) - f(x_0)}{\Delta x}$

The above equation is the general formula to calculate the slope of the tangent line for any function $f(x)$ at any point $(x_0, f(x_0))$.

Example 1: calculate the derivative of the function $f(x)=\frac{1}{x}$.
Generally, $\frac{\Delta f}{\Delta x}=\frac{\frac{1}{x_0+\Delta x}-\frac{1}{x_0}}{\Delta x}=-\frac{1}{(x_0+\Delta x)x_0}$
Therefore, $f'(x_0)=\lim_{\Delta x \to 0} \frac{\Delta f}{\Delta x} = \lim_{\Delta x \to 0} -\frac{1}{(x_0+\Delta x)x_0}=-\frac{1}{x_0^2}$

Followup 1: find the areas of triangles enclosed by the axes and the tangent line to the function $f(x) = \frac{1}{x}$.
Suppose the tangent line passes the point $(x_0, y_0)$, that is $(x_0, \frac{1}{x_0})$. Based on the above result, we know that the equation of the tangent line is $y - y_0 = -\frac{1}{x_0^2}(x - x_0)$.
The next step is to find the coordinates of the x-interception and y-interception.
For the x-interception, it is the intersection of the tangent line and the line $y=0$. Therefore, we have

$0-y_0=-\frac{1}{x_0^2}(x-x_0)$
$0-\frac{1}{x_0}=-\frac{1}{x_0^2}(x-x_0)$
$x=2x_0$
So the x-interception is $(2x_0, 0)$
For the y-interception, we will use symmetry to calculate it. The function $y=\frac{1}{x}$ can also be described as $f(y)=\frac{1}{y}$. So the slope of the tangent line is $-\frac{1}{y_0^2}$, and the equation of the tangent line is $x-x_0 = \frac{1}{y_0^2}(y-y_0)$. Therefore the intersection of the tangent line and the line $x = 0$ is $y=2y_0$, i.e. $(0, 2y_0)$.
Therefore, the area is $\frac{1}{2} \times 2x_0 \times 2y_0 = 2$. Since $(x_0, y_0)$ is a random point on the function, the areas of the described triangles are always 2.

More notations:

1. $\Delta y = \Delta f$
2. $f'=\frac{df}{dx}=\frac{dy}{dx}=\frac{d}{dx}f=\frac{d}{dx}y$

Example 2: calculate the derivative of the function $f(x)=x^n, n =1,2,3,...$

$\frac{\Delta f}{\Delta x}=\frac{(x+\Delta x)^n - x^n}{\Delta x}$ (Here $x$ is the previous $x_0$, so $x$ is actually fixed, and $\Delta x$ is moving to $0$)
According to binomial theorem, 
$(x+\Delta x)^n = (x+\Delta x)(x+\Delta x)...(x+\Delta x) = x^n + n x^{n-1} \Delta x + O((\Delta x)^2)$
Here $O((\Delta x)^2)$ means these are terms with $(\Delta x)^2$, $(\Delta x)^3$, ...
Therefore,
$\frac{\Delta f}{\Delta x} = \frac{1}{\Delta x}(x^n + n x^{n-1} \Delta x + O((\Delta x)^2) - x^n) = \frac{1}{\Delta x}(n x^{n-1} \Delta x + O((\Delta x)^2)) = n x^{n-1} + O(\Delta x)$

$f'(x) = \lim_{\Delta x \to 0} \frac{\Delta f}{\Delta x} = \lim_{\Delta x \to 0} n x^{n-1} + O(\Delta x) = n x^{n-1}$

The above formula extends to polynomials.