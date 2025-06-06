
## Unit – III: Friction

Friction is a ubiquitous force in engineering, simultaneously being a hindrance (causing energy loss, wear) and an essential phenomenon (enabling movement, braking, fastening). This unit delves into its nature and how it influences the equilibrium of bodies.

### I. Friction and its Relevance in Engineering

* **Friction:** A force that opposes the relative motion or tendency of motion between two surfaces in contact. It arises from the microscopic irregularities and intermolecular forces between the surfaces.
* **Relevance in Engineering:**
    * **Beneficial Aspects:**
        * **Motion:** Enables walking, driving (traction between tires and road), climbing, etc.
        * **Brakes and Clutches:** Essential for stopping vehicles and machinery, and transmitting power.
        * **Fasteners:** Holds screws, nails, and bolted joints in place.
        * **Belts and Pulleys:** Allows power transmission.
    * **Detrimental Aspects:**
        * **Energy Loss:** Dissipates energy as heat, reducing efficiency in machines.
        * **Wear and Tear:** Causes degradation of machine components, leading to maintenance and replacement costs.
        * **Noise and Vibration:** Can generate undesirable sounds and vibrations.
    * **Engineering Solutions:** Engineers constantly work to maximize beneficial friction (e.g., brake design) and minimize detrimental friction (e.g., lubrication, use of low-friction materials).

### II. Types and Laws of Friction

#### A. Types of Friction

1.  **Static Friction ($F_s$):**
    * **Definition:** The friction force that opposes the *tendency of motion* between two surfaces in contact when they are at rest relative to each other.
    * **Characteristic:** It is a variable force, increasing from zero up to a maximum value, known as **limiting friction**, just before motion begins.
2.  **Kinetic Friction (Dynamic Friction or Sliding Friction, $F_k$):**
    * **Definition:** The friction force that opposes the *actual relative motion* between two surfaces in contact when they are sliding past each other.
    * **Characteristic:** It is generally considered to be constant for a given pair of surfaces and normal force, and its magnitude is usually less than the maximum static friction (limiting friction).
3.  **Rolling Friction:**
    * **Definition:** The resistance to motion that occurs when a round object (like a wheel or ball) rolls over a surface.
    * **Characteristic:** Much smaller than sliding friction, which is why wheels are used for transport.
4.  **Fluid Friction:**
    * **Definition:** Friction between layers of a fluid in motion or between a fluid and a solid surface.
    * **Characteristic:** Depends on viscosity, speed, and contact area.

#### B. Laws of Friction (Amontons' and Coulomb's Laws)

These laws apply primarily to dry friction (static and kinetic).

1.  **Law of Static Friction:**
    * The maximum static friction ($F_{s,max}$) is directly proportional to the normal force ($N$) pressing the surfaces together.
    * The maximum static friction is independent of the apparent area of contact.
    * The maximum static friction is approximately independent of the relative speed of the surfaces (before motion starts).
2.  **Law of Kinetic Friction:**
    * The kinetic friction force ($F_k$) is directly proportional to the normal force ($N$).
    * The kinetic friction force is independent of the apparent area of contact.
    * The kinetic friction force is approximately independent of the relative speed between the surfaces, once motion has begun (at low to moderate speeds).

### III. Limiting Equilibrium, Limiting Friction, Coefficient of Friction, Angle of Friction, Angle of Repose

#### A. Limiting Equilibrium

* **Definition:** A state of equilibrium where a body is on the verge of moving, meaning the applied force is just equal to the maximum static friction (limiting friction).
* **Significance:** It's the critical point where static equilibrium transitions to impending motion.

#### B. Limiting Friction ($F_{max}$ or $F_s_{max}$)

* **Definition:** The maximum value of static friction that can be developed between two surfaces in contact before relative motion begins.
* **Formula:** $F_{max} = \mu_s N$
    * Where:
        * $F_{max}$ = Limiting friction
        * $\mu_s$ = Coefficient of static friction
        * $N$ = Normal force between the surfaces

#### C. Coefficient of Friction ($\mu$)

* **Definition:** A dimensionless constant that represents the ratio of the friction force to the normal force between two surfaces. It depends on the nature of the materials in contact and the roughness of their surfaces.
* **Types:**
    * **Coefficient of Static Friction ($\mu_s$):** Ratio of limiting static friction to the normal force.
        * $\mu_s = \frac{F_{s,max}}{N}$
    * **Coefficient of Kinetic Friction ($\mu_k$):** Ratio of kinetic friction to the normal force.
        * $\mu_k = \frac{F_k}{N}$
* **Note:** Typically, $\mu_s > \mu_k$.

#### D. Angle of Friction ($\phi$)

* **Definition:** The angle that the resultant of the normal force ($N$) and the limiting friction force ($F_{max}$) makes with the normal force when the body is on the verge of motion.
* **Relationship to Coefficient of Friction:**
    * $\tan \phi = \frac{F_{max}}{N} = \frac{\mu_s N}{N} = \mu_s$
    * Therefore, $\phi = \arctan(\mu_s)$
* **Significance:** It conceptually represents the steepest angle at which a force can be applied without causing motion, considering the friction.

#### E. Angle of Repose ($\alpha$)

* **Definition:** The maximum angle of inclination of a rough inclined plane with the horizontal at which a body placed on it will just begin to slide down by its own weight.
* **Relationship to Angle of Friction:** For a body on the verge of sliding down an inclined plane due to its own weight, the angle of repose is numerically equal to the angle of static friction.
    * $\alpha = \phi$
