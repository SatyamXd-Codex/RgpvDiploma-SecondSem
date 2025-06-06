

## UNIT - 4: Current Electricity

This unit delves into the fundamental principles governing the flow of electric charge, its associated properties, and practical applications.

### 1. Electric Current and its Units

* **Electric Current ($I$):** The rate of flow of electric charge through a conductor.
    * Mathematically, $I = \frac{dQ}{dt}$, where $dQ$ is the amount of charge flowing in time $dt$.
* **Units of Electric Current:** The SI unit of electric current is the **Ampere (A)**.
    * 1 Ampere = 1 Coulomb/second (C/s)

### 2. Direct and Alternating Current

* **Direct Current (DC):** Electric current that flows in only one direction.
    * Examples: Current from batteries, solar cells.
* **Alternating Current (AC):** Electric current that periodically reverses its direction.
    * Examples: Household electricity supply.

### 3. Resistance and its Units

* **Resistance ($R$):** The opposition offered by a conductor to the flow of electric current.
    * It is a measure of how difficult it is for electrons to move through a material.
* **Units of Resistance:** The SI unit of resistance is the **Ohm ($\Omega$)**.

### 4. Specific Resistance (Resistivity)

* **Specific Resistance ($\rho$):** Also known as resistivity, it is an intrinsic property of a material that quantifies its resistance to electrical conduction. It is independent of the dimensions of the conductor.
    * Mathematically, $R = \rho \frac{L}{A}$, where $R$ is resistance, $L$ is length, and $A$ is cross-sectional area.
* **Units of Specific Resistance:** Ohm-meter ($\Omega \cdot m$).

### 5. Conductance

* **Conductance ($G$):** The reciprocal of resistance. It measures how easily electric current flows through a material.
    * Mathematically, $G = \frac{1}{R}$.
* **Units of Conductance:** The SI unit of conductance is the **Siemens (S)**, also sometimes referred to as mho ($\mho$).

### 6. Specific Conductance (Conductivity)

* **Specific Conductance ($\sigma$):** Also known as conductivity, it is the reciprocal of specific resistance (resistivity). It is an intrinsic property of a material that quantifies its ability to conduct electricity.
    * Mathematically, $\sigma = \frac{1}{\rho}$.
* **Units of Specific Conductance:** Siemens per meter (S/m).

### 7. Series and Parallel Combination of Resistances

* **Series Combination:**
    * Resistances are connected end-to-end.
    * The total resistance ($R_{eq}$) is the sum of individual resistances: $R_{eq} = R_1 + R_2 + R_3 + ...$
    * The current is the same through each resistor.
    * The voltage divides across each resistor.
* **Parallel Combination:**
    * Resistances are connected across the same two points.
    * The reciprocal of the total resistance is the sum of the reciprocals of individual resistances: $\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + ...$
    * The voltage is the same across each resistor.
    * The current divides among the branches.

### 8. Factors Affecting Resistance of a Wire

The resistance of a metallic wire depends on the following factors:
* **Length ($L$):** Resistance is directly proportional to the length of the wire ($R \propto L$). Longer wires have higher resistance.
* **Area of Cross-section ($A$):** Resistance is inversely proportional to the area of cross-section of the wire ($R \propto \frac{1}{A}$). Thicker wires have lower resistance.
* **Nature of the Material ($\rho$):** Resistance depends on the resistivity of the material. Different materials have different inherent resistivities.
* **Temperature:** For most conductors, resistance increases with an increase in temperature.

### 9. Carbon Resistances and Colour Coding

* **Carbon Resistances:** Commonly used resistors made from carbon composition or film. They are small, inexpensive, and widely used in electronic circuits.
* **Colour Coding:** A standardized system using coloured bands on the resistor to indicate its resistance value and tolerance. Each colour represents a digit, a multiplier, and a tolerance percentage.

### 10. Ohm’s Law and its Verification

* **Ohm's Law:** States that the current flowing through a conductor between two points is directly proportional to the voltage across the two points, provided the temperature and other physical conditions remain constant.
    * Mathematically, $V = IR$, where $V$ is voltage, $I$ is current, and $R$ is resistance.
* **Verification:** Can be verified experimentally by setting up a circuit, varying the voltage across a resistor, measuring the corresponding current, and plotting a V-I graph. A straight line passing through the origin indicates Ohm's law is obeyed.

### 11. Kirchhoff’s Laws

