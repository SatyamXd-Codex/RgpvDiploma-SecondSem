

## UNIT - II: Integral Calculus

Integral calculus is a branch of calculus concerned with the theory and applications of integrals. It deals with concepts like accumulation, areas, volumes, and other quantities that can be thought of as the sum of infinitesimally small parts.

### I. Integration as Inverse Operation of Differentiation (Anti-derivative)

* **Concept:** Integration is fundamentally the reverse process of differentiation. If you differentiate a function $F(x)$ to get $f(x)$, then integrating $f(x)$ will give you $F(x)$ (plus a constant).
* **Formula:** If $\frac{d}{dx} F(x) = f(x)$, then $\int f(x) dx = F(x) + C$
    * **$f(x)$:** The integrand (the function to be integrated).
    * **$dx$:** Indicates that the integration is with respect to the variable $x$.
    * **$F(x)$:** The anti-derivative or primitive function.
    * **$C$:** The constant of integration. This is added because the derivative of any constant is zero. When we reverse the differentiation, we lose information about any constant that might have been present.

* **Basic Integration Formulas (from differentiation rules):**
    1.  $\int x^n dx = \frac{x^{n+1}}{n+1} + C$ (for $n \neq -1$)
    2.  $\int \frac{1}{x} dx = \ln|x| + C$
    3.  $\int e^x dx = e^x + C$
    4.  $\int a^x dx = \frac{a^x}{\ln a} + C$ (for $a > 0, a \neq 1$)
    5.  $\int \sin x dx = -\cos x + C$
    6.  $\int \cos x dx = \sin x + C$
    7.  $\int \sec^2 x dx = \tan x + C$
    8.  $\int \csc^2 x dx = -\cot x + C$
    9.  $\int \sec x \tan x dx = \sec x + C$
    10. $\int \csc x \cot x dx = -\csc x + C$
    11. $\int \frac{1}{\sqrt{a^2 - x^2}} dx = \sin^{-1}\left(\frac{x}{a}\right) + C$
    12. $\int \frac{1}{a^2 + x^2} dx = \frac{1}{a} \tan^{-1}\left(\frac{x}{a}\right) + C$
    13. $\int \frac{1}{x\sqrt{x^2 - a^2}} dx = \frac{1}{a} \sec^{-1}\left(\frac{x}{a}\right) + C$
    14. $\int \frac{1}{x^2 - a^2} dx = \frac{1}{2a} \ln\left|\frac{x-a}{x+a}\right| + C$
    15. $\int \frac{1}{a^2 - x^2} dx = \frac{1}{2a} \ln\left|\frac{a+x}{a-x}\right| + C$

### II. Simple Integration Techniques

#### A. Integration by Substitution (Change of Variable)

* **Concept:** This technique is used when the integrand is a composite function, and its derivative (or a multiple of it) is also present in the integral. We substitute a part of the integrand with a new variable, simplifying the integral.
* **Formula/Method:**
    To evaluate $\int f(g(x)) g'(x) dx$:
    1.  Let $u = g(x)$.
    2.  Differentiate $u$ with respect to $x$: $\frac{du}{dx} = g'(x)$, which implies $du = g'(x) dx$.
    3.  Substitute $u$ and $du$ into the integral: $\int f(u) du$.
    4.  Integrate with respect to $u$.
    5.  Replace $u$ with $g(x)$ to get the result in terms of $x$.
* **Example:** $\int 2x \cos(x^2) dx$
    1.  Let $u = x^2$.
    2.  $du = 2x dx$.
    3.  Substitute: $\int \cos(u) du$.
    4.  Integrate: $\sin(u) + C$.
    5.  Substitute back: $\sin(x^2) + C$.

#### B. Integration by Parts

* **Concept:** Used to integrate products of two different types of functions (e.g., algebraic and trigonometric, logarithmic and exponential). It's based on the product rule of differentiation.
* **Formula:** $\int u \, dv = uv - \int v \, du$
    * **Choosing $u$ and $dv$:** Use the "ILATE" rule (or LIATE) to prioritize $u$:
        * **I** - Inverse trigonometric functions ($\sin^{-1}x$, $\cos^{-1}x$, etc.)
        * **L** - Logarithmic functions ($\ln x$, $\log_a x$, etc.)
        * **A** - Algebraic functions ($x^n$, polynomials)
        * **T** - Trigonometric functions ($\sin x$, $\cos x$, etc.)
        * **E** - Exponential functions ($e^x$, $a^x$)
        The function appearing earlier in ILATE should generally be chosen as $u$. The remaining part is $dv$.