* **Significance:** Useful for determining the stability of granular materials (like sand, soil, grain piles).

#### F. Relation between Coefficient of Friction and Angle of Friction

As derived above:
$\mu_s = \tan \phi$

This relationship is fundamental and allows conversion between these two properties.

### IV. Equilibrium of Bodies on Level Surface

This involves analyzing the forces acting on a body on a horizontal surface, considering friction.

#### A. Subjected to Force Parallel to Plane

* **Scenario:** A block on a horizontal surface, with a horizontal pulling or pushing force (P) applied.
* **Forces:**
    * Weight (W) acting downwards.
    * Normal force (N) acting upwards (equal to W for a horizontal surface).
    * Applied horizontal force (P).
    * Friction force (F) opposing the tendency of motion.
* **Equilibrium Conditions:**
    1.  $\sum F_y = 0 \Rightarrow N - W = 0 \Rightarrow N = W$
    2.  $\sum F_x = 0$:
        * **Case 1: No motion (static equilibrium):** $P \le F_{max} = \mu_s N$. The friction force $F$ will be equal to $P$.
        * **Case 2: Impending motion (limiting equilibrium):** $P = F_{max} = \mu_s N$. The body is on the verge of moving.
        * **Case 3: Motion (kinetic friction):** $P > F_{max}$. The body moves, and the friction force $F$ becomes $F_k = \mu_k N$.
* **Problem Types:** Find maximum force before motion, find acceleration if motion occurs, find friction force for a given applied force.

#### B. Subjected to Force Inclined to Plane

* **Scenario:** A block on a horizontal surface, with a pulling or pushing force (P) applied at an angle ($\theta$) to the horizontal.
* **Forces:**
    * Weight (W) acting downwards.
    * Normal force (N) acting upwards.
    * Applied force (P) resolved into horizontal ($P_x$) and vertical ($P_y$) components.
    * Friction force (F) opposing the horizontal component of motion.
* **Equilibrium Conditions:**
    1.  **Resolve P:** $P_x = P \cos \theta$, $P_y = P \sin \theta$
    2.  $\sum F_y = 0$:
        * **If P is pulling upwards at angle $\theta$:** $N + P_y - W = 0 \Rightarrow N = W - P \sin \theta$
        * **If P is pushing downwards at angle $\theta$:** $N - P_y - W = 0 \Rightarrow N = W + P \sin \theta$
        * (Note: Normal force changes based on the vertical component of the inclined force)
    3.  $\sum F_x = 0$:
        * **Case 1: No motion:** $P_x \le F_{max} = \mu_s N$. Here $F = P_x$.
        * **Case 2: Impending motion:** $P_x = F_{max} = \mu_s N$.
        * **Case 3: Motion:** $P_x > F_{max}$. $F = F_k = \mu_k N$.
* **Problem Types:** Determine minimum force to cause motion, find optimal angle for pulling/pushing, analyze motion.

### V. Equilibrium of Bodies on Inclined Plane Subjected to Force Parallel to the Plane Only

* **Scenario:** A block resting on an inclined plane (angle $\alpha$ with the horizontal), with an external force (P) applied parallel to the inclined plane (either up or down the plane).
* **Forces (resolved along and perpendicular to the inclined plane):**
    * Weight (W) resolved into components: $W \sin \alpha$ (down the plane) and $W \cos \alpha$ (perpendicular to the plane).
    * Normal force (N) perpendicular to the plane.
    * Applied force (P) parallel to the plane.
    * Friction force (F) parallel to the plane, opposing the tendency of motion.
* **Equilibrium Conditions:**
    1.  $\sum F_{\text{perpendicular to plane}} = 0 \Rightarrow N - W \cos \alpha = 0 \Rightarrow N = W \cos \alpha$
        * (The normal force is only dependent on the weight and the plane's angle).
    2.  $\sum F_{\text{parallel to plane}} = 0$: This equation depends on the direction of impending motion and the applied force.
        * **Case 1: Body tending to slide DOWN the plane (P is acting upwards or no P, just weight component):**
            * Forces resisting downward motion: P (upwards), Friction F (upwards).
            * Force causing downward motion: $W \sin \alpha$.
            * For impending motion: $P + F_{max} = W \sin \alpha \Rightarrow P = W \sin \alpha - \mu_s N$
            * (If no P, then $F_{max} = W \sin \alpha$, which leads to $\tan \alpha = \mu_s$, i.e., angle of repose).
        * **Case 2: Body tending to slide UP the plane (P is acting upwards):**
            * Forces causing upward motion: P.
            * Forces resisting upward motion: $W \sin \alpha$ (down the plane), Friction F (down the plane).
            * For impending motion: $P = W \sin \alpha + F_{max} \Rightarrow P = W \sin \alpha + \mu_s N$
        * **Case 3: Body sliding down due to weight ($W \sin \alpha > \mu_s N$):**
            * The friction force will be kinetic friction $F_k = \mu_k N$.
            * The body will accelerate down the plane.
* **Problem Types:** Find minimum force to prevent sliding, minimum force to cause upward motion, analyze conditions for equilibrium or motion.

---
This comprehensive overview of Unit III provides a strong foundation in understanding friction, its properties, and its application in analyzing the equilibrium of bodies on both horizontal and inclined surfaces.
