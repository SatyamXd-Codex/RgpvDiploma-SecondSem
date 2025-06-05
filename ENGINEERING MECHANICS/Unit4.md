Certainly! I can provide the entire explanation for Unit IV: Centroid and Centre of Gravity in a single, comprehensive Markdown document.

---

# Unit IV: Centroid and Centre of Gravity

This unit delves into the fundamental concepts of **centroid** and **centre of gravity**, which are crucial for understanding the equilibrium and stability of various shapes and objects in engineering and physics.

---

## 1. Centroid

### Definition:
The **centroid** of a plane figure is its geometric center. It's the theoretical point where the entire area of the figure can be considered to be concentrated. For a uniform thin plate, the centroid coincides with its center of mass.

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

---

**Important Tip:** When solving problems, always carefully choose your origin and the directions of your coordinate axes. A wise choice can significantly simplify your calculations.

---

I hope this comprehensive Markdown explanation is exactly what you were looking for! Let me know if you have any other questions.
