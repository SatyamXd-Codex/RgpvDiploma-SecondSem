
## UNIT - IV: Vector Algebra

Vector algebra is a branch of mathematics that deals with vectors. Vectors are mathematical objects that have both magnitude (size) and direction, making them distinct from scalars, which only have magnitude. Vector algebra provides tools to work with these quantities, essential in physics, engineering, and computer graphics.

### I. Definition, Notation, and Rectangular Resolution of a Vector

#### A. Definition of a Vector

* **Vector:** A quantity that has both **magnitude** (a numerical value or size) and **direction**.
    * Examples: Displacement, velocity, acceleration, force, momentum, electric field.
* **Scalar:** A quantity that has only **magnitude**.
    * Examples: Distance, speed, mass, temperature, time, energy, volume.

#### B. Notation of a Vector

* **Geometric Representation:** A vector is usually represented by a directed line segment (an arrow).
    * The length of the arrow represents its magnitude.
    * The arrowhead indicates its direction.
    * If a vector starts at point A and ends at point B, it is denoted as $\vec{AB}$.
* **Symbolic Representation:**
    * Typically denoted by a lowercase letter with an arrow above it (e.g., $\vec{a}, \vec{b}, \vec{v}$) or in boldface (e.g., **a**, **b**, **v**).
* **Magnitude (Modulus) of a Vector:** The length or size of the vector.
    * If $\vec{a}$, its magnitude is denoted as $|\vec{a}|$ or $a$.

#### C. Rectangular Resolution of a Vector

* **Concept:** Any vector in 2D or 3D space can be expressed as the sum of its components along mutually perpendicular axes (usually the x, y, and z axes).
* **Unit Vectors:**
    * $\hat{i}$: Unit vector along the positive x-axis.
    * $\hat{j}$: Unit vector along the positive y-axis.
    * $\hat{k}$: Unit vector along the positive z-axis.
    * These unit vectors have a magnitude of 1.
* **Resolution in 2D:**
    * A vector $\vec{A}$ in the xy-plane can be resolved into components $A_x$ and $A_y$.
    * **Formula:** $\vec{A} = A_x \hat{i} + A_y \hat{j}$
        * If $\theta$ is the angle $\vec{A}$ makes with the positive x-axis:
            * $A_x = |\vec{A}| \cos \theta$
            * $A_y = |\vec{A}| \sin \theta$
    * **Magnitude:** $|\vec{A}| = \sqrt{A_x^2 + A_y^2}$
    * **Direction:** $\tan \theta = \frac{A_y}{A_x}$

* **Resolution in 3D:**
    * A vector $\vec{A}$ in 3D space can be resolved into components $A_x, A_y, A_z$.
    * **Formula:** $\vec{A} = A_x \hat{i} + A_y \hat{j} + A_z \hat{k}$
        * If the vector passes through point $(x_1, y_1, z_1)$ and $(x_2, y_2, z_2)$, then its components are $A_x = x_2-x_1$, $A_y = y_2-y_1$, $A_z = z_2-z_1$.
    * **Magnitude:** $|\vec{A}| = \sqrt{A_x^2 + A_y^2 + A_z^2}$
    * **Direction Cosines:** If $\alpha, \beta, \gamma$ are the angles the vector makes with the x, y, z axes respectively, then:
        * $\cos \alpha = \frac{A_x}{|\vec{A}|}$
        * $\cos \beta = \frac{A_y}{|\vec{A}|}$
        * $\cos \gamma = \frac{A_z}{|\vec{A}|}$
        * $\cos^2 \alpha + \cos^2 \beta + \cos^2 \gamma = 1$

### II. Addition and Subtraction of Vectors

#### A. Vector Addition

* **Triangle Law of Vector Addition:** If two vectors are represented in magnitude and direction by two sides of a triangle taken in the same order, then their resultant is represented by the third side taken in the opposite order.
    * If $\vec{a}$ and $\vec{b}$ are two vectors, then $\vec{R} = \vec{a} + \vec{b}$.
* **Parallelogram Law of Vector Addition:** If two vectors acting at a point are represented in magnitude and direction by the two adjacent sides of a parallelogram drawn from a point, then their resultant is represented in magnitude and direction by the diagonal of the parallelogram drawn from the same point.
* **Analytical Method (using components):**
    * If $\vec{a} = a_x \hat{i} + a_y \hat{j} + a_z \hat{k}$
    * And $\vec{b} = b_x \hat{i} + b_y \hat{j} + b_z \hat{k}$
    * **Formula:** $\vec{a} + \vec{b} = (a_x + b_x) \hat{i} + (a_y + b_y) \hat{j} + (a_z + b_z) \hat{k}$

