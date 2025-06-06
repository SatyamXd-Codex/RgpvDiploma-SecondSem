

## UNIT - III: Co-Ordinate Geometry

Co-ordinate geometry (also known as analytical geometry) is a branch of geometry where the positions of points are described using numerical coordinates. This allows for geometric problems to be solved using algebraic methods, and vice-versa.

### I. Equation of a Straight Line

A straight line is a fundamental geometric object. Its equation represents the set of all points that lie on that line.

#### A. Various Standard Forms of the Equation of a Straight Line (without proof)

1.  **Slope-Intercept Form:**
    * **Formula:** $y = mx + c$
    * **Explanation:**
        * $m$: slope of the line (how steep it is, $\text{rise}/\text{run}$).
        * $c$: y-intercept (the point where the line crosses the y-axis, i.e., $(0, c)$).
    * **Use:** Easiest to graph when slope and y-intercept are known.

2.  **Point-Slope Form:**
    * **Formula:** $y - y_1 = m(x - x_1)$
    * **Explanation:**
        * $m$: slope of the line.
        * $(x_1, y_1)$: a known point on the line.
    * **Use:** Useful when you have the slope and any point on the line.

3.  **Two-Point Form:**
    * **Formula:** $y - y_1 = \frac{y_2 - y_1}{x_2 - x_1}(x - x_1)$ (if $x_1 \neq x_2$)
    * **Explanation:**
        * $(x_1, y_1)$ and $(x_2, y_2)$: two known points on the line.
        * Note that $\frac{y_2 - y_1}{x_2 - x_1}$ is the slope $m$.
    * **Use:** When two points on the line are given.

4.  **Intercept Form:**
    * **Formula:** $\frac{x}{a} + \frac{y}{b} = 1$
    * **Explanation:**
        * $a$: x-intercept (the point where the line crosses the x-axis, i.e., $(a, 0)$).
        * $b$: y-intercept (the point where the line crosses the y-axis, i.e., $(0, b)$).
    * **Use:** When the x-intercept and y-intercept are known.

5.  **General Form (or Standard Form):**
    * **Formula:** $Ax + By + C = 0$
    * **Explanation:**
        * $A, B, C$: real numbers, where A and B are not both zero.
        * **Slope:** $m = -\frac{A}{B}$ (if $B \neq 0$)
        * **x-intercept:** $-\frac{C}{A}$ (if $A \neq 0$)
        * **y-intercept:** $-\frac{C}{B}$ (if $B \neq 0$)
    * **Use:** Any straight line can be represented in this form.

#### B. Intersection of Two Straight Lines

* **Concept:** The point of intersection of two lines is the unique point $(x, y)$ that satisfies the equations of both lines simultaneously.
* **Method:** To find the intersection of two lines, say $A_1x + B_1y + C_1 = 0$ and $A_2x + B_2y + C_2 = 0$, you can solve this system of linear equations using methods like:
    1.  **Substitution Method:** Solve one equation for one variable (e.g., $y$ in terms of $x$) and substitute it into the other equation.
    2.  **Elimination Method:** Multiply one or both equations by constants so that one of the variables has coefficients that are negatives of each other, then add the equations to eliminate that variable.
    3.  **Cross-Multiplication Method (for 2 equations, 2 variables):**
        $$\frac{x}{B_1C_2 - B_2C_1} = \frac{y}{C_1A_2 - C_2A_1} = \frac{1}{A_1B_2 - A_2B_1}$$
        This method directly gives $x$ and $y$.

* **Conditions for Intersection:**
    * **Unique Intersection:** If $\frac{A_1}{A_2} \neq \frac{B_1}{B_2}$, the lines intersect at a unique point. (Non-parallel lines)
    * **Parallel and Distinct (No Intersection):** If $\frac{A_1}{A_2} = \frac{B_1}{B_2} \neq \frac{C_1}{C_2}$, the lines are parallel but distinct, meaning they never intersect.
    * **Coincident (Infinitely Many Intersections):** If $\frac{A_1}{A_2} = \frac{B_1}{B_2} = \frac{C_1}{C_2}$, the lines are identical (coincident), meaning they overlap at every point.

#### C. Angle Between Two Lines

* **Concept:** The angle between two non-vertical lines with slopes $m_1$ and $m_2$ can be found using their slopes.
* **Formula:** If $\theta$ is the acute angle between two lines with slopes $m_1$ and $m_2$, then:
    $$\tan \theta = \left| \frac{m_1 - m_2}{1 + m_1 m_2} \right|$$
* **Special Cases:**
    * **Parallel Lines:** If the lines are parallel, $\theta = 0^\circ$ or $180^\circ$, so $\tan \theta = 0$. This implies $m_1 - m_2 = 0$, so $m_1 = m_2$.
    * **Perpendicular Lines:** If the lines are perpendicular, $\theta = 90^\circ$, so $\tan \theta$ is undefined. This implies $1 + m_1 m_2 = 0$, so $m_1 m_2 = -1$. (This means one slope is the negative reciprocal of the other, assuming neither is vertical).

