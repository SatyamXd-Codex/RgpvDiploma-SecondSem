# Unit V: Simple Lifting Machines

This unit explores the fundamental principles of simple lifting machines, which are devices designed to overcome a large load by applying a relatively small effort. These machines facilitate work by changing the magnitude or direction of a force.

---

## 1. Introduction to Simple Lifting Machines

A **simple lifting machine** is a device that transfers an applied force (effort) to another point to overcome a resistance (load). They are used to multiply force or to change the direction of force, making it easier to perform tasks that would otherwise be difficult or impossible.

* **Load (W):** The resistance that the machine has to overcome. It is the weight or force that needs to be lifted or moved. Measured in Newtons (N) or kilonewtons (kN).
* **Effort (P):** The force applied to the machine to overcome the load. Measured in Newtons (N) or kilonewtons (kN).

### 1.1 Mechanical Advantage (MA)

**Mechanical Advantage** is the ratio of the load lifted to the effort applied. It quantifies how much a machine multiplies the applied force.

$$
\boxed{
\text{MA} = \frac{\text{Load (W)}}{\text{Effort (P)}}
}
$$

* **Applications and Advantages of High MA:**
    * **Lifting Heavy Objects:** Machines like cranes, jacks, and pulley systems are designed to lift very heavy loads with comparatively small human or engine effort.
    * **Reduced Human Effort:** Makes tasks less physically demanding and safer.
    * **Increased Force:** Allows for the application of forces greater than what a human or a single motor could produce directly.
    * **Direction Change:** Can change the direction of force, e.g., pulling down on a rope to lift something up.

### 1.2 Velocity Ratio (VR)

**Velocity Ratio (or Theoretical Mechanical Advantage)** is the ratio of the distance moved by the effort to the distance moved by the load in the same time. It is a theoretical value that depends only on the geometry and configuration of the machine, not on the forces involved or friction.

$$
\boxed{
\text{VR} = \frac{\text{Distance moved by Effort }(d_P)}{\text{Distance moved by Load }(d_W)}
}
$$

* **Important Point:** For an ideal machine (no friction), Mechanical Advantage would be equal to Velocity Ratio.

### 1.3 Efficiency of Machines ($\eta$)

**Efficiency** is the ratio of the output work (work done on the load) to the input work (work done by the effort). It indicates how much of the input energy is converted into useful output work, considering losses due to friction.

$$
\boxed{
\text{Efficiency }(\eta) = \frac{\text{Work Output}}{\text{Work Input}} = \frac{\text{Load} \times \text{Distance moved by Load}}{\text{Effort} \times \text{Distance moved by Effort}}
}
$$

Substituting MA and VR:

$$
\boxed{
\eta = \frac{(\text{Load} / \text{Effort})}{(\text{Distance moved by Effort} / \text{Distance moved by Load})} = \frac{\text{MA}}{\text{VR}}
}
$$

* Efficiency is always less than 1 (or 100%) for real machines because some energy is always lost to friction, sound, or heat.
* **Important Point:** Efficiency helps in selecting machines for specific tasks, as higher efficiency means less effort is wasted.

### 1.4 Law of Machine

The **Law of Machine** is an empirical linear relationship between the effort (P) required to lift a given load (W) for a particular machine. It accounts for the friction present in the machine. It is typically determined experimentally by plotting a graph of effort versus load.

The general form of the law of machine is:

$$
\boxed{
P = mW + C
}
$$

Where:
* $P$ = Effort applied
* $W$ = Load lifted
* $m$ = A constant representing the slope of the P-W graph. It relates to the mechanical advantage of the frictionless parts.
* $C$ = A constant representing the effort required to overcome friction when no load is being lifted (i.e., the effort needed to run the machine itself). This is often called "friction effort at no load."

* **Important Point:** This law is specific to a given machine and helps predict its performance under varying loads.

---

## 2. Ideal Machine and Friction

### 2.1 Ideal Machine

An **ideal machine** is a theoretical machine where there are no energy losses due to friction. In such a machine:

