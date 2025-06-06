Let's get into **UNIT - 5: Electromagnetism**! We'll explore each concept in detail, point by point, with formulas and clear explanations.

---

## UNIT - 5: Electromagnetism

Electromagnetism is a fundamental branch of physics that studies the relationship between electricity and magnetism. It deals with the magnetic effects of electric currents and the electric effects of changing magnetic fields.

---

### 1. Types of Magnetic Materials (चुंबकीय पदार्थों के प्रकार)

Materials respond differently when placed in an external magnetic field. This response is classified into three main types based on their magnetic properties: diamagnetic, paramagnetic, and ferromagnetic.

#### a) Diamagnetic Materials (प्रतिचुंबकीय पदार्थ)

* **Properties:**
    * **Weakly Repelled:** These materials are very weakly repelled by a strong magnetic field.
    * **No Permanent Dipole Moment:** Their atoms do not have a permanent magnetic dipole moment. When an external magnetic field is applied, it induces a weak magnetic dipole moment in the opposite direction to the applied field.
    * **Permeability:** Their relative permeability ($\mu_r$) is slightly less than 1 ($\mu_r < 1$).
    * **Susceptibility:** Their magnetic susceptibility ($\chi_m$) is small, negative, and independent of temperature. ($\chi_m < 0$).
    * **Field Lines:** Magnetic field lines are repelled or pushed out of a diamagnetic material.
* **Examples:** Bismuth (Bi), Copper (Cu), Lead (Pb), Silicon (Si), Nitrogen (N₂), Water (H₂O), Gold (Au), Silver (Ag), Diamond (C), Salt (NaCl).
* **Why they behave this way:** The electrons in these materials are all paired, so their individual magnetic moments cancel out. The weak repulsion arises from the orbital motion of electrons which, according to Lenz's law, induces a magnetic field opposing the external field.

#### b) Paramagnetic Materials (अनुचुंबकीय पदार्थ)