#### B. Vector Subtraction

* **Concept:** Subtracting a vector $\vec{b}$ from $\vec{a}$ is equivalent to adding the negative of $\vec{b}$ to $\vec{a}$, i.e., $\vec{a} - \vec{b} = \vec{a} + (-\vec{b})$. The negative of a vector has the same magnitude but opposite direction.
* **Analytical Method (using components):**
    * If $\vec{a} = a_x \hat{i} + a_y \hat{j} + a_z \hat{k}$
    * And $\vec{b} = b_x \hat{i} + b_y \hat{j} + b_z \hat{k}$
    * **Formula:** $\vec{a} - \vec{b} = (a_x - b_x) \hat{i} + (a_y - b_y) \hat{j} + (a_z - b_z) \hat{k}$

### III. Scalar (Dot) Product of 2 Vectors

* **Definition:** The scalar product (or dot product) of two vectors results in a scalar quantity. It is a measure of how much one vector extends in the direction of the other.
* **Notation:** $\vec{a} \cdot \vec{b}$
* **Geometric Formula:**
    $$\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos \theta$$
    * Where $\theta$ is the angle between $\vec{a}$ and $\vec{b}$ ($0 \le \theta \le \pi$).
* **Component Formula:**
    * If $\vec{a} = a_x \hat{i} + a_y \hat{j} + a_z \hat{k}$
    * And $\vec{b} = b_x \hat{i} + b_y \hat{j} + b_z \hat{k}$
    * $$\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z$$
* **Properties:**
    * Commutative: $\vec{a} \cdot \vec{b} = \vec{b} \cdot \vec{a}$
    * Distributive: $\vec{a} \cdot (\vec{b} + \vec{c}) = \vec{a} \cdot \vec{b} + \vec{a} \cdot \vec{c}$
    * $\hat{i} \cdot \hat{i} = \hat{j} \cdot \hat{j} = \hat{k} \cdot \hat{k} = 1$
    * $\hat{i} \cdot \hat{j} = \hat{j} \cdot \hat{k} = \hat{k} \cdot \hat{i} = 0$
    * If $\vec{a} \cdot \vec{b} = 0$ and $\vec{a}, \vec{b}$ are non-zero vectors, then $\vec{a}$ and $\vec{b}$ are **perpendicular** (orthogonal).
    * Projection of $\vec{a}$ on $\vec{b}$: $\frac{\vec{a} \cdot \vec{b}}{|\vec{b}|}$

### IV. Vector (Cross) Product of 2 Vectors

* **Definition:** The vector product (or cross product) of two vectors results in a vector quantity. The resulting vector is perpendicular to the plane containing the two original vectors.
* **Notation:** $\vec{a} \times \vec{b}$
* **Geometric Formula:**
    $$\vec{a} \times \vec{b} = (|\vec{a}| |\vec{b}| \sin \theta) \hat{n}$$
    * Where $\theta$ is the angle between $\vec{a}$ and $\vec{b}$ ($0 \le \theta \le \pi$).
    * $\hat{n}$ is a unit vector perpendicular to the plane containing $\vec{a}$ and $\vec{b}$, whose direction is given by the right-hand rule.
    * The magnitude of the cross product: $|\vec{a} \times \vec{b}| = |\vec{a}| |\vec{b}| \sin \theta$. Geometrically, this magnitude represents the area of the parallelogram formed by vectors $\vec{a}$ and $\vec{b}$.
* **Component Formula (Determinant Form):**
    * If $\vec{a} = a_x \hat{i} + a_y \hat{j} + a_z \hat{k}$
    * And $\vec{b} = b_x \hat{i} + b_y \hat{j} + b_z \hat{k}$
    * $$\vec{a} \times \vec{b} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ a_x & a_y & a_z \\ b_x & b_y & b_z \end{vmatrix}$$    * $$= (a_y b_z - a_z b_y) \hat{i} - (a_x b_z - a_z b_x) \hat{j} + (a_x b_y - a_y b_x) \hat{k}$$