These laws are fundamental for analyzing complex electrical circuits.
* **Kirchhoff’s Current Law (KCL) / Junction Rule:** The algebraic sum of currents entering a junction (node) is equal to the algebraic sum of currents leaving the junction. (Conservation of charge)
* **Kirchhoff’s Voltage Law (KVL) / Loop Rule:** The algebraic sum of the changes in potential around any closed loop in a circuit is zero. (Conservation of energy)

### 12. Wheatstone Bridge and its Applications (Slide Wire Bridge Only)

* **Wheatstone Bridge:** An electrical circuit used to measure an unknown electrical resistance by balancing two legs of a bridge circuit, one leg of which includes the unknown component.
* **Principle:** When the bridge is balanced, no current flows through the galvanometer, and the ratio of resistances in the two arms is equal.
    * $\frac{P}{Q} = \frac{R}{S}$ (where P, Q, R, S are resistances in the four arms)
* **Slide Wire Bridge (Meter Bridge):** A practical application of the Wheatstone bridge used to measure unknown resistances or compare resistances. It uses a uniform resistance wire along which a sliding contact can be moved to balance the bridge.

### 13. Concept of Terminal Potential Difference and Electromotive Force (EMF)

* **Electromotive Force (EMF - $\mathcal{E}$):** The maximum potential difference that a source of electrical energy (like a battery or generator) can provide when no current is drawn from it (i.e., in an open circuit). It represents the energy provided per unit charge.
* **Terminal Potential Difference ($V_T$):** The actual potential difference across the terminals of a source when current is being drawn from it.
    * Due to the internal resistance ($r$) of the source, there is a voltage drop across it.
    * $V_T = \mathcal{E} - Ir$ (when current is flowing out of the source)
    * $V_T = \mathcal{E} + Ir$ (when current is flowing into the source, e.g., during charging)

### 14. Heating Effect of Current (Joule Heating)

* **Heating Effect:** When electric current flows through a conductor, electrical energy is converted into heat energy. This phenomenon is known as the heating effect of current or Joule heating.
* **Joule's Law of Heating:** The heat produced ($H$) in a conductor is directly proportional to the square of the current ($I^2$), the resistance ($R$) of the conductor, and the time ($t$) for which the current flows.
    * $H = I^2 R t$ (in Joules)
    * This heat can be used in various applications like electric heaters, geysers, etc.

### 15. Electric Power

* **Electric Power ($P$):** The rate at which electrical energy is consumed or dissipated in an electrical circuit.
    * Mathematically, $P = \frac{W}{t}$, where $W$ is work done (energy) and $t$ is time.
* **Formulas for Electric Power:**
    * $P = VI$ (Voltage × Current)
    * $P = I^2 R$ (Current squared × Resistance)
    * $P = \frac{V^2}{R}$ (Voltage squared / Resistance)
* **Units of Electric Power:** The SI unit of electric power is the **Watt (W)**.
    * 1 Watt = 1 Joule/second (J/s)

### 16. Electric Energy and its Units (Related Numerical Problems)

* **Electric Energy ($W$ or $E$):** The total amount of electrical work done or energy consumed over a period of time.
    * Mathematically, $W = P \times t = VIt = I^2 Rt = \frac{V^2}{R} t$.
* **Units of Electric Energy:** The SI unit of electric energy is the **Joule (J)**.
* **Commercial Unit of Electric Energy:** The **kilowatt-hour (kWh)**.
    * 1 kWh = $1000 \text{ W} \times 3600 \text{ s} = 3.6 \times 10^6 \text{ J}$
    * This is the unit used by electricity meters to bill consumers.
* **Numerical Problems:** Expect problems involving calculations of resistance, current, voltage, power, energy consumption, and cost of electricity based on the given formulas.

### 17. Advantages of Electric Energy over other forms of energy

* **Clean and Environmentally Friendly (at the point of use):** Does not produce pollutants or combustion byproducts at the consumer end.
* **Easy Transmission:** Can be transmitted over long distances through wires with relatively low losses.
* **Easy Conversion:** Can be easily converted into other forms of energy such as light (bulbs), heat (heaters), mechanical energy (motors), and sound (speakers).
* **Versatility:** Used in a vast array of applications, from lighting and heating to communication, computing, and industrial processes.
* **Controllability:** Can be precisely controlled in terms of voltage, current, and power.
* **Convenience:** Easily accessible through power outlets in homes and workplaces.

---