* **Properties:**
    * **Weakly Attracted:** These materials are weakly attracted to a strong magnetic field.
    * **Permanent Dipole Moment:** Their atoms have a permanent magnetic dipole moment due to unpaired electrons. However, these moments are randomly oriented in the absence of an external field, so the net magnetism is zero.
    * **Alignment:** When an external magnetic field is applied, these individual dipole moments tend to align themselves parallel to the field, causing a weak magnetization in the direction of the field.
    * **Permeability:** Their relative permeability ($\mu_r$) is slightly greater than 1 ($\mu_r > 1$).
    * **Susceptibility:** Their magnetic susceptibility ($\chi_m$) is small, positive, and inversely proportional to absolute temperature (Curie's Law). ($\chi_m > 0$).
    * **Field Lines:** Magnetic field lines are slightly concentrated or drawn into a paramagnetic material.
* **Examples:** Aluminum (Al), Sodium (Na), Platinum (Pt), Oxygen (O₂), Copper Chloride (CuCl₂), Chromium (Cr).
* **Why they behave this way:** The presence of unpaired electrons gives individual atoms a small magnetic moment. Thermal agitation prevents perfect alignment, leading to weak magnetization.

#### c) Ferromagnetic Materials (लौहचुंबकीय पदार्थ)

* **Properties:**
    * **Strongly Attracted:** These materials are strongly attracted to a magnetic field and can be permanently magnetized.
    * **Domains:** They consist of microscopic regions called **domains**, where atomic magnetic moments are spontaneously aligned in the same direction, even without an external field. However, in an unmagnetized piece, these domains are randomly oriented, resulting in no net magnetic moment.
    * **Strong Magnetization:** When an external magnetic field is applied, the domains aligned with the field grow in size, and domains not aligned with the field may reorient. This leads to very strong magnetization in the direction of the applied field.
    * **Hysteresis:** They exhibit hysteresis, meaning their magnetization depends not only on the current applied field but also on their past magnetic history. This property is crucial for making permanent magnets.
    * **Curie Temperature:** Above a certain temperature called the **Curie temperature**, ferromagnetic materials lose their ferromagnetism and become paramagnetic.
    * **Permeability:** Their relative permeability ($\mu_r$) is much greater than 1 (often thousands or tens of thousands). ($\mu_r \gg 1$).
    * **Susceptibility:** Their magnetic susceptibility ($\chi_m$) is large and positive, and dependent on temperature in a complex way. ($\chi_m \gg 0$).
    * **Field Lines:** Magnetic field lines are strongly concentrated or drawn into a ferromagnetic material.
* **Examples:** Iron (Fe), Nickel (Ni), Cobalt (Co), and their alloys (like steel, alnico).
* **Why they behave this way:** The strong interaction between the atomic magnetic moments (exchange coupling) leads to the formation of domains and strong cooperative alignment.

---

### 2. Magnetic Field and its Units (चुंबकीय क्षेत्र और उसकी इकाई)

A **magnetic field** is a region around a magnetic material or a moving electric charge within which the force of magnetism acts. It is represented by magnetic field lines.

* **Units:**
    * The SI unit of magnetic field (magnetic flux density or magnetic induction, denoted by $\vec{B}$) is the **Tesla (T)**.
    * Another unit commonly used is the **Gauss (G)**.
    * 1 Tesla = 10,000 Gauss.
    * The Earth's magnetic field at the surface is typically around $25 \text{ to } 65 \mu\text{T}$ (microteslas) or $0.25 \text{ to } 0.65$ Gauss.

---

### 3. Magnetic Intensity (चुंबकीय तीव्रता)

Magnetic Intensity, also known as **Magnetic Field Strength** or **Magnetizing Field** (denoted by $\vec{H}$), is a measure of the strength of an external magnetic field applied to a material. It represents the ability of the applied current to create a magnetic field, irrespective of the material.

* **Concept:** When an external magnetic field is applied to a material, the total magnetic field inside the material is due to the applied field plus the field produced by the magnetization of the material itself. Magnetic intensity $\vec{H}$ is a quantity that solely depends on the external currents (and not on the material's response).

* **Relationship with Magnetic Field ($\vec{B}$):**
    The total magnetic field $\vec{B}$ inside a material is related to the magnetic intensity $\vec{H}$ and the magnetization $\vec{M}$ of the material by:
    $$\vec{B} = \mu_0 (\vec{H} + \vec{M})$$
    Where:
    * $\vec{B}$ = Magnetic field (magnetic flux density) in Tesla (T)
    * $\vec{H}$ = Magnetic intensity (magnetizing field) in Amperes per meter (A/m)
    * $\vec{M}$ = Magnetization of the material in Amperes per meter (A/m)
    * $\mu_0$ = Permeability of free space ($\mu_0 = 4\pi \times 10^{-7} \text{ T m/A}$)

* **Units:** The SI unit of magnetic intensity ($\vec{H}$) is **Amperes per meter (A/m)**.

---

### 4. Magnetic Lines of Force (चुंबकीय बल रेखाएँ)

Magnetic lines of force (or magnetic field lines) are imaginary lines used to represent the direction and strength of a magnetic field.

* **Properties:**
    1.  **Closed Loops:** Unlike electric field lines, magnetic field lines always form continuous closed loops. They emerge from the North pole and enter the South pole outside the magnet, and continue from the South pole to the North pole inside the magnet.
    2.  **Direction:** The tangent to a magnetic field line at any point gives the direction of the magnetic field ($\vec{B}$) at that point.
    3.  **No Intersection:** No two magnetic field lines can intersect each other. If they did, it would mean that at the point of intersection, the magnetic field has two directions, which is impossible.
    4.  **Density (Closeness):** The density of magnetic field lines (how closely packed they are) indicates the strength of the magnetic field. Where the lines are denser, the field is stronger; where they are sparser, the field is weaker.
    5.  **Perpendicular to Surfaces:** Magnetic field lines emerge from or enter the surface of a magnet perpendicularly.

---

### 5. Magnetic Flux and Units (चुंबकीय फ्लक्स और इकाई)

**Magnetic flux ($\Phi_B$)** is a measure of the total number of magnetic field lines passing through a given area. It quantifies the amount of magnetic field passing through a surface.

* **Definition:** Magnetic flux through an area element is defined as the product of the magnitude of the magnetic field component perpendicular to the area and the area itself.

* **Formula:**
    * **For a uniform magnetic field ($\vec{B}$) and a flat surface with area vector ($\vec{A}$):**
        $$\Phi_B = \vec{B} \cdot \vec{A} = BA \cos\theta$$
        Where $\theta$ is the angle between the magnetic field vector $\vec{B}$ and the area vector $\vec{A}$ (which is perpendicular to the surface).
    * **For a non-uniform magnetic field or a curved surface (using calculus):**
        $$\Phi_B = \int \vec{B} \cdot d\vec{A}$$
        This integral is taken over the entire surface.

* **Units:** The SI unit of magnetic flux is the **Weber (Wb)**.
    * 1 Weber = 1 Tesla-meter squared (1 T m²).

---

### 6. Magnetization (चुंबकन)

**Magnetization ($\vec{M}$)** is a vector quantity that represents the magnetic dipole moment per unit volume of a material. It describes how much a material becomes magnetized when placed in an external magnetic field.

* **Concept:** When an external magnetic field is applied to a material, the atomic magnetic moments within the material tend to align with the field. This alignment results in a net magnetic dipole moment for the material. Magnetization quantifies this induced or intrinsic magnetic moment per unit volume.

* **Formula:**
    $$\vec{M} = \frac{\text{Magnetic dipole moment}}{\text{Volume}}$$
    The SI unit of magnetization is **Amperes per meter (A/m)**.

* **Relationship with Magnetic Susceptibility ($\chi_m$):**
    Magnetization ($\vec{M}$) is often proportional to the applied magnetic intensity ($\vec{H}$) for many materials:
    $$\vec{M} = \chi_m \vec{H}$$
    Where $\chi_m$ is the **magnetic susceptibility**, a dimensionless quantity that indicates how easily a material can be magnetized.
    * For diamagnetic materials, $\chi_m < 0$.
    * For paramagnetic materials, $\chi_m > 0$.
    * For ferromagnetic materials, $\chi_m \gg 0$ and is not constant.

* **Relation to Permeability:**
    We previously had $\vec{B} = \mu_0 (\vec{H} + \vec{M})$. Substituting $\vec{M} = \chi_m \vec{H}$:
    $$\vec{B} = \mu_0 (\vec{H} + \chi_m \vec{H})$$   $$\vec{B} = \mu_0 \vec{H} (1 + \chi_m)$$
    We also define the relative permeability $\mu_r = (1 + \chi_m)$, so:
    $$\vec{B} = \mu_0 \mu_r \vec{H} = \mu \vec{H}$$
    Where $\mu = \mu_0 \mu_r$ is the absolute permeability of the material.

---

### 7. Concept of Electromagnetic Induction (विद्युत चुम्बकीय प्रेरण की अवधारणा)

**Electromagnetic Induction** is the phenomenon where an electric current is generated in a conductor when it is exposed to a changing magnetic field. This is the fundamental principle behind generators, transformers, and many other electrical devices.

* **Key Idea:** It's not a static magnetic field that produces current, but a *changing* magnetic field. The change can be due to:
    * A magnet moving relative to a coil.
    * A coil moving relative to a magnet.
    * Changing the current in a nearby coil (which changes its magnetic field).
    * Changing the orientation or area of a coil in a magnetic field.

* **Induced EMF (Electromotive Force):** The changing magnetic field induces an electromotive force (EMF) across the ends of the conductor. This induced EMF then drives an induced current if the circuit is closed.

---

### 8. Faraday's Laws of Electromagnetic Induction (फैराडे के विद्युत चुम्बकीय प्रेरण के नियम)

Michael Faraday discovered the laws governing electromagnetic induction.

#### a) Faraday's First Law:

* **Statement:** Whenever the amount of magnetic flux linked with a circuit changes, an electromotive force (EMF) is induced in the circuit. This induced EMF lasts as long as the change in magnetic flux continues.

* **Simple Explanation:** If you change how much magnetic field passes through a loop of wire, a voltage (EMF) will be created in that loop. This voltage will last only as long as the magnetic field is changing.

#### b) Faraday's Second Law:

* **Statement:** The magnitude of the induced electromotive force (EMF) in a circuit is directly proportional to the rate of change of magnetic flux linked with the circuit.

* **Mathematical Form:**
    $$E = -\frac{d\Phi_B}{dt}$$
    Where:
    * $E$ = Induced electromotive force (in Volts, V)
    * $\Phi_B$ = Magnetic flux (in Webers, Wb)
    * $\frac{d\Phi_B}{dt}$ = Rate of change of magnetic flux with respect to time (in Wb/s)
    * The negative sign is due to **Lenz's Law**.

* **Lenz's Law (लेनज़ का नियम):**
    Lenz's Law gives the *direction* of the induced EMF and current. It states that the direction of the induced current (or EMF) is always such that it opposes the cause that produced it.
    * **Explanation:** If the magnetic flux through a coil is increasing, the induced current will flow in a direction that creates a magnetic field *opposing* this increase. If the flux is decreasing, the induced current will create a magnetic field that *supports* the original field to oppose the decrease. This is a consequence of the conservation of energy.

* **For a coil with N turns:** If a coil has $N$ turns, and the flux through each turn changes by $d\Phi_B$, the total induced EMF is:
    $$E = -N \frac{d\Phi_B}{dt}$$

---

### 9. Lorentz Force (force on moving charge in magnetic field) (लॉरेंज बल - चुंबकीय क्षेत्र में गतिमान आवेश पर बल)

The Lorentz force is the total force exerted by an electromagnetic field on a charged particle. It consists of two components: the electric force and the magnetic force. Here, we'll focus on the magnetic component.

* **Statement:** A moving electric charge in a magnetic field experiences a force.

* **Formula (Magnetic Lorentz Force):**
    If a charge $q$ moves with a velocity $\vec{v}$ in a magnetic field $\vec{B}$, the magnetic force ($\vec{F}_B$) on the charge is given by:
    $$\vec{F}_B = q (\vec{v} \times \vec{B})$$
    The magnitude of this force is:
    $$F_B = q v B \sin\theta$$
    Where:
    * $q$ = Magnitude of the charge (in Coulombs, C)
    * $v$ = Magnitude of the velocity of the charge (in m/s)
    * $B$ = Magnitude of the magnetic field (in Tesla, T)
    * $\theta$ = Angle between the velocity vector $\vec{v}$ and the magnetic field vector $\vec{B}$.

* **Direction of Force:** The direction of the force is perpendicular to both the velocity vector ($\vec{v}$) and the magnetic field vector ($\vec{B}$), as determined by the right-hand rule for cross products.
    * If $q$ is positive, the direction of $\vec{F}_B$ is in the direction of $\vec{v} \times \vec{B}$.
    * If $q$ is negative, the direction of $\vec{F}_B$ is opposite to $\vec{v} \times \vec{B}$.

* **Important Points:**
    * No force is exerted on a stationary charge in a magnetic field ($v=0 \Rightarrow F_B=0$).
    * No force is exerted if the charge moves parallel or anti-parallel to the magnetic field ($\theta=0^\circ$ or $180^\circ \Rightarrow \sin\theta=0 \Rightarrow F_B=0$).
    * The force is maximum when the charge moves perpendicular to the magnetic field ($\theta=90^\circ \Rightarrow \sin\theta=1 \Rightarrow F_B = qvB$).
    * The magnetic force *never* does any work on the charged particle because the force is always perpendicular to the displacement. It only changes the direction of motion, not the speed. This is why charged particles move in circular or helical paths in uniform magnetic fields.

---

### 10. Force on Current Carrying Conductor (धारावाही चालक पर बल)

A current-carrying conductor consists of charges moving in a specific direction. Therefore, a current-carrying conductor placed in a magnetic field will experience a force due to the magnetic force on the individual moving charges within it.

* **Derivation (Simplified):**
    Consider a conductor of length $L$ carrying current $I$ placed in a uniform magnetic field $\vec{B}$.
    Let $n$ be the number of charge carriers (electrons) per unit volume.
    Let $A$ be the cross-sectional area of the conductor.
    Let $v_d$ be the drift velocity of the charge carriers.
    The total charge in the conductor is $Q = (nA)L e$, where $e$ is the charge of an electron.
    The current $I = nAv_d e$.
    The force on one charge carrier is $F_{charge} = e (\vec{v}_d \times \vec{B})$.
    The total force on the conductor is the sum of forces on all charge carriers:
    $\vec{F} = (\text{number of charge carriers}) \times F_{charge}$
    $\vec{F} = (nAL) \times e (\vec{v}_d \times \vec{B})$
    Rearranging terms:
    $\vec{F} = (n A v_d e) (L \vec{B})$ (assuming $\vec{L}$ is in direction of $\vec{v}_d$)
    Since $I = n A v_d e$, we get:
    $$\vec{F} = I (\vec{L} \times \vec{B})$$

* **Formula:** The magnetic force on a current-carrying conductor of length $L$ with current $I$ in a uniform magnetic field $\vec{B}$ is:
    $$\vec{F} = I (\vec{L} \times \vec{B})$$
    The magnitude of this force is:
    $$F = BIL \sin\theta$$
    Where:
    * $I$ = Current in the conductor (in Amperes, A)
    * $L$ = Length of the conductor (in meters, m)
    * $B$ = Magnitude of the magnetic field (in Tesla, T)
    * $\theta$ = Angle between the direction of current (or $\vec{L}$) and the magnetic field $\vec{B}$.

* **Direction of Force:** The direction of the force is given by the right-hand rule (or Fleming's Left-Hand Rule).
    * Maximum force occurs when the conductor is perpendicular to the magnetic field ($\theta=90^\circ, F=BIL$).
    * No force occurs when the conductor is parallel or anti-parallel to the magnetic field ($\theta=0^\circ$ or $180^\circ, F=0$).

---

### 11. Force on Rectangular Coil Placed in Magnetic Field (चुंबकीय क्षेत्र में रखी आयताकार कुंडली पर बल)

When a current-carrying rectangular coil is placed in a uniform magnetic field, the forces acting on its sides produce a net torque, causing the coil to rotate. This principle is fundamental to electric motors and galvanometers.

* **Setup:** Consider a rectangular coil of length $l$ and breadth $b$, having $N$ turns, carrying a current $I$. It is placed in a uniform magnetic field $\vec{B}$.

* **Forces on Sides:**
    Let's assume the magnetic field is along the x-axis, and the coil rotates in the xy-plane.
    1.  **Sides Perpendicular to Field (Length $l$):**
        * The two sides of length $l$ (say, AB and CD) are parallel to the axis of rotation and experience forces.
        * Force on side AB: $F_1 = BI l \sin 90^\circ = BI l$. This force is directed inwards (into the page).
        * Force on side CD: $F_2 = BI l \sin 90^\circ = BI l$. This force is directed outwards (out of the page).
        * These two forces are equal in magnitude, opposite in direction, and act on different lines of action, forming a couple.
    2.  **Sides Parallel to Field (Breadth $b$):**
        * The two sides of breadth $b$ (say, BC and DA) are parallel to the magnetic field lines when the coil's plane is perpendicular to the field.
        * Force on side BC: $F_3 = BI b \sin 0^\circ = 0$. (When the side is parallel to the field, angle is 0).
        * Force on side DA: $F_4 = BI b \sin 180^\circ = 0$.
        * When the coil rotates, the forces on these sides will not always be zero, but they will always be along the axis of rotation and thus produce no torque.

* **Torque on the Coil ($\tau$):**
    The forces $F_1$ and $F_2$ form a couple, producing a torque that tends to rotate the coil.
    The perpendicular distance between $F_1$ and $F_2$ is $b \sin\alpha$, where $\alpha$ is the angle between the normal to the plane of the coil and the magnetic field $\vec{B}$.
    Torque ($\tau$) = Force $\times$ Perpendicular distance
    $\tau = (BIl) (b \sin\alpha)$
    Since $A = l \times b$ (area of the coil) and for $N$ turns, the total current becomes $NI$:
    $$\tau = N I A B \sin\alpha$$
    This can also be written in vector form using the magnetic dipole moment ($\vec{m}$) of the coil:
    $\vec{m} = NIA \hat{n}$ (where $\hat{n}$ is the normal to the coil's area)
    $$\vec{\tau} = \vec{m} \times \vec{B}$$

* **Important Points:**
    * The torque is maximum when the plane of the coil is parallel to the magnetic field ($\alpha = 90^\circ$, $\sin 90^\circ = 1 \Rightarrow \tau_{max} = NIAB$).
    * The torque is zero when the plane of the coil is perpendicular to the magnetic field ($\alpha = 0^\circ$, $\sin 0^\circ = 0 \Rightarrow \tau = 0$).

---

### 12. Moving Coil Galvanometer (चल कुंडली गैल्वेनोमीटर)

A **moving coil galvanometer** is a sensitive instrument used for detecting and measuring small electric currents. Its operation is based on the principle that a current-carrying coil placed in a magnetic field experiences a torque.

#### a) Principle:

* When a current-carrying coil is placed in a uniform magnetic field, it experiences a torque proportional to the current flowing through it. This torque causes the coil to deflect.

#### b) Construction:

* **Coil:** A rectangular coil of many turns of fine insulated copper wire wound over a non-magnetic (aluminum or brass) frame.
* **Suspension Wire:** The coil is suspended by a thin phosphor bronze strip (acting as a torsion head and current lead) from a torsion head. The other end of the coil is connected to a light spring.
* **Mirror:** A small mirror is attached to the suspension wire (or coil) to measure deflection using a lamp and scale arrangement.
* **Magnets:** A strong permanent horse-shoe magnet provides a radial magnetic field.
* **Soft Iron Core:** A soft iron core is placed centrally and coaxially within the coil. It is stationary and non-magnetic (not touching the coil).

#### c) Working:

1.  When a current $I$ flows through the coil, each turn of the coil experiences a torque.
2.  The torque on the coil is given by $\tau = NIAB \sin\alpha$.
3.  Due to the radial magnetic field provided by the curved poles and the soft iron core, the plane of the coil is always parallel to the magnetic field lines (i.e., the normal to the coil is always perpendicular to the field). So, $\alpha = 90^\circ$, and $\sin\alpha = 1$.
4.  Therefore, the deflecting torque is $\tau_d = NIAB$.
5.  This deflecting torque causes the coil to rotate. As the coil rotates, the suspension wire (phosphor bronze strip) twists.
6.  The twisting of the suspension wire produces a restoring torque ($\tau_r$) which opposes the deflection. This restoring torque is proportional to the angle of twist ($\theta$) of the suspension wire: $\tau_r = k\theta$, where $k$ is the torsional constant of the suspension wire.
7.  The coil deflects until the deflecting torque equals the restoring torque:
    $\tau_d = \tau_r$
    $NIAB = k\theta$
8.  From this, the current $I$ is directly proportional to the deflection $\theta$:
    $$I = \left(\frac{k}{NAB}\right)\theta$$   $$I = G\theta$$
    Where $G = \frac{k}{NAB}$ is the galvanometer constant.
    This means the deflection on the scale is directly proportional to the current flowing through the galvanometer.

---

### 13. Conversion of a Galvanometer into Ammeter and Voltmeter (गैल्वेनोमीटर को एमीटर और वोल्टमीटर में बदलना)

A galvanometer is very sensitive and can only measure very small currents. To measure larger currents (Ammeter) or voltages (Voltmeter), it needs to be modified.

#### a) Conversion of a Galvanometer into Ammeter:

* **Purpose:** An ammeter is used to measure electric current in a circuit. It must have a very low resistance and be connected in **series** with the component through which the current is to be measured.
* **Method:** To convert a galvanometer into an ammeter, a very small resistance, called a **shunt resistance ($R_{sh}$)**, is connected in **parallel** with the galvanometer.
* **Reasoning:**
    * The shunt resistance bypasses most of the current, allowing only a small fraction to pass through the sensitive galvanometer. This protects the galvanometer from damage by large currents.
    * Connecting the shunt in parallel makes the overall resistance of the ammeter very low, ensuring it doesn't significantly change the current in the main circuit when connected in series.
* **Derivation for Shunt Resistance:**
    Let $I$ be the maximum current to be measured by the ammeter.
    Let $I_g$ be the full-scale deflection current of the galvanometer.
    Let $R_g$ be the resistance of the galvanometer coil.
    The current through the shunt is $I_{sh} = I - I_g$.
    Since the galvanometer and shunt are in parallel, the potential difference across them is the same:
    $V_g = V_{sh}$
    $I_g R_g = I_{sh} R_{sh}$
    $I_g R_g = (I - I_g) R_{sh}$
    $$R_{sh} = \frac{I_g R_g}{I - I_g}$$
* **Final Ammeter:** The combination of the galvanometer and the shunt resistance now acts as an ammeter with a specific range (up to $I$).

#### b) Conversion of a Galvanometer into Voltmeter:

* **Purpose:** A voltmeter is used to measure the potential difference (voltage) across two points in a circuit. It must have a very high resistance and be connected in **parallel** across the points where the voltage is to be measured.
* **Method:** To convert a galvanometer into a voltmeter, a very large resistance, called a **series resistance ($R_{series}$)**, is connected in **series** with the galvanometer.
* **Reasoning:**
    * Connecting a high resistance in series increases the overall resistance of the voltmeter.
    * This high resistance ensures that the voltmeter draws a negligible amount of current from the main circuit when connected in parallel, thereby not significantly altering the potential difference it is trying to measure.
    * The series resistance allows the galvanometer to measure a larger voltage range, as a larger voltage drop occurs across the series resistor.
* **Derivation for Series Resistance:**
    Let $V$ be the maximum voltage to be measured by the voltmeter.
    Let $I_g$ be the full-scale deflection current of the galvanometer.
    Let $R_g$ be the resistance of the galvanometer coil.
    The galvanometer and the series resistance are in series, so the total resistance is $R_{total} = R_g + R_{series}$.
    The total voltage $V$ is given by Ohm's Law across this series combination:
    $V = I_g (R_g + R_{series})$
    $$R_{series} = \frac{V}{I_g} - R_g$$
* **Final Voltmeter:** The combination of the galvanometer and the series resistance now acts as a voltmeter with a specific range (up to $V$).

---

This comprehensive breakdown should provide a solid understanding of Electromagnetism concepts from Unit 5!
