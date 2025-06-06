# Unit IV: Centroid and Centre of Gravity

This unit delves into the fundamental concepts of **centroid** and **centre of gravity**, which are crucial for understanding the equilibrium and stability of various shapes and objects in engineering and physics.

---

## 1. Centroid

### Definition:
The **centroid** of a plane figure is its geometric center. It's the theoretical point where the entire area of the figure can be considered to be concentrated. For a uniform thin plate, the centroid coincides with its center of mass.
Let's explore Unit IV: Centroid and Centre of Gravity, covering the concepts and methods for locating the geometric and mass centers of various shapes and solids.

---

## Unit – IV: Centroid and Centre of Gravity

This unit introduces the concepts of centroid and centre of gravity, which are crucial for understanding the stability and behavior of objects under various loads. They are fundamental in structural analysis, machine design, and various other engineering applications.

### I. Centroid

* **Definition:** The centroid is the geometric center of an area, volume, or line. It is the point where the entire area (or volume or line) can be considered to be concentrated. For homogeneous bodies (uniform density), the centroid coincides with the center of gravity.
* **Significance:**
    * Simplifies calculations involving distributed forces (e.g., fluid pressure on a surface).
    * Crucial for calculating moments of inertia in mechanics of solids.
    * Used in design of structural elements like beams and columns.
* **Coordinate Calculation:** For a plane area, the coordinates ($\bar{x}, \bar{y}$) of the centroid are given by:
    * $\bar{x} = \frac{\int x \, dA}{\int dA} = \frac{\int x \, dA}{A}$
    * $\bar{y} = \frac{\int y \, dA}{\int dA} = \frac{\int y \, dA}{A}$
    * Where $A$ is the total area, and $x, y$ are the coordinates of differential area elements $dA$.

#### A. Centroid of Geometrical Plane Figures (Common Shapes)

It's essential to remember the centroid locations for standard geometric shapes relative to a common reference axis (often their base or a corner).

1.  **Square / Rectangle:**
    * **Area (A):** $b \times h$
    * **Centroid ($\bar{x}, \bar{y}$):**
        * From the base: $(\frac{b}{2}, \frac{h}{2})$
        * (Located at the intersection of its diagonals)

2.  **Triangle:**
    * **Area (A):** $\frac{1}{2} b \times h$
    * **Centroid ($\bar{x}, \bar{y}$):**
        * From the base (of side $b$): $(\frac{b}{2}, \frac{h}{3})$
        * (Located at the intersection of its medians. The centroid is always $1/3$ of the height from the base.)

3.  **Circle:**
    * **Area (A):** $\pi r^2 = \frac{\pi d^2}{4}$
    * **Centroid ($\bar{x}, \bar{y}$):**
        * At its geometric center (center of the circle).

4.  **Semi-circle:**
    * **Area (A):** $\frac{1}{2} \pi r^2$
    * **Centroid ($\bar{x}, \bar{y}$):**
        * Along the axis of symmetry, from the diameter:
        * $\bar{y} = \frac{4r}{3\pi}$
        * $\bar{x} = r$ (if the diameter lies along the x-axis and the center is at the origin)
        * (Symmetrically located along its axis of symmetry).

5.  **Quarter Circle:**
    * **Area (A):** $\frac{1}{4} \pi r^2$
    * **Centroid ($\bar{x}, \bar{y}$):**
        * From the corner (where the two perpendicular radii meet):
        * $\bar{x} = \frac{4r}{3\pi}$
        * $\bar{y} = \frac{4r}{3\pi}$
        * (Assumes the quarter circle is in the first quadrant with its corner at the origin).

#### B. Centroid of Composite Figures (Plane Areas)

A composite figure is made up of several simpler geometric shapes. The centroid of a composite figure is found by treating each simple shape as a "part" and using the principle of moments.

* **Method:**
    1.  **Divide the composite figure:** Break down the complex shape into simpler, standard geometric figures (rectangles, triangles, circles, etc.).
    2.  **Establish a reference axis:** Choose a convenient origin (X-Y axes). Often, the bottom-leftmost point of the figure is chosen.
    3.  **Calculate area and centroid for each part:** For each simple figure:
        * Calculate its area ($A_i$).
        * Determine the coordinates of its own centroid ($x_i, y_i$) relative to the chosen reference axis.
    4.  **Apply the centroid formulas for composite figures:**
        * $\bar{X} = \frac{\sum (A_i x_i)}{\sum A_i}$
        * $\bar{Y} = \frac{\sum (A_i y_i)}{\sum A_i}$
    * **For holes/cutouts:** Treat the area of the cutout as negative when summing areas and moments.
* **Limitation (as per syllabus):** Composed of not more than three geometrical figures. This implies a manageable number of parts for manual calculation.

### II. Centre of Gravity (CG)

