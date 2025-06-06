

## UNIT I: Overview of Electronic Components & Signals

This unit introduces fundamental concepts in electronics, covering both the basic building blocks (components) and the nature of electrical quantities (signals).

### I. Passive & Active Components

Electronic components are broadly classified into two categories based on their ability to control or generate power.

#### A. Passive Components

Passive components are those that do not require an external power source to operate and cannot amplify or generate a signal. They either dissipate, store, or filter electrical energy.

##### 1. Resistances (Resistors)

* **Definition:** A resistor is a two-terminal passive electronic component that opposes the flow of electric current. It dissipates electrical energy as heat.
* **Symbol:** Usually a zig-zag line.
* **Unit:** Ohm ($\Omega$).
* **Working Principle:** Based on Ohm's Law. When a voltage is applied across a resistor, current flows through it, and energy is lost as heat due to collisions between electrons and atoms in the material.
* **Formula (Ohm's Law):**
    * $V = I \times R$
        * Where:
            * $V$ = Voltage across the resistor (Volts, V)
            * $I$ = Current flowing through the resistor (Amperes, A)
            * $R$ = Resistance (Ohms, $\Omega$)
* **Power Dissipation:**
    * $P = V \times I$
    * Substituting $V = I \times R$: $P = I^2 \times R$
    * Substituting $I = V/R$: $P = V^2 / R$
        * Where $P$ is power in Watts (W).
* **Derivation of Ohm's Law (Conceptual):** Ohm's Law is an empirical relationship. It states that for many materials (ohmic materials) at a constant temperature, the current flowing through them is directly proportional to the voltage applied across them. The constant of proportionality is the resistance.
* **Applications:** Current limiting, voltage division, pull-up/pull-down resistors in digital circuits, timing circuits (in conjunction with capacitors).

##### 2. Capacitors

* **Definition:** A capacitor is a two-terminal passive electronic component that stores electrical energy in an electric field. It consists of two conductive plates separated by a dielectric (insulating) material.
* **Symbol:** Two parallel lines.
* **Unit:** Farad (F).
* **Working Principle:** When a voltage is applied across a capacitor, charge accumulates on the plates, creating an electric field between them. The capacitor stores this charge and thus energy. It opposes sudden changes in voltage.
* **Formula (Charge Storage):**
    * $Q = C \times V$
        * Where:
            * $Q$ = Charge stored (Coulombs, C)
            * $C$ = Capacitance (Farads, F)
            * $V$ = Voltage across the capacitor (Volts, V)
* **Current-Voltage Relationship (in AC circuits):**
    * $I_c = C \frac{dV_c}{dt}$
        * This shows that the current through a capacitor is proportional to the rate of change of voltage across it. If the voltage is constant (DC), the current is zero (capacitor acts as an open circuit once charged).
* **Energy Stored:**
    * $E = \frac{1}{2} C V^2$
        * Where $E$ is energy in Joules (J).
* **Derivation (Current-Voltage Relationship):**
    * We know $Q = C \times V$.
    * Current is the rate of change of charge: $I = \frac{dQ}{dt}$.
    * Substitute $Q$: $I = \frac{d(CV)}{dt}$.
    * Assuming $C$ is constant: $I = C \frac{dV}{dt}$.
* **Applications:** Filtering (smoothing power supply ripples), coupling/decoupling signals, timing circuits, energy storage, frequency selection (in tuned circuits).

##### 3. Inductors

* **Definition:** An inductor is a two-terminal passive electronic component that stores energy in a magnetic field when electric current flows through it. It typically consists of a coil of wire.
* **Symbol:** A coil/helix.
* **Unit:** Henry (H).
* **Working Principle:** When current flows through an inductor, it creates a magnetic field. Any change in this current causes a change in the magnetic field, which in turn induces an electromotive force (EMF) that opposes the change in current (Lenz's Law). It opposes sudden changes in current.
* **Formula (Magnetic Flux Linkage):**
    * $\Phi = L \times I$
        * Where:
            * $\Phi$ = Magnetic flux linkage (Weber-turns)
            * $L$ = Inductance (Henries, H)
            * $I$ = Current flowing through the inductor (Amperes, A)
* **Voltage-Current Relationship (in AC circuits):**
    * $V_L = L \frac{dI_L}{dt}$
        * This shows that the voltage across an inductor is proportional to the rate of change of current through it. If the current is constant (DC), the voltage is zero (inductor acts as a short circuit).
* **Energy Stored:**
    * $E = \frac{1}{2} L I^2$
        * Where $E$ is energy in Joules (J).
* **Derivation (Voltage-Current Relationship):**
    * According to Faraday's Law of Induction, the induced EMF is $V = -\frac{d\Phi}{dt}$.
    * We know $\Phi = L \times I$.
    * Substitute $\Phi$: $V = -\frac{d(LI)}{dt}$.
    * Assuming $L$ is constant: $V = -L \frac{dI}{dt}$. The negative sign indicates opposition to the change in current. In circuit analysis, we often consider the magnitude of the voltage drop across it, so $V_L = L \frac{dI_L}{dt}$.
* **Applications:** Filters, chokes (to block AC while allowing DC), energy storage (in switching power supplies), resonant circuits, transformers.

#### B. Active Components

Active components are those that require an external power source to operate and can amplify or generate a signal. They exhibit control over current or voltage.

##### 1. Diodes

* **Definition:** A diode is a two-terminal semiconductor device that essentially acts as a one-way valve for current. It allows current to flow easily in one direction (forward bias) and blocks current flow in the opposite direction (reverse bias).
* **Symbol:** An arrow pointing towards a bar (anode to cathode).
* **Working Principle:** Diodes are made from p-n junctions.
    * **Forward Bias:** When the anode (p-side) is made positive with respect to the cathode (n-side), the depletion region shrinks, and current flows. There's a small voltage drop (typically 0.7V for silicon diodes, 0.3V for germanium).
    * **Reverse Bias:** When the cathode is positive with respect to the anode, the depletion region widens, and virtually no current flows (except for a very small leakage current) until the breakdown voltage is reached.
* **I-V Characteristic:** Non-linear. Exponential current increase in forward bias after the knee voltage, very little current in reverse bias until breakdown.
* **Ideal Diode Model:**
    * Forward Bias: Acts as a short circuit (0V drop).
    * Reverse Bias: Acts as an open circuit (infinite resistance).
* **Real Diode Equation (Shockley Diode Equation):**
    * $I = I_S (e^{\frac{V_D}{\eta V_T}} - 1)$
        * Where:
            * $I$ = Diode current
            * $I_S$ = Reverse saturation current (temperature dependent)
            * $V_D$ = Voltage across the diode
            * $\eta$ = Ideality factor (1 to 2, depending on the manufacturing process)
            * $V_T$ = Thermal voltage ($kT/q$, approx. 25.85 mV at room temperature)
* **Applications:** Rectification (converting AC to DC), voltage regulation (Zener diodes), signal limiting, switching, light-emitting diodes (LEDs).

##### 2. Transistors

Transistors are three-terminal semiconductor devices used for amplification or switching electronic signals and electrical power. The two main types are Bipolar Junction Transistors (BJTs) and Field-Effect Transistors (FETs).

###### a. Bipolar Junction Transistors (BJTs)

* **Definition:** A BJT is a current-controlled device. A small current at the base terminal controls a larger current flow between the collector and emitter terminals.
* **Types:** NPN and PNP.
* **Terminals:** Base (B), Collector (C), Emitter (E).
* **Working Principle:** Consists of two p-n junctions.
    * **NPN:** An n-type semiconductor between two p-type regions. Forward bias the base-emitter junction and reverse bias the collector-base junction for active region operation (amplification).
    * **PNP:** A p-type semiconductor between two n-type regions. Works similarly but with opposite voltage polarities and current directions.
* **Operating Regions:**
    * **Cut-off:** Both junctions reverse biased, no current flow (acts as an open switch).
    * **Active:** Base-emitter forward biased, collector-base reverse biased; used for amplification.
    * **Saturation:** Both junctions forward biased, maximum current flow (acts as a closed switch).
* **Current Relationships (NPN in active region):**
    * $I_E = I_B + I_C$
    * $I_C = \beta I_B$ (where $\beta$ is the current gain, typically 50-200)
    * $I_C = \alpha I_E$ (where $\alpha \approx 0.95 - 0.99$)
* **Applications:** Amplifiers, switches, oscillators, digital logic gates.

##### 3. FET (Field-Effect Transistors)

* **Definition:** FETs are voltage-controlled devices. A voltage applied to the gate terminal controls the current flow between the source and drain terminals. They have high input impedance, making them suitable for voltage amplification.
* **Types:**
    * **JFET (Junction Field-Effect Transistor):** Uses a reverse-biased p-n junction for the gate.
    * **MOSFET (Metal-Oxide-Semiconductor Field-Effect Transistor):** Uses an insulated gate, leading to even higher input impedance.

##### 4. MOS and CMOS

###### a. MOS (Metal-Oxide-Semiconductor)

* **Refers to:** The fundamental structure of MOSFETs. It describes the layers: Metal (gate electrode), Oxide (insulator, typically silicon dioxide), and Semiconductor (silicon substrate).
* **MOSFETs** are the most widely used transistors in digital and analog circuits today.
* **Types:**
    * **nMOS (n-channel MOSFET):** Current flows through an n-type channel. Requires a positive gate voltage to turn ON (for enhancement mode).
    * **pMOS (p-channel MOSFET):** Current flows through a p-type channel. Requires a negative gate voltage to turn ON (for enhancement mode).
* **Working Principle (nMOS Enhancement Mode):** Applying a positive voltage to the gate attracts electrons to the region under the gate, forming a conductive n-channel between the source and drain, allowing current to flow. No current flows when gate voltage is zero or negative.
* **Advantages:** High input impedance, good for scaling down (smaller size), low power consumption when static (especially CMOS).
* **Applications:** Amplifiers, switches, digital logic gates (especially in microprocessors, memory chips).

###### b. CMOS (Complementary Metal-Oxide-Semiconductor)

* **Definition:** A technology that uses complementary pairs of nMOS and pMOS transistors to implement logic gates and other digital circuits.
* **Working Principle:** In a CMOS circuit, when an nMOS transistor is ON, the corresponding pMOS transistor is OFF, and vice-versa. This ensures that there is never a direct path from the power supply to ground through both transistors at the same time in static operation.
* **Advantages:**
    * **Extremely Low Static Power Dissipation:** Only draws significant current during switching transitions. This is a major reason for its dominance in modern integrated circuits.
    * High noise immunity.
    * Good scalability.
* **Applications:** Virtually all modern digital integrated circuits, including microprocessors, microcontrollers, memory (RAM, ROM), digital signal processors (DSPs). It's the backbone of digital electronics.

---

### II. Signals

Electrical signals are waveforms that convey information. Understanding their characteristics is crucial for analyzing and designing electronic circuits.

#### A. DC/AC Signals

##### 1. DC (Direct Current) Signals

* **Definition:** A signal whose magnitude and direction remain constant over time.
* **Characteristics:**
    * Constant voltage (e.g., from a battery).
    * Constant current.
    * Frequency is 0 Hz.
* **Examples:** Battery voltage, output of a DC power supply.
* **Waveform:** A straight horizontal line.

##### 2. AC (Alternating Current) Signals

* **Definition:** A signal whose magnitude and direction vary periodically with time.
* **Characteristics:**
    * Periodically reverses direction.
    * Has a non-zero frequency.
* **Examples:** Household mains electricity, radio waves, audio signals.
* **Waveform:** Often sinusoidal, but can also be square, triangular, sawtooth, etc.

#### B. Voltage/Current Signals

Signals can be represented as variations in either voltage or current.

* **Voltage Signal:** Represents information by varying the potential difference across two points in a circuit. Measured in Volts (V).
* **Current Signal:** Represents information by varying the flow of charge through a point in a circuit. Measured in Amperes (A).

#### C. Periodic/Non-periodic Signals

##### 1. Periodic Signals

* **Definition:** A signal that repeats its pattern exactly after a fixed interval of time.
* **Characteristics:**
    * Has a well-defined **period (T)**: The smallest time interval after which the signal repeats itself.
    * Has a well-defined **frequency (f)**: The number of cycles per second ($f = 1/T$). Unit is Hertz (Hz).
* **Examples:** Sine wave, square wave, triangular wave.
* **Mathematical Representation:** $x(t) = x(t + nT)$ for any integer $n$.

##### 2. Non-periodic (Aperiodic) Signals

* **Definition:** A signal that does not repeat its pattern exactly after any fixed interval of time.
* **Characteristics:**
    * Does not have a defined period or fundamental frequency.
    * Their spectral content is continuous (contains a continuum of frequencies).
* **Examples:** Speech, music, random noise, a single pulse.

#### D. Average, RMS, Peak Values

These are different ways to quantify the "size" or "strength" of an AC signal.

##### 1. Peak Value ($V_P$ or $I_P$)

* **Definition:** The maximum instantaneous value of the signal from the zero level to its highest point. For a symmetrical waveform, it's the amplitude.
* **For Sine Wave:** $V(t) = V_P \sin(\omega t + \phi)$

##### 2. Peak-to-Peak Value ($V_{PP}$ or $I_{PP}$)

* **Definition:** The difference between the maximum positive peak and the maximum negative peak.
* **For Symmetrical Waveforms (like sine wave):** $V_{PP} = 2 \times V_P$

##### 3. Average Value ($V_{avg}$ or $I_{avg}$)

* **Definition:** The DC equivalent of a periodic signal. For a full cycle of a symmetrical AC waveform (like a sine wave), the average value is zero. Therefore, the average value is usually calculated over a half-cycle for such waveforms.
* **Formula (General for a function $f(t)$ over a period $T$):**
    * $V_{avg} = \frac{1}{T} \int_{t_0}^{t_0+T} V(t) dt$
* **For a Sine Wave (over a half-cycle, $0$ to $\pi$):**
    * $V_{avg} = \frac{1}{\pi} \int_{0}^{\pi} V_P \sin(\theta) d\theta = \frac{V_P}{\pi} [-\cos(\theta)]_0^{\pi} = \frac{V_P}{\pi} (-(-1) - (-1)) = \frac{2V_P}{\pi} \approx 0.637 V_P$
* **For a Full Cycle of Sine Wave:** $V_{avg} = 0$.

##### 4. RMS (Root Mean Square) Value ($V_{rms}$ or $I_{rms}$)

* **Definition:** The effective value of an AC signal, equivalent to the DC voltage or current that would produce the same amount of heat in a given resistive load. It's the most common way to specify AC voltage/current.
* **Formula (General for a function $f(t)$ over a period $T$):**
    * $V_{rms} = \sqrt{\frac{1}{T} \int_{t_0}^{t_0+T} [V(t)]^2 dt}$
* **Derivation for a Sine Wave ($V(t) = V_P \sin(\omega t)$):**
    * $V_{rms}^2 = \frac{1}{T} \int_{0}^{T} (V_P \sin(\omega t))^2 dt$
    * $V_{rms}^2 = \frac{V_P^2}{T} \int_{0}^{T} \sin^2(\omega t) dt$
    * Using the identity $\sin^2(x) = \frac{1 - \cos(2x)}{2}$:
    * $V_{rms}^2 = \frac{V_P^2}{T} \int_{0}^{T} \frac{1 - \cos(2\omega t)}{2} dt$
    * $V_{rms}^2 = \frac{V_P^2}{2T} \left[ t - \frac{\sin(2\omega t)}{2\omega} \right]_0^T$
    * Since $2\omega T = 2 (2\pi f) (1/f) = 4\pi$, $\sin(4\pi) = 0$.
    * $V_{rms}^2 = \frac{V_P^2}{2T} [T - 0] = \frac{V_P^2}{2}$
    * $V_{rms} = \sqrt{\frac{V_P^2}{2}} = \frac{V_P}{\sqrt{2}} \approx 0.707 V_P$
* **For a Sine Wave:**
    * $V_{rms} = \frac{V_P}{\sqrt{2}}$
    * $I_{rms} = \frac{I_P}{\sqrt{2}}$
* **Relation to Peak-to-Peak:** $V_{rms} = \frac{V_{PP}}{2\sqrt{2}}$

#### E. Different Types of Signal Waveforms

Besides sinusoidal, signals can have various shapes.

1.  **Sinusoidal Wave:**
    * **Formula:** $V(t) = V_P \sin(\omega t + \phi)$
    * **Description:** Smooth, continuous oscillation. Pure tone.
    * **Applications:** AC power distribution, radio frequency signals, audio signals.

2.  **Square Wave:**
    * **Description:** Alternates rapidly between two fixed voltage levels, spending equal time at each level.
    * **Characteristics:** Contains odd harmonics of the fundamental frequency.
    * **Applications:** Digital clock signals, timing circuits, switching power supplies.

3.  **Triangular Wave:**
    * **Description:** Rises linearly to a peak, then falls linearly to a trough, and repeats.
    * **Characteristics:** Contains odd harmonics, but their amplitude decreases faster than square waves.
    * **Applications:** Sweep generators (oscilloscopes), function generators, pulse width modulation (PWM).

4.  **Sawtooth Wave:**
    * **Description:** Rises linearly to a peak, then drops sharply back to the starting level, and repeats. (Or falls linearly and rises sharply).
    * **Characteristics:** Contains all harmonics (both odd and even).
    * **Applications:** Oscilloscope sweep signals, music synthesizers.

5.  **Pulse Wave:**
    * **Description:** A signal that is typically high for a short duration and then low for a longer duration (or vice versa).
    * **Characteristics:** Defined by pulse width and duty cycle.
    * **Applications:** Digital communication, radar, triggering circuits.

#### F. Ideal/Non-ideal Voltage/Current Sources

Sources provide electrical energy to a circuit. Their "ideality" describes how closely they match theoretical behavior.

##### 1. Ideal Voltage Source

* **Definition:** A theoretical two-terminal device that maintains a constant voltage across its terminals, regardless of the current drawn from it.
* **Characteristics:**
    * Zero internal resistance.
    * Provides infinite current if needed.
    * Output voltage is perfectly stable.
* **Symbol:** A circle with '+' and '-' signs, or a circle with an arrow indicating positive direction.
* **Practicality:** Cannot be perfectly realized in practice, but batteries and regulated power supplies approximate this.

##### 2. Non-ideal (Practical) Voltage Source

* **Definition:** Represents a real-world voltage source. It has a small internal resistance in series with an ideal voltage source.
* **Characteristics:**
    * Output voltage drops as more current is drawn due to the voltage drop across its internal resistance.
    * $V_{out} = V_{ideal} - I_{load} \times R_{internal}$
* **Symbol:** An ideal voltage source in series with a resistor.

##### 3. Ideal Current Source

* **Definition:** A theoretical two-terminal device that provides a constant current through its terminals, regardless of the voltage across its terminals (i.e., the load resistance).
* **Characteristics:**
    * Infinite internal resistance.
    * Can provide any voltage needed to maintain constant current.
* **Symbol:** A circle with an arrow indicating the direction of current.
* **Practicality:** Cannot be perfectly realized, but current mirrors or current regulators approximate this.

##### 4. Non-ideal (Practical) Current Source

* **Definition:** Represents a real-world current source. It has a large internal resistance in parallel with an ideal current source.
* **Characteristics:**
    * The output current will slightly decrease as the load voltage increases, due to some current flowing through its internal resistance.
    * $I_{out} = I_{ideal} - V_{load} / R_{internal}$
* **Symbol:** An ideal current source in parallel with a resistor.

#### G. Independent/Dependent Voltage/Current Sources

These describe how the source's output is determined.

##### 1. Independent Sources

* **Definition:** The voltage or current generated by the source is independent of any other voltage or current in the circuit. Their values are constant or vary with time in a predetermined way (e.g., a 5V DC source, or a 10V peak 60Hz AC source).
* **Symbol:** Circle (as described above for ideal sources).
* **Examples:** Batteries, wall outlets, function generators.

##### 2. Dependent (Controlled) Sources

* **Definition:** The voltage or current generated by the source depends on another voltage or current elsewhere in the circuit. These are models used to represent the behavior of active devices like transistors and operational amplifiers.
* **Symbol:** Diamond shape.
* **Types:**
    * **Voltage-Controlled Voltage Source (VCVS):** Output voltage is proportional to a controlling voltage. $V_{out} = k \times V_{control}$
    * **Current-Controlled Voltage Source (CCVS):** Output voltage is proportional to a controlling current. $V_{out} = k \times I_{control}$
    * **Voltage-Controlled Current Source (VCCS):** Output current is proportional to a controlling voltage. $I_{out} = k \times V_{control}$
    * **Current-Controlled Current Source (CCCS):** Output current is proportional to a controlling current. $I_{out} = k \times I_{control}$
        * Where 'k' is a constant of proportionality (gain).
* **Applications:** Used extensively in modeling transistor circuits, operational amplifier circuits, and other complex active networks in circuit analysis.
