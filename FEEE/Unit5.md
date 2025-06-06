Let's break down UNIT V: A.C. Circuits, covering the fundamental concepts, mathematical representations, and circuit analysis for alternating current systems.

---

## UNIT V: A.C. Circuits

Alternating Current (AC) circuits involve currents and voltages that vary periodically over time, typically in a sinusoidal manner. AC is widely used for power transmission and distribution due to its ease of transformation and generation.

### I. Fundamental Concepts of AC Waveforms

For a sinusoidal AC waveform, we define several key parameters:

#### A. Cycle

* **Definition:** One complete set of positive and negative values of an alternating quantity. It represents one complete repetition of the waveform.
* **Visual:** From one peak to the next peak, or one zero crossing to the next zero crossing in the same direction.

#### B. Frequency (f)

* **Definition:** The number of cycles completed by an alternating quantity per second.
* **Unit:** Hertz (Hz).
* **Significance:** Determines how rapidly the current or voltage changes direction. Standard power frequencies are 50 Hz (e.g., India, Europe) or 60 Hz (e.g., North America).

#### C. Periodic Time (T)

* **Definition:** The time taken to complete one full cycle of an alternating quantity.
* **Unit:** Seconds (s).
* **Relationship with Frequency:** $T = \frac{1}{f}$

#### D. Amplitude (Peak Value, $V_m$ or $I_m$)

* **Definition:** The maximum instantaneous value attained by an alternating quantity in one cycle. It's the peak positive or negative value from the zero level.
* **Unit:** Volts (V) for voltage, Amperes (A) for current.
* **Notation:** Often denoted as $V_m$ (for maximum voltage) or $I_m$ (for maximum current), or $V_P$, $I_P$.

#### E. Angular Velocity ($\omega$) / Angular Frequency

* **Definition:** The rate of change of the angle of the rotating phasor that represents the sinusoidal quantity. It's the angular speed in radians per second.
* **Unit:** Radians per second (rad/s).
* **Relationship with Frequency:** $\omega = 2\pi f$
* **Significance:** Used in the mathematical representation of AC waveforms.

#### F. RMS Value (Root Mean Square)

* **Definition:** The effective value of an AC quantity. It is equivalent to the DC value that would produce the same heating effect in a given resistive load.
* **Formula (for a sinusoidal waveform):**
    * $V_{rms} = \frac{V_m}{\sqrt{2}} \approx 0.707 V_m$
    * $I_{rms} = \frac{I_m}{\sqrt{2}} \approx 0.707 I_m$
* **Significance:** Most AC voltage and current ratings (e.g., 230V AC mains) are given as RMS values.

#### G. Average Value

* **Definition:** The average of all instantaneous values of an alternating quantity over one complete cycle.
* **Formula (for a full cycle of a symmetrical AC waveform like sine wave):** The average value is **zero**.
* **Formula (for half-cycle of a sinusoidal waveform):**
    * $V_{avg} = \frac{2V_m}{\pi} \approx 0.637 V_m$
    * $I_{avg} = \frac{2I_m}{\pi} \approx 0.637 I_m$
* **Significance:** Used in calculating the DC output of rectifiers.

#### H. Form Factor ($F_f$)

* **Definition:** The ratio of the RMS value to the Average value of an alternating quantity.
* **Formula:** $F_f = \frac{RMS Value}{Average Value}$
* **For a sinusoidal waveform:** $F_f = \frac{V_m/\sqrt{2}}{2V_m/\pi} = \frac{\pi}{2\sqrt{2}} \approx 1.11$
* **Significance:** Indicates the shape of the waveform. Different waveforms have different form factors.

#### I. Peak Factor (Crest Factor, $K_f$)

* **Definition:** The ratio of the Peak value to the RMS value of an alternating quantity.
* **Formula:** $K_f = \frac{Peak Value}{RMS Value}$
* **For a sinusoidal waveform:** $K_f = \frac{V_m}{V_m/\sqrt{2}} = \sqrt{2} \approx 1.414$
* **Significance:** Indicates the maximum instantaneous stress on insulation or peak current requirements.

#### J. Impedance (Z)

* **Definition:** The total opposition to the flow of alternating current in an AC circuit. It is the complex sum of resistance and reactance.
* **Unit:** Ohm ($\Omega$).
* **Components:**
    * **Resistance (R):** Opposition due to energy dissipation (heat). (Unit: $\Omega$)
    * **Reactance (X):** Opposition due to energy storage in electric or magnetic fields.
        * **Inductive Reactance ($X_L$):** Opposition offered by an inductor. $X_L = \omega L = 2\pi f L$. (Unit: $\Omega$)
        * **Capacitive Reactance ($X_C$):** Opposition offered by a capacitor. $X_C = \frac{1}{\omega C} = \frac{1}{2\pi f C}$. (Unit: $\Omega$)
