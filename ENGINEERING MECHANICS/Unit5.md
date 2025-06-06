

## Unit – V: Simple Lifting Machines

Simple lifting machines are devices that allow a smaller effort to lift a larger load, or to change the direction of a force. They operate on the principle of trading distance for force. This unit explores their fundamental concepts and various common types.

### I. Simple Lifting Machine, Load, Effort

* **Simple Lifting Machine:** A device that helps lift or move heavy objects by applying a relatively smaller force (effort) over a greater distance, or by changing the direction of the applied force. They achieve this by utilizing mechanical advantage.
* **Load (W):** The heavy object or resistance that needs to be lifted or overcome by the machine. It is the output force of the machine.
    * **Unit:** Newton (N) or Kilogram-force (kgf).
* **Effort (P):** The force applied to the machine to lift the load. It is the input force to the machine.
    * **Unit:** Newton (N) or Kilogram-force (kgf).

### II. Mechanical Advantage (MA)

* **Definition:** The ratio of the load lifted to the effort applied. It quantifies how much a machine multiplies the input force.
* **Formula:** $MA = \frac{\text{Load (W)}}{\text{Effort (P)}}$
* **Significance:** If MA > 1, the machine is a force multiplier (e.g., car jack). If MA < 1, it's a distance multiplier (e.g., fishing rod). If MA = 1, it only changes direction (e.g., simple pulley).
* **Applications and Advantages:** Simple lifting machines are widely used because they:
    * Reduce the effort required to move heavy objects.
    * Make otherwise impossible tasks (lifting very heavy objects) possible.
    * Change the direction of the applied force to a more convenient one.
    * Allow for controlled movement of loads.

### III. Velocity Ratio (VR)

* **Definition:** The ratio of the distance moved by the effort to the distance moved by the load in the same interval of time. It is a theoretical property of the machine, determined by its geometry, and does not account for friction.
* **Formula:** $VR = \frac{\text{Distance moved by Effort (d_E)}}{\text{Distance moved by Load (d_L)}}$
* **Significance:** VR is a constant for a given machine and represents the theoretical maximum mechanical advantage if there were no friction.

### IV. Efficiency of Machines ($\eta$)

* **Definition:** The ratio of the useful work output (work done on the load) to the total work input (work done by the effort). It indicates how effectively a machine converts input energy into useful output energy.
* **Formula:** $\eta = \frac{\text{Work Output}}{\text{Work Input}} = \frac{W \times d_L}{P \times d_E}$
* **Relationship with MA and VR:**
    * Since $MA = W/P$ and $VR = d_E/d_L$, we can rewrite efficiency as:
        $\eta = \frac{(W/P)}{(d_E/d_L)} = \frac{MA}{VR}$
* **Significance:**
    * Efficiency is always less than 1 (or 100%) in real machines due to friction and other energy losses.
    * A higher efficiency means less energy is wasted.

### V. Law of Machine

* **Definition:** An empirical linear relationship between the effort applied (P) and the load lifted (W) for a given machine.
* **Formula:** $P = mW + C$
    * Where:
        * $P$ = Effort applied.
        * $W$ = Load lifted.
        * $m$ = A constant related to friction and efficiency, representing the inverse of the ideal mechanical advantage ($\frac{1}{VR} + \text{friction component}$). It is the slope of the P-W graph.
        * $C$ = A constant representing the effort required to overcome friction when no load is being lifted (the effort required to just move the machine itself without any external load). It is the intercept on the P-axis.
* **Determination:** By conducting experiments, plotting P vs. W, and finding the best-fit line.

### VI. Ideal Machine, Friction in Machine

* **Ideal Machine:**
    * **Definition:** A hypothetical machine that has no energy losses due to friction or other factors.
    * **Characteristics:**
        * Efficiency is 1 (or 100%).
        * Mechanical Advantage equals Velocity Ratio ($MA = VR$).
        * Work input equals work output.
