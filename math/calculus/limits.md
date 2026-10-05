# Limits, Continuity, and Differentiability Formulas

## I. Basic Limit Properties and Algebra of Limits

* Limit of a Constant: $\lim_{x \to a} c = c$

* Limit of Identity Function: $\lim_{x \to a} x = a$

* Sum Rule: $\lim_{x \to a} [f(x) \pm g(x)] = \lim_{x \to a} f(x) \pm \lim_{x \to a} g(x)$

* Difference Rule: $\lim_{x \to a} [f(x) - g(x)] = \lim_{x \to a} f(x) - \lim_{x \to a} g(x)$

* Product Rule: $\lim_{x \to a} [f(x) \cdot g(x)] = \left(\lim_{x \to a} f(x)\right) \cdot \left(\lim_{x \to a} g(x)\right)$

* Quotient Rule: $\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{\lim_{x \to a} f(x)}{\lim_{x \to a} g(x)}$ (provided $\lim_{x \to a} g(x) \neq 0$)

* Constant Multiple Rule: $\lim_{x \to a} [c \cdot f(x)] = c \cdot \lim_{x \to a} f(x)$

* Power Rule: $\lim_{x \to a} [f(x)]^{n} = \left(\lim_{x \to a} f(x)\right)^n$

* Root Rule: $\lim_{x \to a} \sqrt[n]{f(x)} = \sqrt[n]{\lim_{x \to a} f(x)}$

## II. Standard Limits and Indeterminate Forms

* Definition of Limit: $\lim_{x \to a} f(x) = L$ implies $\lim_{x \to a^-} f(x) = \lim_{x \to a^+} f(x) = L$

* Indeterminate Forms: $\frac{0}{0}, \frac{\infty}{\infty}, 0 \cdot \infty, \infty - \infty, 0^0, 1^\infty, \infty^0$

* L'Hôpital's Rule: If $\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{0}{0}$ or $\frac{\infty}{\infty}$, then $\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}$

* Fundamental Trigonometric Limit 1: $\lim_{x \to 0} \frac{\sin x}{x} = 1$ (where $x$ is in radians)

* Fundamental Trigonometric Limit 2: $\lim_{x \to 0} \frac{\tan x}{x} = 1$

* Fundamental Trigonometric Limit 3: $\lim_{x \to 0} \frac{\sin^{-1} x}{x} = 1$

* Fundamental Trigonometric Limit 4: $\lim_{x \to 0} \frac{\tan^{-1} x}{x} = 1$

* Cosine Limit Form: $\lim_{x \to 0} \frac{1 - \cos x}{x^2} = \frac{1}{2}$

* Fundamental Algebraic Limit: $\lim_{x \to a} \frac{x^n - a^n}{x - a} = n a^{n-1}$

* Exponential Limit: $\lim_{x \to 0} \frac{e^x - 1}{x} = 1$

* Logarithmic Limit: $\lim_{x \to 0} \frac{\ln(1 + x)}{x} = 1$

* General Exponential Limit: $\lim_{x \to 0} \frac{a^x - 1}{x} = \ln a$ ($a > 0$)

## III. Exponential and Power Limits (One-Infinity Forms)

* Standard Form 1: $\lim_{x \to 0} (1 + x)^{\frac{1}{x}} = e$

* Standard Form 2: $\lim_{x \to \infty} \left(1 + \frac{1}{x}\right)^x = e$

* General Form 1: $\lim_{x \to 0} (1 + kx)^{\frac{1}{x}} = e^k$

* General Form 2: $\lim_{x \to \infty} \left(1 + \frac{k}{x}\right)^x = e^k$

* Functional Form: If $\lim_{x \to a} f(x) = 1$ and $\lim_{x \to a} g(x) = \infty$, then $\lim_{x \to a} [f(x)]^{g(x)} = e^{\lim_{x \to a} [f(x) - 1]g(x)}$

## IV. Continuity of Functions

* Continuity at a Point: A function $f(x)$ is continuous at $x = c$ if:
  1. $f(c)$ is defined
  2. $\lim_{x \to c} f(x)$ exists
  3. $\lim_{x \to c} f(x) = f(c)$ i.e., $\lim_{x \to c^-} f(x) = \lim_{x \to c^+} f(x) = f(c)$

* Continuity on an Open Interval $(a, b)$: $f(x)$ is continuous at every point in the interval.

* Continuity on a Closed Interval $[a, b]$: $f(x)$ is continuous on $(a, b)$, right-continuous at $x = a$ ($\lim_{x \to a^+} f(x) = f(a)$), and left-continuous at $x = b$ ($\lim_{x \to b^-} f(x) = f(b)$).

* Intermediate Value Theorem (IVT): If $f(x)$ is continuous on $[a, b]$ and $u$ is any number between $f(a)$ and $f(b)$, then there exists at least one $c \in (a, b)$ such that $f(c) = u$.

## V. Algebra and Properties of Continuous Functions

* Sum/Difference of Continuous Functions: If $f$ and $g$ are continuous at $x = c$, then $f \pm g$ is continuous at $x = c$.

* Product of Continuous Functions: If $f$ and $g$ are continuous at $x = c$, then $f \cdot g$ is continuous at $x = c$.

* Quotient of Continuous Functions: If $f$ and $g$ are continuous at $x = c$ and $g(c) \neq 0$, then $\frac{f}{g}$ is continuous at $x = c$.

* Composite Function Continuity: If $g$ is continuous at $c$ and $f$ is continuous at $g(c)$, then the composite function $(f \circ g)(x) = f(g(x))$ is continuous at $c$.

## VI. Continuity of Standard Functions

* Polynomial Functions: Continuous everywhere ($\mathbb{R}$).

* Rational Functions: Continuous at all points in their domain (where denominator $\neq 0$).

* Trigonometric Functions ($\sin x, \cos x$): Continuous everywhere on $\mathbb{R}$.

* Other Trig Functions ($\tan x, \sec x, \csc x, \cot x$): Continuous on their respective domains.

* Inverse Trigonometric Functions: Continuous on their respective domains.

* Exponential Functions ($a^x$): Continuous everywhere for $a > 0$.

* Logarithmic Functions ($\log_a x$): Continuous everywhere on their domain $(0, \infty)$.

## VII. Differentiability and Continuity Relationship

* Differentiability Implies Continuity: If a function $f(x)$ is differentiable at $x = c$, then it is guaranteed to be continuous at $x = c$.

* Converse is Not True: Continuity does not imply differentiability (e.g., $f(x) = |x|$ is continuous at $x=0$ but not differentiable there).

* Condition for Differentiability at a Point: $f(x)$ is differentiable at $x = c$ if Left-Hand Derivative (LHD) equals Right-Hand Derivative (RHD) and both are finite:
  $$\text{LHD} = \lim_{h \to 0^+} \frac{f(c - h) - f(c)}{-h} = \text{RHD} = \lim_{h \to 0^+} \frac{f(c + h) - f(c)}{h} = f'(c)$$