* **Formula (General, for series RLC):** $Z = \sqrt{R^2 + (X_L - X_C)^2}$ (Magnitude)
* **Phasor/Complex Form:** $Z = R + jX$ (where $X = X_L - X_C$)

#### K. Phase Angle ($\phi$)

* **Definition:** The angular difference (in degrees or radians) between the voltage and current waveforms in an AC circuit.
* **Significance:** Indicates whether the current leads or lags the voltage, which is crucial for power calculations.
    * If current lags voltage: Circuit is inductive.
    * If current leads voltage: Circuit is capacitive.
    * If current is in phase with voltage: Circuit is purely resistive.
* **Formula (from impedance triangle):** $\phi = \arctan \left( \frac{X}{R} \right) = \arctan \left( \frac{X_L - X_C}{R} \right)$

#### L. Power Factor (PF)

* **Definition:** The cosine of the phase angle ($\phi$) between the voltage and current in an AC circuit. It represents the ratio of real power to apparent power.
* **Formula:** $PF = \cos(\phi)$
* **Significance:**
    * Indicates how effectively electrical power is being used.
    * A power factor of 1 (unity) means all power is real power (resistive load).
    * A power factor less than 1 means some power is reactive (inductive or capacitive load), which does no useful work.
* **Types:**
    * **Leading Power Factor:** Current leads voltage (capacitive circuit).
    * **Lagging Power Factor:** Current lags voltage (inductive circuit).
    * **Unity Power Factor:** Current and voltage are in phase (purely resistive circuit, or resonant circuit).

### II. Mathematical and Phasor Representation of Alternating EMF and Current

#### A. Mathematical Representation (Time Domain)

Sinusoidal AC quantities are typically represented as sine or cosine functions of time.

* **Voltage:** $v(t) = V_m \sin(\omega t \pm \phi_v)$ or $v(t) = V_m \cos(\omega t \pm \phi_v)$
* **Current:** $i(t) = I_m \sin(\omega t \pm \phi_i)$ or $i(t) = I_m \cos(\omega t \pm \phi_i)$
    * Where:
        * $V_m$, $I_m$ are peak voltages/currents.
        * $\omega$ is angular frequency.
        * $\phi_v$, $\phi_i$ are the phase angles (relative to a reference).
    * The phase difference between voltage and current is $\phi = \phi_v - \phi_i$.

#### B. Phasor Representation (Frequency Domain)

Phasors are rotating vectors used to represent sinusoidal quantities in the complex plane. They simplify AC circuit analysis by converting differential equations into algebraic equations.

* **Concept:** A phasor has a magnitude (RMS or peak value) and an angle (phase). It rotates counter-clockwise at angular frequency $\omega$.
* **Notation:**
    * **Polar Form:** $\mathbf{V} = V_{rms} \angle \phi_v$ or $\mathbf{I} = I_{rms} \angle \phi_i$
    * **Rectangular Form:** $\mathbf{V} = V_x + jV_y$ or $\mathbf{I} = I_x + jI_y$ (where $j = \sqrt{-1}$)
    * **Euler's Form:** $\mathbf{V} = V_{rms} e^{j\phi_v}$
* **Conversion:**
    * Polar to Rectangular: $V_x = V_{rms} \cos(\phi_v)$, $V_y = V_{rms} \sin(\phi_v)$
    * Rectangular to Polar: $V_{rms} = \sqrt{V_x^2 + V_y^2}$, $\phi_v = \arctan(V_y/V_x)$
* **Advantages:**
    * Allows algebraic addition, subtraction, multiplication, and division of sinusoidal quantities.
    * Simplifies analysis of complex AC circuits.

### III. Voltage and Current Relationship in Star and Delta Connections (Three-Phase Systems)

These connections are fundamental in three-phase AC power systems, offering advantages like efficient power transmission and constant power delivery.

#### A. Star (Y) Connection

* **Description:** Three windings (or loads) are connected such that one end of each winding is joined at a common point called the neutral point (or star point). The other three ends are connected to the three line terminals.
* **Voltage Relationships:**
    * **Line Voltage ($V_L$):** Voltage between any two line terminals.
    * **Phase Voltage ($V_{ph}$):** Voltage between a line terminal and the neutral point.
    * $V_L = \sqrt{3} V_{ph}$
    * Line voltages are 120$^\circ$ out of phase with each other. Phase voltages are also 120$^\circ$ out of phase with each other.
    * Line voltage is 30$^\circ$ ahead of its corresponding phase voltage.
* **Current Relationships:**
    * **Line Current ($I_L$):** Current flowing through the line.
    * **Phase Current ($I_{ph}$):** Current flowing through each winding/phase.
    * $I_L = I_{ph}$