* **Friction in Machine:**
    * **Definition:** The difference between the ideal effort (effort if no friction) and the actual effort, or the energy lost due to friction.
    * **Ideal Effort ($P_i$):** The effort required to lift a load 'W' in an ideal machine. $P_i = W / VR$.
    * **Friction in terms of Effort ($P_f$):** $P_f = P_{actual} - P_i = P - \frac{W}{VR}$
    * **Friction in terms of Load ($W_f$):** The additional load that could have been lifted if there was no friction, for the same effort. $W_f = W_{ideal} - W_{actual} = P \times VR - W$.
    * **Significance:** Friction is unavoidable in real machines and is the primary reason why actual efficiency is less than 100%. It causes energy dissipation as heat.

### VII. Maximum Mechanical Advantage and Efficiency

* **Maximum Mechanical Advantage ($MA_{max}$):**
    * From the law of machine $P = mW + C$, as the load W increases, the effort P also increases.
    * $MA = W/P = W/(mW+C)$.
    * As W becomes very large, the term C becomes negligible compared to mW, so $MA \approx W/(mW) = 1/m$.
    * Therefore, the maximum mechanical advantage approaches $1/m$.
* **Maximum Efficiency ($\eta_{max}$):**
    * $\eta = \frac{MA}{VR} = \frac{W/P}{VR} = \frac{W}{(mW+C)VR}$
    * As W becomes very large, the term C becomes negligible, and $\eta \approx \frac{W}{(mW)VR} = \frac{1}{m \times VR}$.
    * This is the highest efficiency a machine can achieve under ideal (heavy load) conditions, often called the "limiting efficiency."
* **Condition for Maximum Efficiency:** Occurs at the highest possible load the machine can lift, where the effort C (to overcome internal friction) becomes a smaller proportion of the total effort.

### VIII. Reversible and Non-Reversible Machines

* **Reversible Machine:**
    * **Definition:** A machine that can run in the reverse direction (i.e., the load can do work on the effort side) when the effort is removed.
    * **Condition for Reversibility:** Efficiency ($\eta$) must be greater than 50% (or 0.5).
    * **Explanation:** If $\eta > 0.5$, the work output is more than half the work input. This means that the work done by the load is sufficient to overcome the internal friction when the effort is removed, allowing the machine to reverse.
* **Non-Reversible (Irreversible or Self-locking) Machine:**
    * **Definition:** A machine that cannot run in the reverse direction on its own when the effort is removed. The load will remain in its position or move downwards slowly due to gravity, but the effort side will not move or contribute to the reversal.
    * **Condition for Non-Reversibility:** Efficiency ($\eta$) must be less than or equal to 50% (or 0.5).
    * **Explanation:** If $\eta \le 0.5$, the work output is less than or equal to half the work input. This means that the friction within the machine is high enough to prevent the load from driving the machine backward. The friction loss is greater than or equal to the useful work output.
    * **Significance:** Non-reversible machines are desirable in applications like screw jacks, hoists, and cranes where it's crucial for the load to remain in position when the effort is removed, preventing it from slipping back.

### IX. Velocity Ratios of Specific Simple Lifting Machines

Here are the VR calculations for various common simple lifting machines:

1.  **Simple Axle and Wheel:**
    * **Mechanism:** Effort applied at the circumference of a large wheel, load lifted by a rope wound around a smaller axle co-axial with the wheel.
    * **VR:** $VR = \frac{\text{Radius of Wheel (R)}}{\text{Radius of Axle (r)}} = \frac{\text{Diameter of Wheel (D)}}{\text{Diameter of Axle (d)}}$

2.  **Differential Axle and Wheel:**
    * **Mechanism:** Similar to simple axle and wheel, but the axle has two different diameters. A rope is wound around the larger axle and then around the smaller axle in the opposite direction, passing through a movable pulley supporting the load.
    * **VR:** $VR = \frac{2 \times \text{Radius of Wheel (R)}}{\text{Radius of larger axle (r1) - Radius of smaller axle (r2)}} = \frac{2 \times \text{Diameter of Wheel (D)}}{\text{Diameter of larger axle (d1) - Diameter of smaller axle (d2)}}$