#### D. Parallel and Perpendicular Lines

* **Parallel Lines:**
    * **Condition:** Two lines are parallel if and only if their slopes are equal ($m_1 = m_2$).
    * **Exception:** Two vertical lines (e.g., $x=k_1, x=k_2$) are parallel.

* **Perpendicular Lines:**
    * **Condition:** Two non-vertical lines are perpendicular if and only if the product of their slopes is $-1$ ($m_1 m_2 = -1$).
    * **Exception:** A horizontal line ($y=k$) is perpendicular to a vertical line ($x=c$).

#### E. Perpendicular Distance Formula

* **Concept:** The shortest distance from a given point to a given line.
* **Formula:** The perpendicular distance $d$ from a point $(x_1, y_1)$ to a line $Ax + By + C = 0$ is given by:
    $$d = \frac{|Ax_1 + By_1 + C|}{\sqrt{A^2 + B^2}}$$
* **Explanation:** The numerator is the absolute value of the expression from the line equation when the point coordinates are substituted. The denominator normalizes it by the magnitude of the normal vector to the line.

### II. General Equation of a Circle and its Characteristics

#### A. General Equation of a Circle

* **Formula:** $x^2 + y^2 + 2gx + 2fy + c = 0$
* **Characteristics (derived from the general equation):**
    * **Center:** The center of the circle is at $(-g, -f)$.
    * **Radius:** The radius $r$ of the circle is given by $r = \sqrt{g^2 + f^2 - c}$.
    * **Condition for a Real Circle:** For a real circle to exist, the radius must be real, so $g^2 + f^2 - c > 0$.
        * If $g^2 + f^2 - c = 0$, the equation represents a **point circle** (radius is 0).
        * If $g^2 + f^2 - c < 0$, the equation represents an **imaginary circle** (no real points satisfy the equation).

#### B. To Find the Equation of a Circle, Given:

1.  **Centre $(h, k)$ and Radius $r$:**
    * **Formula (Standard Form):** $(x - h)^2 + (y - k)^2 = r^2$
    * **Explanation:** This is derived from the distance formula. Any point $(x, y)$ on the circle is at a fixed distance $r$ from the center $(h, k)$.

2.  **Three Points Lying on It:**
    * **Method:**
        1.  Let the general equation of the circle be $x^2 + y^2 + 2gx + 2fy + c = 0$.
        2.  Substitute the coordinates of each of the three given points into this general equation.
        3.  This will give you three linear equations in terms of $g, f,$ and $c$.
        4.  Solve this system of three linear equations simultaneously to find the values of $g, f,$ and $c$.
        5.  Substitute these values back into the general equation to get the specific equation of the circle.

3.  **Coordinates of End Points of a Diameter $(x_1, y_1)$ and $(x_2, y_2)$:**
    * **Method 1 (Midpoint and Distance):**
        1.  **Center:** The center of the circle is the midpoint of the diameter:
            $(h, k) = \left(\frac{x_1 + x_2}{2}, \frac{y_1 + y_2}{2}\right)$
        2.  **Radius:** The radius is half the length of the diameter. The diameter length is found using the distance formula between $(x_1, y_1)$ and $(x_2, y_2)$.
            $D = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$
            $r = \frac{D}{2}$
        3.  Substitute $(h, k)$ and $r$ into the standard form: $(x - h)^2 + (y - k)^2 = r^2$.
    * **Method 2 (Diameter Form):**
        1.  **Formula:** $(x - x_1)(x - x_2) + (y - y_1)(y - y_2) = 0$
        2.  **Explanation:** This formula is derived from the property that the angle subtended by a diameter at any point on the circumference is $90^\circ$. If $P(x,y)$ is any point on the circle, then the lines connecting $P$ to the endpoints of the diameter are perpendicular.

### III. Definition of Conics and Their Standard Equations (without proof)

Conic sections are curves formed by the intersection of a plane with a double-napped cone. They include circles (a special case), parabolas, ellipses, and hyperbolas.

#### A. Definition of Conics (General)

A conic section can be defined as the locus of a point that moves in a plane such that its distance from a fixed point (called the **focus**, $S$) is always in a constant ratio to its perpendicular distance from a fixed straight line (called the **directrix**, $L$).
* This constant ratio is called the **eccentricity**, denoted by $e$.
* If $P$ is a point on the conic, $S$ is the focus, and $PM$ is the perpendicular distance from $P$ to the directrix $L$, then $\frac{SP}{PM} = e$.

#### B. Types of Conics based on Eccentricity ($e$)