* **Applications:** Power generation (alternators), distribution systems (for supplying both line-to-line and line-to-neutral loads), motors.

#### B. Delta ($\Delta$) Connection

* **Description:** The three windings (or loads) are connected end-to-end, forming a closed triangular loop. There is no neutral point.
* **Voltage Relationships:**
    * $V_L = V_{ph}$
* **Current Relationships:**
    * $I_L = \sqrt{3} I_{ph}$
    * Line current is 30$^\circ$ lagging its corresponding phase current.
* **Applications:** Power transformers, induction motors, and load connections where high line currents are required.

### IV. A.C. in Resistors, Inductors, and Capacitors (Pure Components)

#### A. A.C. in Resistors (Purely Resistive Circuit)

* **Voltage-Current Relationship:** Voltage and current are **in phase**.
* **Phasor Diagram:** Voltage and current phasors align.
* **Impedance:** $Z_R = R$ (purely real, no imaginary component)
* **Power Factor:** $PF = \cos(0^\circ) = 1$ (Unity power factor)
* **Power:** All power is consumed as real power (heat). $P = V_{rms} I_{rms} = I_{rms}^2 R = \frac{V_{rms}^2}{R}$

#### B. A.C. in Inductors (Purely Inductive Circuit)

* **Voltage-Current Relationship:** Current **lags** voltage by 90$^\circ$ ($\pi/2$ radians).
* **Phasor Diagram:** Current phasor lags voltage phasor by 90$^\circ$.
* **Impedance (Inductive Reactance):** $Z_L = jX_L = j\omega L = j2\pi f L$
* **Power Factor:** $PF = \cos(90^\circ) = 0$ (Lagging power factor)
* **Power:** Only reactive power is exchanged (stored and returned). Real power is zero.
    * $Q_L = V_{rms} I_{rms} = I_{rms}^2 X_L = \frac{V_{rms}^2}{X_L}$ (Units: VAR - Volt-Ampere Reactive)

#### C. A.C. in Capacitors (Purely Capacitive Circuit)

* **Voltage-Current Relationship:** Current **leads** voltage by 90$^\circ$ ($\pi/2$ radians).
* **Phasor Diagram:** Current phasor leads voltage phasor by 90$^\circ$.
* **Impedance (Capacitive Reactance):** $Z_C = -jX_C = -j\frac{1}{\omega C} = -j\frac{1}{2\pi f C}$
* **Power Factor:** $PF = \cos(-90^\circ) = 0$ (Leading power factor)
* **Power:** Only reactive power is exchanged (stored and returned). Real power is zero.
    * $Q_C = V_{rms} I_{rms} = I_{rms}^2 X_C = \frac{V_{rms}^2}{X_C}$ (Units: VAR)

### V. A.C. in R-L Series, R-C Series, R-L-C Series and Parallel Circuits

Analyzing these circuits involves combining resistances and reactances using complex numbers or phasor diagrams.

#### A. R-L Series Circuit

* **Components:** Resistor (R) in series with an Inductor (L).
* **Impedance:** $\mathbf{Z} = R + jX_L = R + j\omega L$
* **Magnitude of Impedance:** $|Z| = \sqrt{R^2 + X_L^2}$
* **Phase Angle:** $\phi = \arctan\left(\frac{X_L}{R}\right)$ (Current lags voltage)
* **Current:** $I = V/Z$
* **Phasor Diagram:** Voltage across R is in phase with current, voltage across L leads current by 90$^\circ$. Resultant voltage is the phasor sum.

#### B. R-C Series Circuit

* **Components:** Resistor (R) in series with a Capacitor (C).
* **Impedance:** $\mathbf{Z} = R - jX_C = R - j\frac{1}{\omega C}$
* **Magnitude of Impedance:** $|Z| = \sqrt{R^2 + X_C^2}$
* **Phase Angle:** $\phi = \arctan\left(\frac{-X_C}{R}\right) = -\arctan\left(\frac{X_C}{R}\right)$ (Current leads voltage)
* **Current:** $I = V/Z$
* **Phasor Diagram:** Voltage across R is in phase with current, voltage across C lags current by 90$^\circ$. Resultant voltage is the phasor sum.

#### C. R-L-C Series Circuit

* **Components:** Resistor (R), Inductor (L), and Capacitor (C) in series.
* **Impedance:** $\mathbf{Z} = R + j(X_L - X_C)$
* **Magnitude of Impedance:** $|Z| = \sqrt{R^2 + (X_L - X_C)^2}$
* **Phase Angle:** $\phi = \arctan\left(\frac{X_L - X_C}{R}\right)$
    * If $X_L > X_C$: Circuit is inductive, current lags.
    * If $X_C > X_L$: Circuit is capacitive, current leads.
    * If $X_L = X_C$: **Resonance** occurs. Circuit behaves purely resistively. $Z = R$, $\phi = 0^\circ$. This is a very important condition.
