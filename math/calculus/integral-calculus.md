# 📐 Integral Calculus Formulas & Identities

## I. Standard Basic Integrals

* Power Rule: $\int x^n \, dx = \frac{x^{n+1}}{n+1} + C$ (where $n \neq -1$)

* Reciprocal Rule: $\int \frac{1}{x} \, dx = \ln|x| + C$

* Exponential (Base e): $\int e^x \, dx = e^x + C$

* Exponential (General): $\int a^x \, dx = \frac{a^x}{\ln a} + C$ (where $a > 0, a \neq 1$)

* Natural Logarithm Integral: $\int \ln x \, dx = x \ln x - x + C$

## II. Trigonometric Integrals

* Sine Integral: $\int \sin x \, dx = -\cos x + C$

* Cosine Integral: $\int \cos x \, dx = \sin x + C$

* Secant Squared: $\int \sec^2 x \, dx = \tan x + C$

* Cosecant Squared: $\int \csc^2 x \, dx = -\cot x + C$

* Secant Tangent: $\int \sec x \tan x \, dx = \sec x + C$

* Cosecant Cotangent: $\int \csc x \cot x \, dx = -\csc x + C$

* Tangent Integral: $\int \tan x \, dx = \ln|\sec x| + C = -\ln|\cos x| + C$

* Cotangent Integral: $\int \cot x \, dx = \ln|\sin x| + C$

* Secant Integral: $\int \sec x \, dx = \ln|\sec x + \tan x| + C = \ln\left|\tan\left(\frac{x}{2} + \frac{\pi}{4}\right)\right| + C$

* Cosecant Integral: $\int \csc x \, dx = \ln|\csc x - \cot x| + C = \ln\left|\tan\left(\frac{x}{2}\right)\right| + C$

## III. Inverse Trigonometric Integrals

* Arcsine Form: $\int \frac{1}{\sqrt{a^2 - x^2}} \, dx = \sin^{-1}\left(\frac{x}{a}\right) + C$

* Arctangent Form: $\int \frac{1}{a^2 + x^2} \, dx = \frac{1}{a} \tan^{-1}\left(\frac{x}{a}\right) + C$

* Arcsecant Form: $\int \frac{1}{x\sqrt{x^2 - a^2}} \, dx = \frac{1}{a} \sec^{-1}\left(\frac{x}{a}\right) + C$

* Arcsine Logarithmic Form: $\int \frac{1}{\sqrt{x^2 \pm a^2}} \, dx = \ln\left|x + \sqrt{x^2 \pm a^2}\right| + C$

* Inverse Tangent Logarithmic Form: $\int \frac{1}{a^2 - x^2} \, dx = \frac{1}{2a} \ln\left|\frac{a + x}{a - x}\right| + C$

* Inverse Tangent Alternative: $\int \frac{1}{x^2 - a^2} \, dx = \frac{1}{2a} \ln\left|\frac{x - a}{x + a}\right| + C$

## IV. Standard Special Integrals (Square Roots in Numerator)

* Root of Sum of Squares: $\int \sqrt{a^2 + x^2} \, dx = \frac{x}{2}\sqrt{a^2 + x^2} + \frac{a^2}{2}\ln\left|x + \sqrt{a^2 + x^2}\right| + C$

* Root of Difference of Squares (x first): $\int \sqrt{x^2 - a^2} \, dx = \frac{x}{2}\sqrt{x^2 - a^2} - \frac{a^2}{2}\ln\left|x + \sqrt{x^2 - a^2}\right| + C$

* Root of Difference of Squares (a first): $\int \sqrt{a^2 - x^2} \, dx = \frac{x}{2}\sqrt{a^2 - x^2} + \frac{a^2}{2}\sin^{-1}\left(\frac{x}{a}\right) + C$

## V. Advanced Standard Forms (JEE/MIT Favorites)

* Linear over Quadratic: $\int \frac{px + q}{ax^2 + bx + c} \, dx = \frac{p}{2a}\ln|ax^2 + bx + c| + \left(q - \frac{pb}{2a}\right) \int \frac{dx}{ax^2 + bx + c}$

* Linear over Square Root Quadratic: $\int \frac{px + q}{\sqrt{ax^2 + bx + c}} \, dx = \frac{p}{a}\sqrt{ax^2 + bx + c} + \left(q - \frac{pb}{2a}\right) \int \frac{dx}{\sqrt{ax^2 + bx + c}}$

* Exponential with Trig Product: $\int e^{ax} \sin(bx) \, dx = \frac{e^{ax}}{a^2 + b^2}(a \sin(bx) - b \cos(bx)) + C$

