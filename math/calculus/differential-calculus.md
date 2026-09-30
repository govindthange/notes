# Differential Calculus Formulas

## I. Limits and Standard Forms

* Definition of Limit: $\lim_{x \to a} f(x) = L$

* Indeterminate Forms: $\frac{0}{0}, \frac{\infty}{\infty}, 0 \cdot \infty, \infty - \infty, 0^0, 1^\infty, \infty^0$

* L'Hôpital's Rule: If $\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{0}{0}$ or $\frac{\infty}{\infty}$, then $\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}$

* Fundamental Trigonometric Limit: $\lim_{x \to 0} \frac{\sin x}{x} = 1$ (where $x$ is in radians)

* Fundamental Trigonometric Limit (Tan): $\lim_{x \to 0} \frac{\tan x}{x} = 1$

* Fundamental Algebraic Limit: $\lim_{x \to a} \frac{x^n - a^n}{x - a} = n a^{n-1}$

* Exponential Limit: $\lim_{x \to 0} \frac{e^x - 1}{x} = 1$

* Logarithmic Limit: $\lim_{x \to 0} \frac{\ln(1 + x)}{x} = 1$

* General Exponential Limit: $\lim_{x \to 0} \frac{a^x - 1}{x} = \ln a$ ($a > 0$)

* Standard Expansion ($e^x$): $e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \dots$

* Standard Expansion ($\ln(1+x)$): $\ln(1 + x) = x - \frac{x^2}{2} + \frac{x^3}{3} - \dots$ (|x| < 1)

* Standard Expansion ($\sin x$): $\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \dots$

* Standard Expansion ($\cos x$): $\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \dots$

## II. Continuity and Differentiability

* Condition for Continuity: A function $f(x)$ is continuous at $x = c$ if $\lim_{x \to c^-} f(x) = \lim_{x \to c^+} f(x) = f(c)$

* Condition for Differentiability: $f(x)$ is differentiable at $x = c$ if Left-Hand Derivative (LHD) equals Right-Hand Derivative (RHD): $\text{LHD} = \text{RHD} = f'(c)$

## III. Standard Derivatives

* Power Rule: $\frac{d}{dx}(x^n) = n x^{n-1}$

* Constant Rule: $\frac{d}{dx}(c) = 0$

* Exponential Rule ($e^x$): $\frac{d}{dx}(e^x) = e^x$

* General Exponential Rule: $\frac{d}{dx}(a^x) = a^x \ln a$

* Natural Logarithm Rule: $\frac{d}{dx}(\ln x) = \frac{1}{x}$

* General Logarithm Rule: $\frac{d}{dx}(\log_a x) = \frac{1}{x \ln a}$

* Sine Rule: $\frac{d}{dx}(\sin x) = \cos x$

* Cosine Rule: $\frac{d}{dx}(\cos x) = -\sin x$

* Tangent Rule: $\frac{d}{dx}(\tan x) = \sec^2 x$

* Cosecant Rule: $\frac{d}{dx}(\csc x) = -\csc x \cot x$

* Secant Rule: $\frac{d}{dx}(\sec x) = \sec x \tan x$

* Cotangent Rule: $\frac{d}{dx}(\cot x) = -\csc^2 x$

* Inverse Sine: $\frac{d}{dx}(\sin^{-1} x) = \frac{1}{\sqrt{1 - x^2}}$ (where $-1 < x < 1$)

* Inverse Cosine: $\frac{d}{dx}(\cos^{-1} x) = \frac{-1}{\sqrt{1 - x^2}}$ (where $-1 < x < 1$)

* Inverse Tangent: $\frac{d}{dx}(\tan^{-1} x) = \frac{1}{1 + x^2}$

* Inverse Cosecant: $\frac{d}{dx}(\csc^{-1} x) = \frac{-1}{|x|\sqrt{x^2 - 1}}$ (where $|x| > 1$)

* Inverse Secant: $\frac{d}{dx}(\sec^{-1} x) = \frac{1}{|x|\sqrt{x^2 - 1}}$ (where $|x| > 1$)

* Inverse Cotangent: $\frac{d}{dx}(\cot^{-1} x) = \frac{-1}{1 + x^2}$

## IV. Differentiation Rules

* Sum and Difference Rule: $\frac{d}{dx}[f(x) \pm g(x)] = f'(x) \pm g'(x)$

* Constant Multiple Rule: $\frac{d}{dx}[c \cdot f(x)] = c \cdot f'(x)$

* Product Rule: $\frac{d}{dx}[f(x)g(x)] = f'(x)g(x) + f(x)g'(x)$

* Quotient Rule: $\frac{d}{dx}\left[\frac{f(x)}{g(x)}\right] = \frac{f'(x)g(x) - f(x)g'(x)}{[g(x)]^2}$ (where $g(x) \neq 0$)

* Chain Rule: $\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)$

* Parametric Differentiation: If $x = f(t)$ and $y = g(t)$, then $\frac{dy}{dx} = \frac{dy/dt}{dx/dt} = \frac{g'(t)}{f'(t)}$

## V. Applications of Derivatives: Tangents and Normals

* Slope of Tangent: $m = \frac{dy}{dx}\Big|_{(x_1, y_1)}$

* Equation of Tangent Line: $y - y_1 = m(x - x_1)$

* Slope of Normal Line: $m_n = -\frac{1}{m} = -\frac{1}{dy/dx}\Big|_{(x_1, y_1)}$

* Equation of Normal Line: $y - y_1 = -\frac{1}{m}(x - x_1)$

* Angle Between Two Curves: $\tan \theta = \left| \frac{m_1 - m_2}{1 + m_1 m_2} \right|$

## VI. Monotonicity and Extrema

* Strictly Increasing Function: $f'(x) > 0$ for all $x$ in an interval

* Strictly Decreasing Function: $f'(x) < 0$ for all $x$ in an interval

* First Derivative Test for Extrema: If $f'(c) = 0$ and changes sign from positive to negative at $x = c$, $c$ is a local maximum. If negative to positive, $c$ is a local minimum.

* Second Derivative Test: If $f'(c) = 0$ and $f''(c) < 0$, $c$ is a local maximum. If $f''(c) > 0$, $c$ is a local minimum.

* Point of Inflection: A point where $f''(x) = 0$ or undefined and changes sign (concavity changes).

## VII. Mean Value Theorems

* Rolle's Theorem: If $f(x)$ is continuous on $[a, b]$, differentiable on $(a, b)$, and $f(a) = f(b)$, then there exists at least one $c \in (a, b)$ such that $f'(c) = 0$.

* Lagrange's Mean Value Theorem (LMVT): If $f(x)$ is continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists at least one $c \in (a, b)$ such that $f'(c) = \frac{f(b) - f(a)}{b - a}$.

* Cauchy's Mean Value Theorem: If $f(x)$ and $g(x)$ are continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists $c \in (a, b)$ such that $\frac{f'(c)}{g'(c)} = \frac{f(b) - f(a)}{g(b) - g(a)}$.