* **Current:** $I = V/Z$
* **Phasor Diagram:** Combined effect of inductive and capacitive reactances.

#### D. Parallel AC Circuits (e.g., R-L-C Parallel)

* **Components:** R, L, and C connected in parallel across the same voltage source.
* **Analysis Method:** Usually easier to analyze using **admittance (Y)**, which is the reciprocal of impedance ($Y = 1/Z$).
    * **Admittance:** $\mathbf{Y} = G + jB$
        * **Conductance (G):** $1/R$
        * **Susceptance (B):** $B_L = -1/X_L = -1/(\omega L)$ (inductive susceptance), $B_C = 1/X_C = \omega C$ (capacitive susceptance)
    * Total Admittance: $\mathbf{Y}_{total} = G + j(B_C - B_L)$
* **Magnitude of Admittance:** $|Y| = \sqrt{G^2 + (B_C - B_L)^2}$
* **Total Current:** $I_{total} = V \times Y_{total}$
* **Phase Angle:** $\phi_Y = \arctan\left(\frac{B_C - B_L}{G}\right)$. The phase angle of the impedance is $-\phi_Y$.
* **Resonance (Parallel):** Occurs when $B_C = B_L$. At resonance, the total current is minimum, and the impedance is maximum and purely resistive.
* **Phasor Diagram:** Current through R is in phase with voltage. Current through L lags voltage by 90$^\circ$. Current through C leads voltage by 90$^\circ$. Total current is the phasor sum.

### VI. Power in A.C. Circuits

In AC circuits, power needs to be defined more carefully than in DC circuits due to the phase difference between voltage and current.

#### A. Types of Power

1.  **Real Power (Active Power, P)**
    * **Definition:** The actual power consumed or dissipated by the circuit elements (primarily resistors) and converted into useful work (heat, light, mechanical energy).
    * **Unit:** Watt (W).
    * **Formula:** $P = V_{rms} I_{rms} \cos(\phi) = I_{rms}^2 R = \frac{V_{rms}^2}{R}$
    * **Significance:** This is the power that does work and is billed by electricity providers.

2.  **Reactive Power (Q)**
    * **Definition:** The power that continuously oscillates between the source and the reactive components (inductors and capacitors). It is stored and returned to the source without doing any useful work.
    * **Unit:** Volt-Ampere Reactive (VAR).
    * **Formula:** $Q = V_{rms} I_{rms} \sin(\phi) = I_{rms}^2 X = \frac{V_{rms}^2}{X}$
    * **Significance:** Essential for magnetic fields (motors) and electric fields (capacitors), but contributes to the total current in the system without doing work. High reactive power leads to larger current flow for the same real power, increasing losses in transmission lines.

3.  **Apparent Power (S)**
    * **Definition:** The total power delivered by the source, which is the product of RMS voltage and RMS current, without considering the phase angle. It is the "total" power that the source needs to supply.
    * **Unit:** Volt-Ampere (VA).
    * **Formula:** $S = V_{rms} I_{rms}$
    * **Significance:** It represents the capacity of the power system (generators, transformers, cables). Equipment is often rated in kVA or MVA.

#### B. Power Triangle

The relationship between real, reactive, and apparent power can be represented graphically by a right-angled triangle called the power triangle.

* **Hypotenuse:** Apparent Power (S)
* **Adjacent Side:** Real Power (P) (along the horizontal axis)
* **Opposite Side:** Reactive Power (Q) (along the vertical axis)
* **Angle:** The angle between P and S is the phase angle ($\phi$).

* **Mathematical Relationships (from Pythagorean theorem and trigonometry):**
    * $S^2 = P^2 + Q^2$
    * $P = S \cos(\phi)$
    * $Q = S \sin(\phi)$
    * $\cos(\phi) = \frac{P}{S} = \text{Power Factor}$

* **Interpretation:**
    * **Lagging PF:** Q is positive (inductive load), triangle points upwards.
    * **Leading PF:** Q is negative (capacitive load), triangle points downwards.
    * **Unity PF:** Q = 0, triangle collapses to a line (S = P).

**Importance of Power Factor Correction:** In industrial and large commercial installations, inductive loads (motors, transformers) cause a lagging power factor. This increases the total current drawn from the supply, leading to higher line losses and larger required equipment ratings. Power factor correction (by adding capacitors in parallel) is used to bring the power factor closer to unity, reducing these issues.

---
This detailed explanation covers all the concepts within Unit V, providing definitions, formulas, and practical significance for understanding AC circuits.
