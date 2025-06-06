

## Unit – II: Equilibrium

This unit focuses on the principles of equilibrium, which is a state where a body is either at rest or moving with a constant velocity. Understanding equilibrium is fundamental to designing stable structures and systems.

### I. Equilibrium and Equilibrant

* **Equilibrium:**
    * **Definition:** A state where a body is either at rest (static equilibrium) or moving with a constant velocity (dynamic equilibrium). In both cases, the net external force and the net external moment acting on the body are zero.
    * **Conditions for Equilibrium (2D Coplanar Force System):** For a body to be in equilibrium, the following conditions must be met:
        1.  **Translational Equilibrium:** The algebraic sum of all forces acting on the body in any direction must be zero.
            * $\sum F_x = 0$ (Sum of forces in the horizontal direction is zero)
            * $\sum F_y = 0$ (Sum of forces in the vertical direction is zero)
        2.  **Rotational Equilibrium:** The algebraic sum of moments of all forces about any point (or axis) must be zero.
            * $\sum M = 0$ (Sum of moments about any point is zero)
    * **Significance:** These conditions are used to find unknown forces (reactions, tensions, etc.) acting on a body in equilibrium.

* **Equilibrant:**
    * **Definition:** A single force that, when added to a system of forces, brings the system into equilibrium. It is equal in magnitude and opposite in direction to the resultant of all other forces in the system.
    * **Relationship to Resultant:** If $\vec{R}$ is the resultant of a force system, then the equilibrant is $-\vec{R}$.
    * **Application:** Useful conceptually, as it represents the single force needed to balance a given force system.

### II. Free Body and Free Body Diagram (FBD)

* **Free Body:**
    * **Definition:** An isolated body or a part of a system that is conceptually separated from all other bodies and supports.
    * **Concept:** To analyze forces acting on a specific object, we imagine it as "free" from its surroundings.

* **Free Body Diagram (FBD):**
    * **Definition:** A sketch of the free body showing all external forces and moments acting on it. These forces include applied loads, reactions from supports, weight of the body, and forces from contact with other bodies.
    * **Purpose:** The FBD is the most critical step in solving any mechanics problem. It simplifies a complex system into a manageable diagram for applying equilibrium equations.
    * **Steps to Draw an FBD:**
        1.  **Isolate the body:** Mentally separate the body from its surroundings.
        2.  **Draw the body:** Sketch the outline of the isolated body.
        3.  **Show all active forces:** Include all known applied loads, weights (acting at the center of gravity), and any forces from other bodies in contact.
        4.  **Show all reactive forces (reactions):** Replace supports with the forces they exert on the body. (Refer to "Types of Supports" below for details).
        5.  **Indicate known and unknown forces:** Clearly label magnitudes and directions. Assume directions for unknown forces; if the calculated value turns out negative, the assumed direction was opposite to the actual direction.
        6.  **Add dimensions and angles:** Include relevant geometric information.

### III. Analytical and Graphical Methods of Analysing Equilibrium

#### A. Analytical Method

* **Description:** Involves applying the algebraic equations of equilibrium ($\sum F_x = 0$, $\sum F_y = 0$, $\sum M = 0$).
* **Steps:**
    1.  Draw a clear Free Body Diagram.
    2.  Establish a coordinate system (e.g., x-y axes).
    3.  Resolve all forces into their components along the chosen axes.
    4.  Apply the equilibrium equations:
        * Sum of horizontal forces = 0
        * Sum of vertical forces = 0
        * Sum of moments about any convenient point = 0 (Choosing a point where unknown forces pass through simplifies the moment equation as their moment arm becomes zero).
    5.  Solve the resulting system of algebraic equations for the unknown forces.
* **Advantages:** Precise results, suitable for complex problems with many forces.
* **Disadvantages:** Can be mathematically intensive.

#### B. Graphical Method

* **Description:** Involves drawing the forces to scale as a force polygon. For a body in equilibrium, the force polygon must close (form a closed loop).
* **Steps (for Concurrent Force System):**
    1.  Draw a space diagram (actual arrangement of forces).
    2.  Choose a suitable scale for forces.
    3.  Draw the forces one after another, tip-to-tail, maintaining their correct magnitude and direction.
    4.  If the polygon closes (the end of the last vector meets the start of the first vector), the system is in equilibrium. If not, the vector drawn from the start of the first to the end of the last is the resultant. The equilibrant is equal and opposite to this resultant.
* **Advantages:** Provides a visual understanding, useful for checking analytical results.
* **Disadvantages:** Less precise (depends on drawing accuracy), primarily suitable for concurrent force systems or parallel force systems. More complex for general non-concurrent systems.

### IV. Lami’s Theorem

