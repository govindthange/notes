# 📐 Vector Algebra Formulas

## I. Basics and Magnitude

* Position Vector: $\vec{r} = x\hat{i} + y\hat{j} + z\hat{k}$

* Magnitude of a Vector: $|\vec{a}| = \sqrt{x^2 + y^2 + z^2}$

* Unit Vector: $\hat{a} = \frac{\vec{a}}{|\vec{a}|}$

* Direction Cosines: $l = \cos\alpha, m = \cos\beta, n = \cos\gamma$ (where $l^2 + m^2 + n^2 = 1$)

* Section Formula (Internal): $\vec{r} = \frac{m\vec{b} + n\vec{a}}{m + n}$

* Section Formula (External): $\vec{r} = \frac{m\vec{b} - n\vec{a}}{m - n}$

## II. Product of Vectors

* Dot (Scalar) Product: $\vec{a} \cdot \vec{b} = |\vec{a}||\vec{b}|\cos\theta = a_1b_1 + a_2b_2 + a_3b_3$

* Angle between Two Vectors: $\cos\theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|}$

* Cross (Vector) Product: $\vec{a} \times \vec{b} = |\vec{a}||\vec{b}|\sin\theta \, \hat{n} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3 \end{vmatrix}$

* Lagrange's Identity: $|\vec{a} \times \vec{b}|^2 + (\vec{a} \cdot \vec{b})^2 = |\vec{a}|^2 |\vec{b}|^2$

## III. Triple Products

* Scalar Triple Product (STP): $[\vec{a} \vec{b} \vec{c}] = \vec{a} \cdot (\vec{b} \times \vec{c}) = \begin{vmatrix} a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3 \\ c_1 & c_2 & c_3 \end{vmatrix}$

* Cyclic Property of STP: $[\vec{a} \vec{b} \vec{c}] = [\vec{b} \vec{c} \vec{a}] = [\vec{c} \vec{a} \vec{b}]$

* Vector Triple Product (VTP): $\vec{a} \times (\vec{b} \times \vec{c}) = (\vec{a} \cdot \vec{c})\vec{b} - (\vec{a} \cdot \vec{b})\vec{c}$

## IV. Geometrical Applications

* Projection of $\vec{a}$ on $\vec{b}$: $\text{proj}_{\vec{b}} \vec{a} = \frac{\vec{a} \cdot \vec{b}}{|\vec{b}|}$

* Area of Triangle (given two adjacent side vectors): $\text{Area} = \frac{1}{2} |\vec{a} \times \vec{b}|$

* Area of Parallelogram (given two adjacent side vectors): $\text{Area} = |\vec{a} \times \vec{b}|$

* Area of Parallelogram (given diagonals): $\text{Area} = \frac{1}{2} |\vec{d}_1 \times \vec{d}_2|$

* Volume of Parallelopiped: $V = |[\vec{a} \vec{b} \vec{c}]|$

* Volume of Tetrahedron: $V = \frac{1}{6} |[\vec{a} \vec{b} \vec{c}]|$

## V. Lines and Planes in Space

* Equation of a Line (Vector Form): $\vec{r} = \vec{a} + \lambda\vec{b}$

* Equation of a Line (Cartesian Form): $\frac{x - x_1}{a} = \frac{y - y_1}{b} = \frac{z - z_1}{c}$

* Equation of a Plane (Normal Form): $\vec{r} \cdot \hat{n} = d$

* Equation of a Plane (Cartesian Form): $Ax + By + Cz + D = 0$

* Distance from a Point to a Plane: $d = \frac{|Ax_1 + By_1 + Cz_1 + D|}{\sqrt{A^2 + B^2 + C^2}}$