3.  **Worm and Worm Wheel:**
    * **Mechanism:** A worm (a screw thread) meshes with a worm wheel (a gear). The effort is applied to the handle of the worm, and the load is lifted by a rope wound around the axle of the worm wheel.
    * **VR:** $VR = \frac{2\pi L \times T}{C}$ (where L is length of effort arm, T is number of teeth on worm wheel, C is circumference of load drum on worm wheel axle. A simpler approach is to consider one revolution of the worm.)
    * If $L$ is the length of the effort handle (radius of effort circle) and $T$ is the number of teeth on the worm wheel, and the load drum radius is $r$:
        * Distance moved by effort in one revolution of worm $= 2\pi L$
        * Number of teeth moved on worm wheel $= 1$ (for a single-start worm)
        * Angle rotated by worm wheel $= 1/T$ of a revolution
        * Distance moved by load $= (1/T) \times 2\pi r$
        * $VR = \frac{2\pi L}{(1/T) \times 2\pi r} = \frac{L \times T}{r}$ (Often this is expressed as $VR = \frac{\text{circumference of effort handle}}{\text{circumference of load drum per tooth of worm wheel}}$)
        * Simplified for single start worm: $VR = \frac{2\pi R_{effort}}{2\pi r_{load\_drum}/T_{teeth}} = \frac{R_{effort} \times T_{teeth}}{r_{load\_drum}}$
    * **Characteristic:** Worm and worm wheel systems are often self-locking (non-reversible) due to high friction.

4.  **Single Purchase Crab Winch:**
    * **Mechanism:** Effort applied to a handle, which turns a small gear (pinion). The pinion meshes with a larger gear (spur wheel), which is rigidly attached to the load drum.
    * **VR:** $VR = \frac{\text{Radius of effort handle (L)}}{\text{Radius of load drum (r)}} \times \frac{\text{Number of teeth on spur wheel (T)}}{\text{Number of teeth on pinion (t)}}$
    * $VR = \frac{L}{r} \times G$ (where $G = T/t$ is the gear ratio)

5.  **Double Purchase Crab Winch:**
    * **Mechanism:** Involves two sets of gears. Effort applied to a handle turning a pinion (P1). P1 meshes with a gear (G1) on a second shaft. A smaller pinion (P2) is on this second shaft and meshes with a larger gear (G2) on the load drum shaft.
    * **VR:** $VR = \frac{\text{Radius of effort handle (L)}}{\text{Radius of load drum (r)}} \times \frac{\text{Number of teeth on G1}}{\text{Number of teeth on P1}} \times \frac{\text{Number of teeth on G2}}{\text{Number of teeth on P2}}$
    * $VR = \frac{L}{r} \times G_1 \times G_2$
    * **Characteristic:** Provides a very high VR, allowing very heavy loads to be lifted with relatively small effort.

6.  **Simple Screw Jack:**
    * **Mechanism:** A screw is rotated by applying effort to a lever arm, causing a nut (or the screw itself) to move axially, lifting a load.
    * **VR:** $VR = \frac{\text{Distance moved by effort in one revolution}}{\text{Distance moved by load in one revolution}}$
        * Distance moved by effort $= 2\pi L$ (where L is the length of the lever arm)
        * Distance moved by load $= p$ (where p is the pitch of the screw, i.e., the axial distance moved for one full rotation)
    * $VR = \frac{2\pi L}{p}$
    * **Characteristic:** Often self-locking (non-reversible) due to high friction, making it suitable for holding loads in position.

7.  **Weston’s Differential Pulley Block:**
    * **Mechanism:** Consists of an upper block with two co-axial pulleys of slightly different diameters ($D_1$ and $D_2$), and a lower movable pulley. A continuous chain passes over the pulleys.
    * **VR:** $VR = \frac{2 D_1}{D_1 - D_2}$ (where $D_1$ is the diameter of the larger upper pulley, $D_2$ is the diameter of the smaller upper pulley)
    * **Characteristic:** Provides a high VR and is often self-locking.

8.  **Geared Pulley Block (or Chain Hoist):**
    * **Mechanism:** Uses a system of gears (often a worm and worm wheel or spur gears) integrated into the top block to achieve a very high VR. The chain passes over a load wheel.
    * **VR:** Depends on the specific gear ratios and pulley diameters, but it is typically a very high value.
    * **Characteristic:** Allows a very heavy load to be lifted with minimal effort. Often self-locking.

Understanding these concepts and the VR of different machines is crucial for designing and analyzing mechanical systems that involve lifting or moving loads efficiently.