* **Example:** $\int x \sin x dx$
    1.  Choose $u$ and $dv$:
        * Let $u = x$ (Algebraic, comes before Trigonometric in ILATE).
        * Let $dv = \sin x dx$.
    2.  Find $du$ and $v$:
        * $du = dx$.
        * $v = \int \sin x dx = -\cos x$.
    3.  Apply the formula:
        $\int x \sin x dx = x(-\cos x) - \int (-\cos x) dx$
        $= -x \cos x + \int \cos x dx$
        $= -x \cos x + \sin x + C$.

#### C. Integration by Partial Fractions (for Linear Factors Only)

* **Concept:** Used for integrating rational functions (a polynomial divided by another polynomial) where the denominator can be factored into linear factors. The rational function is decomposed into simpler fractions that are easier to integrate.
* **Conditions:**
    * The degree of the numerator must be less than the degree of the denominator (if not, perform polynomial long division first).
    * The denominator must be factorable into linear factors.
* **Formula/Method (for linear factors):**
    1.  **Non-repeated Linear Factors:**
        If the denominator is $(ax+b)(cx+d)$, then:
        $$\frac{P(x)}{(ax+b)(cx+d)} = \frac{A}{ax+b} + \frac{B}{cx+d}$$
    2.  **Repeated Linear Factors:**
        If the denominator is $(ax+b)^n$, then:
        $$\frac{P(x)}{(ax+b)^n} = \frac{A_1}{ax+b} + \frac{A_2}{(ax+b)^2} + \dots + \frac{A_n}{(ax+b)^n}$$
    * **Steps:**
        * Factorize the denominator.
        * Set up the partial fraction decomposition with unknown constants (A, B, etc.).
        * Multiply both sides by the original denominator to clear it.
        * Solve for the constants by substituting specific values of $x$ (roots of factors) or by equating coefficients of like powers of $x$.
        * Integrate each resulting simple fraction (usually of the form $\int \frac{1}{ax+b} dx = \frac{1}{a} \ln|ax+b| + C$).
* **Example:** $\int \frac{1}{x^2 - 1} dx$
    1.  Factor denominator: $x^2 - 1 = (x-1)(x+1)$.
    2.  Decompose: $\frac{1}{(x-1)(x+1)} = \frac{A}{x-1} + \frac{B}{x+1}$
    3.  Clear denominator: $1 = A(x+1) + B(x-1)$
    4.  Solve for A, B:
        * Set $x=1 \Rightarrow 1 = A(2) + B(0) \Rightarrow A = 1/2$.
        * Set $x=-1 \Rightarrow 1 = A(0) + B(-2) \Rightarrow B = -1/2$.
    5.  Integrate:
        $\int \left(\frac{1/2}{x-1} - \frac{1/2}{x+1}\right) dx$
        $= \frac{1}{2} \int \frac{1}{x-1} dx - \frac{1}{2} \int \frac{1}{x+1} dx$
        $= \frac{1}{2} \ln|x-1| - \frac{1}{2} \ln|x+1| + C$
        $= \frac{1}{2} \ln\left|\frac{x-1}{x+1}\right| + C$.

### III. Definite Integrals and Reduction Formulas (Wallis' Formulas)

* **Definite Integral:** An integral with upper and lower limits of integration. It evaluates to a numerical value, representing a signed area under the curve.
    * Formula: $\int_a^b f(x) dx = F(b) - F(a)$ (where $F(x)$ is the anti-derivative of $f(x)$).

* **Wallis' Formulas (Reduction Formulas for $\int_0^{\pi/2}$):** These are special formulas for definite integrals of powers of sine and cosine over the interval $[0, \pi/2]$. They are extremely useful for directly solving problems.