* **Efficiency ($\eta$) = 1 (or 100%)**
* **Mechanical Advantage (MA) = Velocity Ratio (VR)**
* **Work Output = Work Input**

* **Important Point:** Ideal machines do not exist in reality but serve as a benchmark to assess the performance of real machines and simplify initial design calculations.

### 2.2 Friction in Machine

**Friction** is the resistance to motion when two surfaces are in contact. In any real machine, friction is always present in its moving parts (bearings, gears, sliding surfaces).

* **Effect of Friction:**
    * It reduces the output work (work done on load) for a given input work (work done by effort).
    * It causes energy loss, primarily as heat.
    * It requires additional effort to overcome, meaning the actual MA is always less than the theoretical VR.
* **Effort lost in Friction ($P_f$):**
    * $P_f = P - P_{ideal}$, where $P_{ideal} = W / \text{VR}$.
    * Alternatively, the load that can be lifted by the ideal machine for effort P is $W_{ideal} = P \times \text{VR}$.
    * Load lost due to friction is $W_f = W_{ideal} - W = (P \times \text{VR}) - W$.

### 2.3 Maximum Mechanical Advantage and Efficiency

Since friction is always present, as the load increases, the effort also increases (as per the law of machine).

* **Maximum Mechanical Advantage:** The MA of a machine typically increases with the load, reaching a maximum value before the machine's components might deform or fail. This maximum MA is usually found at the highest permissible load for the machine.
* **Maximum Efficiency:** Similarly, efficiency tends to increase with the load up to a certain point. This is because the "no-load" friction (constant $C$ in the law of machine) becomes a smaller proportion of the total effort at higher loads. Maximum efficiency occurs when the load is such that the ratio of useful work to total work is maximized.
    * The maximum efficiency for a machine following $P = mW + C$ is given by $\eta_{max} = \frac{1}{m \cdot \text{VR}}$.

* **Important Point:** Designers aim to minimize friction to achieve higher MA and efficiency, but eliminating it entirely is impossible.

### 2.4 Reversible and Non-Reversible Machines

A machine is classified based on whether the load can move itself (run backward) when the effort is removed.