1.  **Parabola:**
    * **Definition:** The set of all points that are equidistant from a fixed point (focus) and a fixed line (directrix).
    * **Eccentricity:** $e = 1$.
    * **Standard Equation (Opening Right/Left):** $y^2 = 4ax$ (Focus: $(a,0)$, Directrix: $x = -a$)
        * If $a < 0$, it opens left ($y^2 = -4|a|x$).
    * **Standard Equation (Opening Up/Down):** $x^2 = 4ay$ (Focus: $(0,a)$, Directrix: $y = -a$)
        * If $a < 0$, it opens down ($x^2 = -4|a|y$).
    * **Vertex:** $(0,0)$ for these standard forms.

2.  **Ellipse:**
    * **Definition:** The set of all points for which the sum of the distances from two fixed points (foci) is constant.
    * **Eccentricity:** $0 < e < 1$.
    * **Standard Equation (Horizontal Major Axis):** $\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$ (where $a > b$)
        * **Foci:** $(\pm ae, 0)$
        * **Vertices:** $(\pm a, 0)$
        * **Major Axis Length:** $2a$
        * **Minor Axis Length:** $2b$
        * **Relationship:** $b^2 = a^2(1 - e^2)$
    * **Standard Equation (Vertical Major Axis):** $\frac{x^2}{b^2} + \frac{y^2}{a^2} = 1$ (where $a > b$)
        * **Foci:** $(0, \pm ae)$
        * **Vertices:** $(0, \pm a)$
        * **Relationship:** $b^2 = a^2(1 - e^2)$
    * **Center:** $(0,0)$ for these standard forms.

3.  **Hyperbola:**
    * **Definition:** The set of all points for which the absolute difference of the distances from two fixed points (foci) is constant.
    * **Eccentricity:** $e > 1$.
    * **Standard Equation (Horizontal Transverse Axis):** $\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1$
        * **Foci:** $(\pm ae, 0)$
        * **Vertices:** $(\pm a, 0)$
        * **Transverse Axis Length:** $2a$
        * **Conjugate Axis Length:** $2b$
        * **Relationship:** $b^2 = a^2(e^2 - 1)$
    * **Standard Equation (Vertical Transverse Axis):** $\frac{y^2}{a^2} - \frac{x^2}{b^2} = 1$
        * **Foci:** $(0, \pm ae)$
        * **Vertices:** $(0, \pm a)$
        * **Relationship:** $b^2 = a^2(e^2 - 1)$
    * **Center:** $(0,0)$ for these standard forms.

#### C. Problems on Conics when their Foci, Directrices or Vertices are given.

These problems typically involve using the definitions and standard forms to derive the equation of the conic.

* **Given Focus and Directrix (and Eccentricity):**
    * Use the general definition: $SP = e \cdot PM$.
    * Let $P(x,y)$ be a point on the conic.
    * $S(x_0, y_0)$ is the given focus.
    * $L$ is the given directrix ($Ax + By + C = 0$).
    * $SP = \sqrt{(x - x_0)^2 + (y - y_0)^2}$
    * $PM = \frac{|Ax + By + C|}{\sqrt{A^2 + B^2}}$
    * Substitute into $SP = e \cdot PM$ and square both sides to eliminate the square root and absolute value. Simplify to get the equation of the conic.
    * **For Parabola ($e=1$):** This directly gives the equation.

* **Given Vertices or Foci for Ellipse/Hyperbola:**
    * **Strategy:** Identify the type of conic (ellipse or hyperbola) and whether its major/transverse axis is horizontal or vertical based on the given coordinates.
    * **Determine $a$ and $ae$ (or $b$):**
        * For **Ellipse**: Vertices are $(\pm a, 0)$ or $(0, \pm a)$. Foci are $(\pm ae, 0)$ or $(0, \pm ae)$.
        * For **Hyperbola**: Vertices are $(\pm a, 0)$ or $(0, \pm a)$. Foci are $(\pm ae, 0)$ or $(0, \pm ae)$.
    * From the given values, find $a$ and $ae$. Then calculate $e$.
    * Use the relationship between $a, b,$ and $e$ ($b^2 = a^2(1 - e^2)$ for ellipse; $b^2 = a^2(e^2 - 1)$ for hyperbola) to find $b^2$.
    * Substitute $a^2$ and $b^2$ into the appropriate standard equation.

**Example Problem Strategy:**
If you are given a focus $(3,0)$ and directrix $x = -3$, for instance, and asked to find the conic.
1.  Assume $P(x,y)$ on the conic.
2.  $SP = \sqrt{(x-3)^2 + (y-0)^2}$.
3.  $PM = |x - (-3)| / \sqrt{1^2 + 0^2} = |x+3|$.
4.  If $e=1$ (Parabola): $\sqrt{(x-3)^2 + y^2} = |x+3|$. Square both sides: $(x-3)^2 + y^2 = (x+3)^2$.
    $x^2 - 6x + 9 + y^2 = x^2 + 6x + 9$.
    $y^2 = 12x$. This is the equation of a parabola.
