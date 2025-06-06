Let's explore UNIT VI: Transformers and Machines, covering their construction, principles, and key equations.

---

## UNIT VI: Transformers and Machines

This unit covers two fundamental types of electrical devices: transformers, which efficiently transfer AC electrical energy between circuits, and electric motors, which convert electrical energy into mechanical energy.

### I. Transformers

A transformer is a static device that transfers electrical energy from one AC circuit to another at the same frequency but usually with a different voltage and current. It operates on the principle of electromagnetic induction.

#### A. General Construction

* **Core:** Made of laminated sheets of silicon steel (ferromagnetic material). The laminations are insulated from each other to reduce eddy current losses. The core provides a low-reluctance path for the magnetic flux. Common core types:
    * **Core-type:** Windings surround the core.
    * **Shell-type:** Core surrounds the windings.
* **Windings:** Two or more coils of insulated wire wound around the core.
    * **Primary Winding:** Connected to the input AC voltage source.
    * **Secondary Winding:** Connected to the load. The voltage and current in the secondary winding are transformed relative to the primary.
* **Insulation:** Essential to prevent short circuits between windings and between windings and the core. Materials include varnish, paper, and oil.
* **Cooling System:** For larger transformers, cooling is crucial to dissipate heat generated due to core losses and copper losses. Methods include:
    * Air cooling (natural or forced).
    * Oil cooling (with or without forced circulation and radiators).

#### B. Principle of Operation

* **Electromagnetic Induction:** A changing alternating current in the primary winding creates a time-varying magnetic flux in the core. This changing flux links with both the primary and secondary windings.
* **Faraday's Law:** The changing magnetic flux induces an EMF (voltage) in both windings. The magnitude of the induced EMF is proportional to the rate of change of flux linkage and the number of turns in the winding.
* **Voltage Transformation:** The ratio of the number of turns in the secondary winding ($N_s$) to the number of turns in the primary winding ($N_p$) determines the voltage transformation ratio.
    * **Step-up Transformer:** $N_s > N_p$ (secondary voltage is higher).
    * **Step-down Transformer:** $N_s < N_p$ (secondary voltage is lower).

#### C. Different Types of Transformers

1.  **Power Transformers:** Used in power transmission and distribution systems. Typically large and operate at high voltages.
2.  **Distribution Transformers:** Step down the voltage from the transmission level to the distribution level (e.g., from 11kV to 400V/230V).
3.  **Instrument Transformers:** Used to measure high voltages and currents safely.
    * **Current Transformers (CTs):** Step down the current.
    * **Potential Transformers (PTs) or Voltage Transformers (VTs):** Step down the voltage.
4.  **Audio Transformers:** Used in audio circuits for impedance matching and isolation.
5.  **Isolation Transformers:** Provide electrical isolation between circuits, often with a 1:1 turns ratio.
6.  **Autotransformers:** Have a single winding with a tap. Part of the winding is common to both the primary and secondary circuits.

#### D. EMF Equation and Transformation Ratio

* **EMF Equation:**
    * $E_p = 4.44 f N_p \Phi_m$ (Induced EMF in the primary winding)
    * $E_s = 4.44 f N_s \Phi_m$ (Induced EMF in the secondary winding)
        * Where:
            * $E_p$, $E_s$ are the RMS values of the induced EMFs.
            * $f$ is the frequency of the AC supply.
            * $N_p$, $N_s$ are the number of turns in the primary and secondary windings, respectively.
            * $\Phi_m$ is the maximum value of the magnetic flux in the core.
* **Transformation Ratio (Voltage Ratio), K:**
    * $K = \frac{N_s}{N_p} = \frac{E_s}{E_p} \approx \frac{V_s}{V_p}$ (Under ideal conditions, neglecting voltage drops due to winding impedance)
        * Where:
            * $V_p$, $V_s$ are the primary and secondary voltages, respectively.
* **Current Ratio (Ideal Transformer):**
    * $I_p V_p = I_s V_s$ (Assuming no power loss)
    * $\frac{I_p}{I_s} = \frac{V_s}{V_p} = \frac{N_s}{N_p} = K$
        * $I_p = K I_s$

#### E. Autotransformers

* **Construction:** A single winding is used, and a tap is taken off at the appropriate point to obtain the desired secondary voltage. Part of the winding is common to both the primary and secondary circuits.
* **Advantages:**
    * Smaller, lighter, and cheaper than two-winding transformers of the same rating.
    * Higher efficiency (less copper and core material).
    * Better voltage regulation.
* **Disadvantages:**
    * No electrical isolation between the primary and secondary circuits.
    * Limited applications (typically for smaller voltage changes).
* **Applications:**
    * Starters for induction motors.
    * Variable AC voltage supplies.
    * High-voltage transmission systems (for small voltage adjustments).

### II. Motors

An electric motor is a machine that converts electrical energy into mechanical energy.

#### A. Construction and Working Principle of Motors