* **Definition:** The centre of gravity (CG) of a body is the single point where the entire weight of the body appears to act. It's the point through which the resultant gravitational force passes, regardless of the orientation of the body.
* **Relationship with Centroid:**
    * For **homogeneous bodies** (uniform density and uniform gravitational field), the center of gravity coincides with the centroid.
    * For **non-homogeneous bodies** or bodies in non-uniform gravitational fields, the CG and centroid may not coincide. However, in most engineering mechanics problems, bodies are assumed to be homogeneous, so the terms are often used interchangeably.
* **Significance:**
    * Crucial for stability analysis (e.g., tipping of vehicles, stability of ships).
    * Used in balancing rotating machinery.
    * Essential for calculating moments and reactions in structures and machines.

#### A. Centre of Gravity of Simple Solids

The CG of simple, homogeneous solids is located at their geometric center.

1.  **Cube / Cuboid:**
    * **Volume (V):** $l \times b \times h$
    * **CG:** At the intersection of its diagonals. If origin is at one corner, then $(\frac{l}{2}, \frac{b}{2}, \frac{h}{2})$.

2.  **Cone:**
    * **Volume (V):** $\frac{1}{3} \pi r^2 h$
    * **CG (from the base along the axis of symmetry):** $\bar{y} = \frac{h}{4}$

3.  **Cylinder:**
    * **Volume (V):** $\pi r^2 h$
    * **CG (from the base along the axis of symmetry):** $\bar{y} = \frac{h}{2}$

4.  **Sphere:**
    * **Volume (V):** $\frac{4}{3} \pi r^3$
    * **CG:** At its geometric center.

5.  **Hemisphere:**
    * **Volume (V):** $\frac{2}{3} \pi r^3$
    * **CG (from the flat base along the axis of symmetry):** $\bar{y} = \frac{3r}{8}$

#### B. Centre of Gravity of Composite Solids

Similar to composite plane figures, the CG of a composite solid is found by considering the individual simple solids.

* **Method:**
    1.  **Divide the composite solid:** Break down the complex solid into simpler, standard solids (cubes, cylinders, cones, etc.).
    2.  **Establish a reference axis:** Choose a convenient origin (X-Y-Z axes).
    3.  **Calculate volume and centroid for each part:** For each simple solid:
        * Calculate its volume ($V_i$).
        * Determine the coordinates of its own centroid ($x_i, y_i, z_i$) relative to the chosen reference axis.
    4.  **Apply the CG formulas for composite solids:**
        * $\bar{X} = \frac{\sum (V_i x_i)}{\sum V_i}$
        * $\bar{Y} = \frac{\sum (V_i y_i)}{\sum V_i}$
        * $\bar{Z} = \frac{\sum (V_i z_i)}{\sum V_i}$
    * **For holes/cutouts:** Treat the volume of the cutout as negative when summing volumes and moments.
* **Limitation (as per syllabus):** Composed of not more than two simple solids. This simplifies the calculations to a manageable level.

**General Steps for Solving Centroid/CG Problems:**

1.  **Draw the figure:** Sketch the composite figure/solid clearly.
2.  **Choose a reference axis:** Select a convenient origin (e.g., bottom-left corner for 2D, or a corner of the base for 3D). All measurements will be from this origin.
3.  **Divide into simple shapes:** Break the composite figure/solid into standard shapes for which you know the centroid/CG.
4.  **Create a table:** Organize the data for each simple shape:
    * Shape number
    * Area ($A_i$) or Volume ($V_i$)
    * Centroid coordinates ($x_i, y_i$) or ($x_i, y_i, z_i$) from the reference axis
    * $A_i x_i$ (or $V_i x_i$), $A_i y_i$ (or $V_i y_i$), etc.
5.  **Sum the columns:** Find $\sum A_i$ (or $\sum V_i$), $\sum (A_i x_i)$, $\sum (A_i y_i)$, etc.
6.  **Calculate $\bar{X}$ and $\bar{Y}$ (and $\bar{Z}$ for 3D):** Use the summation formulas.

Understanding centroids and centers of gravity is foundational for many subsequent topics in engineering, particularly in solid mechanics and structural design.
### 1.1 Centroid of Basic Geometrical Plane Figures

The location of the centroid $(\bar{x}, \bar{y})$ for common two-dimensional shapes, often measured from a chosen origin (like a bottom-left corner or the center), is as follows:

| Shape         | Dimensions                 | Centroid Coordinates $(\bar{x}, \bar{y})$                     |
|---------------|----------------------------|-----------------------------------------------------------------|
| **Square**    | Side = $l$                 | $\bar{x} = \frac{l}{2}, \quad \bar{y} = \frac{l}{2}$          |
| **Rectangle** | Length = $l$, Width = $b$  | $\bar{x} = \frac{l}{2}, \quad \bar{y} = \frac{b}{2}$          |
| **Triangle**  | Base = $b$, Height = $h$   | $\bar{x} = \frac{b}{3}, \quad \bar{y} = \frac{h}{3}$          |
| **Circle**    | Radius = $r$               | $\bar{x} = 0, \quad \bar{y} = 0$                              |
| **Semi-circle** | Radius = $r$             | $\bar{x} = 0, \quad \bar{y} = \frac{4r}{3\pi}$                |
| **Quarter circle** | Radius = $r$           | $\bar{x} = \frac{4r}{3\pi}, \quad \bar{y} = \frac{4r}{3\pi}$  |

*Note: For the circle, semi-circle, and quarter circle, coordinates are typically relative to their geometric center or the corner where the straight edges meet, respectively. For instance, for a semi-circle, $\bar{x}=0$ is along the axis of symmetry from the center of the diameter.*

### 1.2 Centroid of Composite Figures

When dealing with complex plane figures that can be divided into simpler shapes (up to three as specified), we calculate the overall centroid by using the **principle of moments**. This means summing the moments of individual areas about the chosen axes and dividing by the total area.

Let $A_i$ be the area of the $i$-th simple shape, and $(x_i, y_i)$ be the centroid coordinates of that shape (measured from a common reference origin). The total area is $A = A_1 + A_2 + A_3$.

The composite centroid coordinates $(\bar{x}, \bar{y})$ are given by:

$$
\boxed{
\bar{x} = \frac{A_1 x_1 + A_2 x_2 + A_3 x_3}{A_1 + A_2 + A_3}
}
$$

$$
\boxed{
\bar{y} = \frac{A_1 y_1 + A_2 y_2 + A_3 y_3}{A_1 + A_2 + A_3}
}
$$

---

## 2. Centre of Gravity (C.G.)

### Definition:
The **centre of gravity (C.G.)** is the single point within a body where its entire weight can be considered to act. If the body were suspended from this point, it would remain in equilibrium regardless of its orientation.

* For bodies made of **uniform material**, the centre of gravity coincides exactly with the **centroid** (geometric center).
* For **non-uniform bodies**, where the material density varies, the centre of gravity's position depends on the distribution of weight throughout the body and may not coincide with its geometric center.

### 2.1 Centre of Gravity of Simple Solids

The coordinates of the centre of gravity $(\bar{x}, \bar{y}, \bar{z})$ for basic three-dimensional solids are:

| Solid        | Dimensions                     | Coordinates of Centre of Gravity $(\bar{x}, \bar{y}, \bar{z})$ |
|--------------|--------------------------------|--------------------------------------------------------------------|
| **Cube**     | Side = $a$                     | $\bar{x} = \frac{a}{2}, \quad \bar{y} = \frac{a}{2}, \quad \bar{z} = \frac{a}{2}$ |
| **Cuboid**   | Length = $l$, Width = $b$, Height = $h$ | $\bar{x} = \frac{l}{2}, \quad \bar{y} = \frac{b}{2}, \quad \bar{z} = \frac{h}{2}$ |
| **Cone**     | Radius = $r$, Height = $h$     | $\bar{x} = 0, \quad \bar{y} = 0, \quad \bar{z} = \frac{h}{4}$   |
| **Cylinder** | Radius = $r$, Height = $h$     | $\bar{x} = 0, \quad \bar{y} = 0, \quad \bar{z} = \frac{h}{2}$   |
| **Sphere**   | Radius = $r$                   | $\bar{x} = 0, \quad \bar{y} = 0, \quad \bar{z} = 0$             |
| **Hemisphere** | Radius = $r$                 | $\bar{x} = 0, \quad \bar{y} = 0, \quad \bar{z} = \frac{3r}{8}$  |

*Note: For cones, cylinders, and hemispheres, the coordinates are generally given relative to the center of their base and along their axis of symmetry.*

### 2.2 Centre of Gravity of Composite Solids

For composite solids formed by combining not more than two simple solids, we calculate the overall C.G. using the principle of moments with respect to their individual weights.

- Let $W_1$ and $W_2$ be the weights of the two simple solids.
- Let $(x_1, y_1, z_1)$ and $(x_2, y_2, z_2)$ be their respective centre of gravity coordinates (measured from a common reference origin).
- The total weight is $W = W_1 + W_2$.

The coordinates of the composite C.G. $(\bar{x}, \bar{y}, \bar{z})$ are:

$$
\boxed{
\bar{x} = \frac{W_1 x_1 + W_2 x_2}{W_1 + W_2}
}
$$

$$
\boxed{
\bar{y} = \frac{W_1 y_1 + W_2 y_2}{W_1 + W_2}
}
$$

$$
\boxed{
\bar{z} = \frac{W_1 z_1 + W_2 z_2}{W_1 + W_2}
}
$$