* **Statement:** If three coplanar, concurrent forces are in equilibrium, then each force is proportional to the sine of the angle between the other two forces.
* **Explanation:** Consider three forces $F_1$, $F_2$, and $F_3$ acting at a point and in equilibrium. Let $\alpha$ be the angle between $F_2$ and $F_3$, $\beta$ be the angle between $F_1$ and $F_3$, and $\gamma$ be the angle between $F_1$ and $F_2$.
    * $\frac{F_1}{\sin \alpha} = \frac{F_2}{\sin \beta} = \frac{F_3}{\sin \gamma}$
* **Derivation (Conceptual):** It can be derived from the sine rule in a force triangle. If three forces are in equilibrium, their force polygon (a triangle in this case) must close.
* **Application for various engineering problems:**
    * **Tension in cables:** Finding forces in ropes supporting a weight.
    * **Forces in simple frameworks:** Analyzing forces at joints in simple trusses.
    * **Suspension systems:** Determining forces in slings or chains.
    * **Pulley systems:** Analyzing forces involved in lifting loads.
    * **Equilibrium of inclined planes:** Finding reaction forces and tensions for objects on slopes.
* **Limitation:** Strictly applicable only to systems with exactly **three** coplanar and concurrent forces in equilibrium.

### V. Types of Beam, Supports, and Loads

#### A. Types of Beam

A beam is a structural element primarily designed to carry loads by resisting bending.

1.  **Cantilever Beam:** Fixed at one end and free at the other.
    * **Supports:** One fixed support.
2.  **Simply Supported Beam:** Supported at both ends, typically by a hinge at one end and a roller at the other.
3.  **Overhanging Beam:** A simply supported beam that extends beyond one or both of its supports.
4.  **Fixed Beam (Built-in or Encastered Beam):** Both ends are rigidly fixed, preventing rotation and translation.
5.  **Continuous Beam:** A beam supported at more than two points (multiple supports).

#### B. Types of Supports and their Reactions

Supports provide constraints that prevent motion and generate reaction forces/moments.

1.  **Simple Support (Rocker or Knife Edge):**
    * **Constraints:** Prevents vertical translation only.
    * **Reactions:** One vertical reaction force, perpendicular to the support surface. (No moment, no horizontal force).
    * **Symbol:** A triangular rocker or a knife edge.

2.  **Hinged Support (Pin Support):**
    * **Constraints:** Prevents both horizontal and vertical translation, but allows rotation.
    * **Reactions:** Two reaction forces: one horizontal and one vertical. (No moment).
    * **Symbol:** A triangle with a pin.

3.  **Roller Support:**
    * **Constraints:** Prevents vertical translation (perpendicular to the surface), but allows horizontal translation and rotation.
    * **Reactions:** One reaction force, perpendicular to the surface on which the rollers rest. (No moment, no horizontal force parallel to surface).
    * **Symbol:** A triangle on rollers.

4.  **Fixed Support (Built-in or Encastered):**
    * **Constraints:** Prevents horizontal translation, vertical translation, and rotation.
    * **Reactions:** Three reactions: one horizontal force, one vertical force, and one moment.
    * **Symbol:** A wall or block with the beam embedded.

#### C. Loads Acting on Beam

Loads are the forces or moments applied to a beam.

1.  **Vertical Point Load (Concentrated Load):**
    * **Description:** A force acting at a single point on the beam.
    * **Unit:** N or kN.
    * **Representation:** A downward arrow at the point of application.

2.  **Inclined Point Load:**
    * **Description:** A force acting at a single point, but at an angle to the beam.
    * **Analysis:** It must be resolved into its vertical and horizontal components for analysis. The vertical component contributes to bending and shear, and the horizontal component contributes to axial force and horizontal reactions.

3.  **Uniformly Distributed Load (UDL):**
    * **Description:** A load spread uniformly over a certain length of the beam, causing the same force per unit length.
    * **Unit:** N/m or kN/m.
    * **Representation:** A series of downward arrows or a rectangle representing the distributed load.
    * **Analysis:** For calculating reactions and moments, the UDL can be replaced by a single equivalent point load acting at the centroid of the distributed load (for a rectangular UDL, this is at its midpoint). The magnitude of this equivalent load is (intensity of UDL $\times$ length of UDL).

4.  **Couple (Moment Load):**
    * **Definition:** Two parallel forces of equal magnitude and opposite direction, separated by a perpendicular distance. It causes pure rotation.
    * **Unit:** N·m or kN·m.
    * **Representation:** A curved arrow indicating the direction of rotation.
    * **Analysis:** A couple has the same moment about any point in its plane. It directly adds to the moment equilibrium equation.

### VI. Beam Reaction for Cantilever, Simply Supported Beam with or without Overhang

Determining beam reactions is the first step in analyzing beams. This involves applying the equations of static equilibrium ($\sum F_x = 0$, $\sum F_y = 0$, $\sum M = 0$).

#### A. Cantilever Beam