1.  **DC Motors:**

    * **Construction:**
        * **Stator:** Stationary part, typically containing field windings (electromagnets) or permanent magnets.
        * **Rotor (Armature):** Rotating part, containing armature windings.
        * **Commutator:** A segmented ring that reverses the current direction in the armature windings as the rotor rotates.
        * **Brushes:** Stationary contacts that make electrical connection to the commutator.
    * **Working Principle:**
        * A current-carrying conductor placed in a magnetic field experiences a force (Lorentz force).
        * The armature windings are placed in the magnetic field produced by the field windings or permanent magnets.
        * The commutator and brushes ensure that the current direction in the armature conductors under the magnetic poles is always such that the force produces a torque in the same direction, causing continuous rotation.
        * The torque is proportional to the magnetic field strength and the armature current.

2.  **AC Induction Motors:**

    * **Construction:**
        * **Stator:** Contains three-phase windings. When energized with three-phase AC, these windings produce a rotating magnetic field.
        * **Rotor:** Two main types:
            * **Squirrel-cage Rotor:** Consists of conducting bars short-circuited at both ends.
            * **Wound Rotor:** Has three-phase windings connected to slip rings.
    * **Working Principle:**
        * The rotating magnetic field produced by the stator windings induces a voltage in the rotor conductors (Faraday's Law).
        * This induced voltage causes current to flow in the rotor conductors.
        * The interaction between the rotor current and the stator's rotating magnetic field produces a torque, causing the rotor to rotate.
        * The rotor rotates at a speed slightly less than the synchronous speed of the rotating magnetic field. This difference in speed is called **slip**.

3.  **Synchronous Motors:**

    * **Construction:**
        * **Stator:** Similar to an induction motor, with three-phase windings to produce a rotating magnetic field.
        * **Rotor:** Contains field windings excited by DC.
    * **Working Principle:**
        * The stator windings produce a rotating magnetic field.
        * The rotor's DC field "locks" onto the rotating magnetic field, and the rotor rotates at the **synchronous speed** (the same speed as the rotating magnetic field).
        * Synchronous motors require an auxiliary starting method (e.g., using damper windings).

#### B. Basic Equations and Characteristics of Motors

1.  **DC Motors:**

    * **EMF Equation:** $E_b = K \Phi \omega$
        * Where:
            * $E_b$ is the back EMF (voltage induced in the armature due to its rotation).
            * $K$ is a constant depending on the motor's construction.
            * $\Phi$ is the magnetic flux per pole.
            * $\omega$ is the angular speed of the rotor (rad/s).
    * **Torque Equation:** $T = K \Phi I_a$
        * Where:
            * $T$ is the torque developed by the motor.
            * $I_a$ is the armature current.
    * **Speed Equation:** $N = \frac{V - I_a R_a}{K \Phi}$
        * Where:
            * $N$ is the speed in RPM.
            * $V$ is the applied voltage.
            * $R_a$ is the armature resistance.
    * **Characteristics:**
        * **Torque-Speed Characteristic:**
            * **Series Motor:** High starting torque, speed decreases significantly with increasing load.
            * **Shunt Motor:** Relatively constant speed, torque increases linearly with armature current.
        * **Applications:**
            * **Series Motors:** High starting torque applications (e.g., traction, cranes).
            * **Shunt Motors:** Constant speed applications (e.g., lathes, pumps).

2.  **AC Induction Motors:**

    * **Synchronous Speed ($N_s$):** $N_s = \frac{120f}{P}$
        * Where:
            * $f$ is the supply frequency (Hz).
            * $P$ is the number of poles.
    * **Slip (s):** $s = \frac{N_s - N_r}{N_s}$
        * Where $N_r$ is the rotor speed.
    * **Rotor Frequency ($f_r$):** $f_r = s f$
    * **Torque Equation:** $T \propto \frac{s V^2 R_2}{R_2^2 + (sX_2)^2}$ (Simplified)
        * Where $R_2$ and $X_2$ are the rotor resistance and reactance, respectively.
    * **Characteristics:**
        * Torque is zero at synchronous speed.
        * Torque increases with slip, reaching a maximum value (breakdown torque) and then decreases.
        * Squirrel-cage motors have simple construction but lower starting torque.
        * Wound-rotor motors have higher starting torque but are more complex.
    * **Applications:** Widely used in industrial drives, pumps, fans, compressors.

3.  **Synchronous Motors:**

    * **Speed:** Constant and equal to synchronous speed ($N_s = \frac{120f}{P}$).
    * **Torque:** Can deliver constant torque at synchronous speed.
    * **Power Factor Control:** Can operate at leading, lagging, or unity power factor by adjusting the field excitation.
    * **Applications:**
        * High-precision constant-speed drives.
        * Power factor correction.
        * Generators (alternators).

---
This comprehensive overview covers the construction, working principles, and key equations for both transformers and various types of electric motors, as outlined in Unit VI.