* Exponential with Cosine Product: $\int e^{ax} \cos(bx) \, dx = \frac{e^{ax}}{a^2 + b^2}(a \cos(bx) + b \sin(bx)) + C$

* Euler Substitution (Rationalizing $\sqrt{ax^2 + bx + c}$): For $a > 0$, substitute $\sqrt{ax^2 + bx + c} = t \pm x \sqrt{a}$

## VI. Integration Techniques & Rules

* Integration by Parts (ILATE Rule): $\int u \, dv = uv - \int v \, du$

* Substitution Rule (Chain Rule Reverse): $\int f(g(x))g'(x) \, dx = \int f(u) \, du$ where $u = g(x)$

* Standard Form Integration by Parts (Exponential Product): $\int e^x [f(x) + f'(x)] \, dx = e^x f(x) + C$

* Trigonometric Substitution ($a^2 - x^2$): Substitute $x = a \sin \theta$ or $x = a \cos \theta$

* Trigonometric Substitution ($a^2 + x^2$): Substitute $x = a \tan \theta$ or $x = a \cot \theta$

* Trigonometric Substitution ($x^2 - a^2$): Substitute $x = a \sec \theta$ or $x = a \csc \theta$

## VII. Reduction Formulas

* Sine Power Reduction: $\int \sin^n x \, dx = -\frac{\sin^{n-1} x \cos x}{n} + \frac{n-1}{n} \int \sin^{n-2} x \, dx$

* Cosine Power Reduction: $\int \cos^n x \, dx = \frac{\cos^{n-1} x \sin x}{n} + \frac{n-1}{n} \int \cos^{n-2} x \, dx$

* Tangent Power Reduction: $\int \tan^n x \, dx = \frac{\tan^{n-1} x}{n-1} - \int \tan^{n-2} x \, dx$ (where $n \neq 1$)

* Secant Power Reduction: $\int \sec^n x \, dx = \frac{\sec^{n-2} x \tan x}{n-1} + \frac{n-2}{n-1} \int \sec^{n-2} x \, dx$ (where $n \neq 1$)

* Sine-Cosine Power Product (Wallis Form): $\int_0^{\pi/2} \sin^m x \cos^n x \, dx = \frac{(m-1)(m-3)\dots(n-1)(n-3)\dots}{(m+n)(m+n-2)\dots} \times k$ (where $k = \frac{\pi}{2}$ if both $m, n$ are even, else $1$)

## VIII. Definite Integrals and Properties

* Newton-Leibniz Formula: $\int_a^b f(x) \, dx = F(b) - F(a)$ where $F'(x) = f(x)$

* Reflection Property (King's Property): $\int_a^b f(x) \, dx = \int_a^b f(a + b - x) \, dx$

* Symmetry (Even Function): If $f(-x) = f(x)$, then $\int_{-a}^a f(x) \, dx = 2 \int_0^a f(x) \, dx$

* Symmetry (Odd Function): If $f(-x) = -f(x)$, then $\int_{-a}^a f(x) \, dx = 0$

* Periodic Function Property: $\int_0^{nT} f(x) \, dx = n \int_0^T f(x) \, dx$ (where $f(x+T) = f(x)$)

* Leibniz Rule (Differentiation Under Integral Sign): $\frac{d}{dx} \left[ \int_{\alpha(x)}^{\beta(x)} f(x, t) \, dt \right] = f(x, \beta(x))\beta'(x) - f(x, \alpha(x))\alpha'(x) + \int_{\alpha(x)}^{\beta(x)} \frac{\partial f}{\partial x} dt$

## IX. Special Functions (Beta and Gamma)

* Gamma Function Definition: $\Gamma(n) = \int_0^\infty e^{-x} x^{n-1} \, dx$ (where $\Gamma(n+1) = n!$ for integer $n$, and $\Gamma(1/2) = \sqrt{\pi}$)

* Beta Function Definition: $B(m, n) = \int_0^1 x^{m-1} (1-x)^{n-1} \, dx$

* Relation Between Beta and Gamma: $B(m, n) = \frac{\Gamma(m)\Gamma(n)}{\Gamma(m+n)}$

## X. Limits of Sums (Definite Integral as Limit of a Sum)

* Riemann Sum Definition: $\lim_{n \to \infty} \frac{1}{n} \sum_{r=1}^{n} f\left(\frac{r}{n}\right) = \int_0^1 f(x) \, dx$

* General Riemann Sum Form: $\lim_{n \to \infty} \sum_{r=1}^{n} \frac{1}{n} f\left(a + \frac{r}{n}(b-a)\right) = \int_a^b f(x) \, dx$