* **Supports:** One fixed support.
* **Reactions:**
    * One vertical reaction ($R_y$).
    * One horizontal reaction ($R_x$, if there are horizontal loads).
    * One moment reaction ($M_A$).
* **Analysis:** Apply the three equilibrium equations to find the three unknowns. The horizontal reaction is zero if there are no horizontal loads. The moment reaction at the fixed end balances all moments caused by external loads.

#### B. Simply Supported Beam (without overhang)

* **Supports:** Typically one hinged support and one roller support.
* **Reactions:**
    * Hinged support: One vertical reaction ($R_{Ay}$) and one horizontal reaction ($R_{Ax}$).
    * Roller support: One vertical reaction ($R_{By}$).
* **Analysis:**
    1.  Assume directions for reactions (e.g., vertical reactions upwards).
    2.  Apply $\sum F_x = 0$ to find $R_{Ax}$ (usually zero if no horizontal loads).
    3.  Apply $\sum M = 0$ about one of the supports (e.g., point A) to eliminate one unknown vertical reaction ($R_{Ay}$) from the moment equation and solve for the other ($R_{By}$).
    4.  Apply $\sum F_y = 0$ to find the remaining vertical reaction ($R_{Ay}$).
* **Combination of Point Load and Uniformly Distributed Load (UDL):**
    * **Steps:**
        1.  Replace each UDL with its equivalent point load acting at its centroid.
        2.  Now the beam has only point loads (original and equivalent UDLs).
        3.  Proceed with the steps for point loads as above.
    * **Example Calculation:**
        * Consider a simply supported beam AB of length L. A UDL of $w$ (N/m) acts over the entire span.
        * Equivalent point load = $w \times L$, acting at L/2 from A (or B).
        * $\sum M_A = 0 \Rightarrow R_{By} \times L - (wL) \times (L/2) = 0 \Rightarrow R_{By} = wL/2$
        * $\sum F_y = 0 \Rightarrow R_{Ay} + R_{By} - wL = 0 \Rightarrow R_{Ay} = wL/2$
        * So, for a simply supported beam with UDL over full span, reactions are $wL/2$ at each end.
        * If point loads are also present, add their contributions to the moment and force sums.

#### C. Simply Supported Beam with Overhang

* **Supports:** Similar to simply supported, but part of the beam extends beyond a support.
* **Reactions:** Two reactions (one vertical at hinge, one vertical at roller) are still primary.
* **Analysis:** The same three equilibrium equations apply. The presence of an overhang means that loads on the overhang will create additional moments at the supports, which must be considered. The calculations proceed identically by taking moments about one of the supports and summing vertical forces.

### VII. Beam Reaction Graphically for Simply Supported Beam Subjected to Vertical Point Loads Only

* **Method:** This involves using the principles of graphic statics, specifically the **funicular polygon (or string polygon)** and the **force polygon**.
* **Steps:**
    1.  **Space Diagram:** Draw the beam to scale, showing supports and all vertical point loads with their positions.
    2.  **Force Diagram (Force Polygon):**
        * Choose a suitable force scale (e.g., 1 cm = 10 N).
        * Draw the load line: Draw vectors representing all vertical point loads, one after another, vertically downwards, in continuous order (e.g., from A to B). Label the spaces between forces using Bow's notation (e.g., AB, BC, CD). The total length of this line represents the sum of the loads.
        * Choose a **pole (O)**: Pick an arbitrary point 'O' anywhere, but typically to the left of the load line.
        * Draw **rays (polar lines):** Connect the pole O to each point on the load line (a, b, c, d...). These rays represent the action lines of the forces.
    3.  **Funicular Polygon (String Polygon):**
        * Draw lines parallel to the rays in the space diagram.
        * Start from a convenient point on the line of action of one support reaction (e.g., $R_A$). Draw a line parallel to the first ray (oa) until it intersects the line of action of the first load (force AB).
        * From that intersection, draw a line parallel to the second ray (ob) until it intersects the line of action of the second load (force BC), and so on.
        * The last line drawn will intersect the line of action of the last support reaction (e.g., $R_B$).
        * The line that connects the starting point on $R_A$'s line of action to the ending point on $R_B$'s line of action is called the **closing line** of the funicular polygon.
    4.  **Determine Reactions:**
        * In the force polygon, draw a line from the pole O parallel to the closing line of the funicular polygon.
        * This parallel line will divide the load line into two segments. The length of these segments, measured to the force scale, will give the magnitudes of the two support reactions ($R_A$ and $R_B$).
        * The direction of the reactions will be upwards.

* **Advantages:** Provides a visual check, good for multiple point loads, can be more intuitive for some problems.
* **Disadvantages:** Requires careful drawing and scaling, results are approximate due to drafting limitations.

---
This comprehensive breakdown covers all the topics in Unit II, providing definitions, principles, methods, and applications related to equilibrium in mechanics.