* **Reversible Machine (or Overhauling Machine):**
    * A machine is reversible if the load can cause the effort to move in the reverse direction when the effort is removed (i.e., the machine can run backward due to the load's weight).
    * **Condition for Reversibility:** Efficiency ($\eta$) > 0.5 (or 50%).
    * This implies that the work done by the load in moving backward is greater than the work lost due to friction.
    * Example: A simple pulley system where the load can fall if released.

* **Non-Reversible Machine (or Self-locking Machine):**
    * A machine is non-reversible (or self-locking) if the load cannot move in the reverse direction on its own when the effort is removed. It stays in position even if the effort is taken off.
    * **Condition for Non-Reversibility:** Efficiency ($\eta$) $\le$ 0.5 (or 50%).
    * This implies that the work done by the load in moving backward is less than or equal to the work lost due to friction. The friction is sufficient to hold the load in place.
    * Example: A screw jack, worm and worm wheel, where friction inherently prevents the load from unwinding.

* **Important Point:** For lifting devices, self-locking is a desirable feature for safety, as it prevents the load from suddenly falling down when the effort is released.

---

## 3. Velocity Ratios of Specific Simple Lifting Machines

The Velocity Ratio (VR) is a geometric property and can be calculated by analyzing the kinematics of the machine.

### 3.1 Simple Axle and Wheel

In a simple axle and wheel, effort is applied to the circumference of the larger wheel, and the load is attached to the circumference of the smaller axle.

* Let $D$ = Diameter of the wheel (where effort is applied)
* Let $d$ = Diameter of the axle (where load is attached)

When the wheel completes one revolution, the effort moves a distance equal to the circumference of the wheel ($\pi D$), and the load moves a distance equal to the circumference of the axle ($\pi d$).

$$
\boxed{
\text{VR} = \frac{\pi D}{\pi d} = \frac{D}{d}
}
$$

### 3.2 Differential Axle and Wheel

This machine uses two axles of slightly different diameters. The effort is applied to a wheel, and a rope wound around both axles lifts the load. A single rope is wound in one direction around the larger axle and in the opposite direction around the smaller axle, with the load attached to a pulley suspended from the loop of the rope.

* Let $D$ = Diameter of the wheel
* Let $d_1$ = Diameter of the larger axle
* Let $d_2$ = Diameter of the smaller axle

When the wheel completes one revolution:
* Effort moves $\pi D$.
* The rope unwinds from $d_2$ and winds onto $d_1$. The net change in rope length supporting the load is $\pi d_1 - \pi d_2$.
* Since the load is supported by a pulley, the load moves half of this net change.

$$
\boxed{
\text{VR} = \frac{\pi D}{\frac{1}{2}(\pi d_1 - \pi d_2)} = \frac{2D}{d_1 - d_2}
}
$$

### 3.3 Worm and Worm Wheel

A worm and worm wheel consists of a worm (a screw-like threaded shaft) that meshes with a worm wheel (a gear). Effort is applied to the handle of the worm.

* Let $L$ = Length of the effort handle (radius of the circle traced by effort)
* Let $T$ = Number of teeth on the worm wheel

When the effort handle completes one revolution, the effort moves $2\pi L$.
For each revolution of the worm, the worm wheel moves by one tooth (assuming a single-start worm).
To make the worm wheel complete one revolution, the worm must rotate $T$ times.
If the load is on an axle of radius $r_W$ (or $D_W$ diameter) connected to the worm wheel, then:

$$
\boxed{
\text{VR} = \frac{\text{Distance moved by Effort}}{\text{Distance moved by Load}} = \frac{2\pi L}{\text{Circumference of load axle} / T} = \frac{2\pi L}{2\pi r_W / T} \text{ (if load on axle)}
}
$$
More commonly, it's defined without the load axle:
If $L$ is the radius of the effort wheel/handle, and $T$ is the number of teeth on the worm wheel.
For one rotation of the effort handle, the effort moves $2\pi L$.
For one rotation of the worm, one tooth of the worm wheel advances. So, to make the worm wheel rotate once, the worm must rotate $T$ times.
If the load is lifted by a rope wound on the load drum of diameter $d_L$ attached to the worm wheel.
Distance moved by load in one revolution of worm wheel = $\pi d_L$.

So, for $T$ revolutions of worm:
Effort distance = $T \times 2\pi L$
Load distance = $\pi d_L$

$$
\boxed{
\text{VR} = \frac{T \times 2\pi L}{\pi d_L} = \frac{2TL}{d_L}
}
$$
If only the worm and worm wheel are considered, and the load is implicitly linked to the worm wheel rotation (e.g., through a drum of radius $r_L$):
For one revolution of the effort wheel/handle of radius $R$: effort moves $2\pi R$.
This causes the worm wheel to rotate by $1/T$ of a revolution (for a single-start worm).
If a drum of radius $r_L$ is attached to the worm wheel, the load moves $2\pi r_L / T$.
So, $\text{VR} = \frac{2\pi R}{2\pi r_L / T} = \frac{RT}{r_L}$. This is a common form.

A simplified VR often refers to the gear ratio for the worm and wheel itself, relating input turns to output turns:
**VR = Number of teeth on worm wheel ($T$)** (for single start worm if load is directly related to worm wheel rotation).

### 3.4 Single Purchase Crab Winch

In a single purchase crab winch, a handle with effort is connected to a pinion, which then meshes with a large gear (wheel), and the load drum is fixed to the gear.

* Let $L$ = Length of the effort handle
* Let $T_1$ = Number of teeth on the gear (large wheel)
* Let $t_1$ = Number of teeth on the pinion (small gear driven by handle)
* Let $d$ = Diameter of the load drum

When the effort handle completes one revolution, the effort moves $2\pi L$.
Number of revolutions of the gear for one revolution of pinion = $t_1 / T_1$.
Distance moved by load in one revolution of gear = $\pi d$.

For one revolution of the effort handle:
Load drum rotates by $t_1 / T_1$ revolutions.
Distance moved by load = $\pi d \times (t_1 / T_1)$.

$$
\boxed{
\text{VR} = \frac{2\pi L}{\pi d \times (t_1 / T_1)} = \frac{2L T_1}{d t_1}
}
$$

### 3.5 Double Purchase Crab Winch

A double purchase crab winch has an additional set of gears, providing a higher VR. The handle drives a pinion, which meshes with a first gear. A second pinion (on the same shaft as the first gear) meshes with a second gear, and the load drum is fixed to this second gear.

* Let $L$ = Length of the effort handle
* Let $T_1$ = Number of teeth on the first gear
* Let $t_1$ = Number of teeth on the first pinion (driven by handle)
* Let $T_2$ = Number of teeth on the second gear
* Let $t_2$ = Number of teeth on the second pinion (on same shaft as $T_1$)
* Let $d$ = Diameter of the load drum

When the effort handle completes one revolution, the effort moves $2\pi L$.
Revolutions of $T_1$ (and $t_2$) = $t_1 / T_1$.
Revolutions of $T_2$ (and load drum) = (Revs of $t_2$) $\times (t_2 / T_2) = (t_1 / T_1) \times (t_2 / T_2)$.
Distance moved by load = $\pi d \times (t_1 / T_1) \times (t_2 / T_2)$.

$$
\boxed{
\text{VR} = \frac{2\pi L}{\pi d \times (t_1 / T_1) \times (t_2 / T_2)} = \frac{2L T_1 T_2}{d t_1 t_2}
}
$$

### 3.6 Simple Screw Jack

A simple screw jack uses the principle of an inclined plane wrapped around a cylinder (a screw thread) to lift a load. Effort is applied at the end of a long handle.

* Let $L$ = Length of the effort handle (radius of the circle traced by effort)
* Let $p$ = Pitch of the screw (axial distance the screw advances in one full revolution)

When the effort handle completes one revolution, the effort moves $2\pi L$.
In one revolution, the load moves a distance equal to the pitch of the screw, $p$.

$$
\boxed{
\text{VR} = \frac{2\pi L}{p}
}
$$

* **Important Point:** Screw jacks are typically self-locking due to their high friction, making them non-reversible ($\eta \le 50\%$).

### 3.7 Weston’s Differential Pulley Block

This machine uses two coaxial pulleys of slightly different diameters in the upper block and a single movable pulley in the lower block where the load is suspended. A continuous chain runs over the pulleys.

* Let $D$ = Diameter of the larger upper pulley
* Let $d$ = Diameter of the smaller upper pulley

When the larger upper pulley completes one revolution:
* Effort applied to the chain moving over the larger pulley moves $\pi D$.
* The chain winds onto the larger pulley ($\pi D$) and unwinds from the smaller pulley ($\pi d$).
* The net length of chain shortened is $\pi D - \pi d$.
* Since the load is supported by the loop of chain passing around the movable pulley, the load moves half of this net change.

$$
\boxed{
\text{VR} = \frac{\pi D}{\frac{1}{2}(\pi D - \pi d)} = \frac{2D}{D - d}
}
$$

### 3.8 Geared Pulley Block (Chain Hoist)

A geared pulley block, also known as a chain hoist or differential hoist, incorporates a gear train within the upper block to achieve a high velocity ratio, making it easy to lift very heavy loads. The exact VR depends on the specific gear arrangement (number of teeth on various gears) and the diameters of the sprockets.

While the general formula is complex and machine-specific, the principle remains:
**VR = (Ratio of teeth of driven gears / Ratio of teeth of driving gears) x (Effort sprocket diameter / Load sprocket diameter)**

A simplified conceptual understanding for the VR in a geared pulley block is often given by:
$$
\boxed{
\text{VR} = \frac{2 \times \text{number of teeth on main gear}}{\text{number of teeth on pinion}}
}
$$
(This is a common simplification for some designs, but actual VR requires detailed gear train analysis).

The underlying concept is that multiple stages of gearing multiply the mechanical advantage, allowing a small effort to lift a very large load over a small distance.