* **Properties:**
    * Not Commutative: $\vec{a} \times \vec{b} = -(\vec{b} \times \vec{a})$
    * Distributive: $\vec{a} \times (\vec{b} + \vec{c}) = \vec{a} \times \vec{b} + \vec{a} \times \vec{c}$
    * $\hat{i} \times \hat{i} = \hat{j} \times \hat{j} = \hat{k} \times \hat{k} = \vec{0}$
    * $\hat{i} \times \hat{j} = \hat{k}$
    * $\hat{j} \times \hat{k} = \hat{i}$
    * $\hat{k} \times \hat{i} = \hat{j}$
    * If $\vec{a} \times \vec{b} = \vec{0}$ and $\vec{a}, \vec{b}$ are non-zero vectors, then $\vec{a}$ and $\vec{b}$ are **parallel** (collinear).

### V. Simple Problems Related to Work, Moment, and Angular Velocity

Vectors are fundamental to expressing and solving problems in physics.

#### A. Work Done

* **Concept:** Work done by a constant force is the product of the magnitude of the force, the magnitude of the displacement, and the cosine of the angle between them. It is a scalar quantity.
* **Formula:** $W = \vec{F} \cdot \vec{d}$
    * $W$: Work done (scalar)
    * $\vec{F}$: Force vector
    * $\vec{d}$: Displacement vector
    * This is a direct application of the **Scalar (Dot) Product**.

* **Problem Type:** Given force vector $\vec{F}$ and displacement vector $\vec{d}$, find the work done.
    * Example: If $\vec{F} = (2\hat{i} + 3\hat{j} - \hat{k})$ Newtons and $\vec{d} = (\hat{i} - 2\hat{j} + 4\hat{k})$ meters.
        $W = (2)(1) + (3)(-2) + (-1)(4) = 2 - 6 - 4 = -8$ Joules.

#### B. Moment (Torque)

* **Concept:** The moment (or torque) of a force about a point measures the tendency of the force to cause rotation around that point. It is a vector quantity.
* **Formula:** $\vec{\tau} = \vec{r} \times \vec{F}$
    * $\vec{\tau}$: Torque vector
    * $\vec{r}$: Position vector from the point of rotation to the point where the force is applied.
    * $\vec{F}$: Force vector
    * This is a direct application of the **Vector (Cross) Product**.

* **Problem Type:** Given a force $\vec{F}$ acting at a point with position vector $\vec{r}$ from the origin (or another reference point), find the moment about the origin.
    * Example: Force $\vec{F} = (2\hat{i} - \hat{j} + 3\hat{k})$ acts at a point whose position vector is $\vec{r} = (\hat{i} + 4\hat{j} - 2\hat{k})$. Find the moment of the force about the origin.
        $$\vec{\tau} = \vec{r} \times \vec{F} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 1 & 4 & -2 \\ 2 & -1 & 3 \end{vmatrix}$$       $$= ( (4)(3) - (-2)(-1) ) \hat{i} - ( (1)(3) - (-2)(2) ) \hat{j} + ( (1)(-1) - (4)(2) ) \hat{k}$$       $$= (12 - 2) \hat{i} - (3 + 4) \hat{j} + (-1 - 8) \hat{k}$$       $$= 10\hat{i} - 7\hat{j} - 9\hat{k}$$

#### C. Angular Velocity

* **Concept:** Angular velocity describes the rate of change of angular displacement. For a particle moving in a circular path, its linear velocity can be related to its angular velocity and position vector.
* **Formula:** $\vec{v} = \vec{\omega} \times \vec{r}$
    * $\vec{v}$: Linear velocity vector of a particle.
    * $\vec{\omega}$: Angular velocity vector (points along the axis of rotation).
    * $\vec{r}$: Position vector of the particle from the origin (or point on the axis of rotation).
    * This is also a direct application of the **Vector (Cross) Product**.

* **Problem Type:** Given the angular velocity vector and the position vector of a particle, find its linear velocity.
    * Example: A particle moves with angular velocity $\vec{\omega} = (3\hat{i} - \hat{j} + 2\hat{k})$ about the origin. Find its linear velocity $\vec{v}$ when its position vector is $\vec{r} = (\hat{i} + 2\hat{j} - 3\hat{k})$.
        $$\vec{v} = \vec{\omega} \times \vec{r} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 3 & -1 & 2 \\ 1 & 2 & -3 \end{vmatrix}$$       $$= ( (-1)(-3) - (2)(2) ) \hat{i} - ( (3)(-3) - (2)(1) ) \hat{j} + ( (3)(2) - (-1)(1) ) \hat{k}$$       $$= (3 - 4) \hat{i} - (-9 - 2) \hat{j} + (6 + 1) \hat{k}$$       $$= -\hat{i} + 11\hat{j} + 7\hat{k}$$