1.  **$\int_0^{\pi/2} \sin^n x \, dx$ and $\int_0^{\pi/2} \cos^n x \, dx$**
    * **If n is an even positive integer (n = 2, 4, 6, ...):**
        $$\int_0^{\pi/2} \sin^n x \, dx = \int_0^{\pi/2} \cos^n x \, dx = \frac{(n-1)(n-3) \dots 1}{n(n-2) \dots 2} \times \frac{\pi}{2}$$
    * **If n is an odd positive integer (n = 1, 3, 5, ...):**
        $$\int_0^{\pi/2} \sin^n x \, dx = \int_0^{\pi/2} \cos^n x \, dx = \frac{(n-1)(n-3) \dots 2}{n(n-2) \dots 1}$$

2.  **$\int_0^{\pi/2} \sin^m x \cos^n x \, dx$ (where m and n are positive integers)**
    * **Formula:**
        $$\int_0^{\pi/2} \sin^m x \cos^n x \, dx = \frac{[(m-1)(m-3)\dots][(n-1)(n-3)\dots]}{(m+n)(m+n-2)\dots}$$
    * **Multiplication Factor:**
        * If both $m$ and $n$ are even, multiply the entire expression by $\frac{\pi}{2}$.
        * If either $m$ or $n$ (or both) are odd, do NOT multiply by $\frac{\pi}{2}$.
    * **Note:** The terms in the brackets (e.g., $(m-1)(m-3)\dots$) continue until the factor becomes 1 (for odd numbers) or 2 (for even numbers). If $m$ or $n$ is 1, the corresponding bracket will be considered as 1. If $m$ or $n$ is 0, the corresponding bracket will also be considered as 1.

### IV. Applications of Integration

#### A. Simple Problem on Evaluation of Area Bounded by a Curve and Axes

* **Concept:** Definite integrals can be used to calculate the area of a region bounded by a curve, the x-axis (or y-axis), and given vertical (or horizontal) lines.
* **Formulas:**
    1.  **Area bounded by curve $y = f(x)$, x-axis, and ordinates $x=a, x=b$:**
        $$Area = \int_a^b y \, dx = \int_a^b f(x) \, dx$$
        (If the curve is below the x-axis, the integral will be negative; take its absolute value for area).
    2.  **Area bounded by curve $x = g(y)$, y-axis, and abscissas $y=c, y=d$:**
        $$Area = \int_c^d x \, dy = \int_c^d g(y) \, dy$$
* **Steps:**
    1.  Sketch the curve and the bounded region to understand the limits.
    2.  Identify the function to integrate ($y$ in terms of $x$ or $x$ in terms of $y$).
    3.  Set up the definite integral with the correct limits.
    4.  Evaluate the integral.

#### B. Calculation of Volume of a Solid Formed by Revolution of an Area about Axes (Simple Problems)

* **Concept:** Integration can be used to find the volume of a three-dimensional solid generated by revolving a two-dimensional area around an axis (either the x-axis or the y-axis). This is often called the Disk Method or Washer Method.
* **Formulas (Disk Method - for simple cases where the region touches the axis of revolution):**
    1.  **Volume of solid formed by revolving area bounded by curve $y = f(x)$, x-axis, and $x=a, x=b$ about the x-axis:**
        $$Volume = \int_a^b \pi y^2 \, dx = \int_a^b \pi [f(x)]^2 \, dx$$
        * **Explanation:** Imagine slicing the solid into thin disks perpendicular to the x-axis. Each disk has a radius $y$ and thickness $dx$. The volume of one disk is $\pi r^2 h = \pi y^2 dx$. Integrating these volumes sums them up.
    2.  **Volume of solid formed by revolving area bounded by curve $x = g(y)$, y-axis, and $y=c, y=d$ about the y-axis:**
        $$Volume = \int_c^d \pi x^2 \, dy = \int_c^d \pi [g(y)]^2 \, dy$$
        * **Explanation:** Similar to the x-axis case, but disks are perpendicular to the y-axis, with radius $x$ and thickness $dy$.
* **Steps:**
    1.  Sketch the area to be revolved and the axis of revolution.
    2.  Determine the variable of integration (x if revolving around x-axis, y if revolving around y-axis).
    3.  Express the radius of the disk in terms of the variable of integration ($y$ for x-axis revolution, $x$ for y-axis revolution).
    4.  Identify the limits of integration.
    5.  Set up the integral with $\pi$ and the square of the radius.
    6.  Evaluate the integral.
