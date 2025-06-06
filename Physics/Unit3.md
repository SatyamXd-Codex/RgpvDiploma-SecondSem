Alright, let's dive into **Electrostatics (स्थिरवैद्युतिकी)** from Unit 3! We'll cover each topic in detail, point by point, with formulas, derivations, and easy-to-understand explanations in English.

---

## UNIT - 3: Electrostatics

Electrostatics is the branch of physics that deals with the properties of electric charges at rest (static charges). It studies the forces, fields, and potentials associated with these stationary charges.

---

### 1. Coulomb's Law (कूलॉम का नियम)

Coulomb's Law describes the electric force between two stationary, charged particles. It's a fundamental law in electrostatics, similar to Newton's Law of Universal Gravitation for masses.

* **Statement:** The force of attraction or repulsion between two point charges is directly proportional to the product of the magnitudes of the charges and inversely proportional to the square of the distance between them. This force acts along the line joining the two charges.

* **Mathematical Form:**
    Consider two point charges, $q_1$ and $q_2$, separated by a distance $r$. The magnitude of the electrostatic force ($F$) between them is given by:
    $$F = k \frac{|q_1 q_2|}{r^2}$$
    Where:
    * $F$ = Electrostatic force (in Newtons, N)
    * $q_1, q_2$ = Magnitudes of the point charges (in Coulombs, C)
    * $r$ = Distance between the charges (in meters, m)
    * $k$ = Coulomb's constant, also known as the electrostatic constant.

* **Value of Coulomb's Constant ($k$):**
    In vacuum or air, the value of $k$ is approximately:
    $$k \approx 9 \times 10^9 \text{ N m}^2/\text{C}^2$$
    Coulomb's constant $k$ is often expressed in terms of another fundamental constant, the permittivity of free space ($\epsilon_0$):
    $$k = \frac{1}{4\pi\epsilon_0}$$
    Where $\epsilon_0$ is the permittivity of free space, and its value is:
    $$\epsilon_0 \approx 8.854 \times 10^{-12} \text{ C}^2/\text{N m}^2$$
    So, the force formula can also be written as:
    $$F = \frac{1}{4\pi\epsilon_0} \frac{|q_1 q_2|}{r^2}$$

* **Direction of Force:**
    * If $q_1$ and $q_2$ have the same sign (both positive or both negative), the force is repulsive (they push each other away).
    * If $q_1$ and $q_2$ have opposite signs (one positive, one negative), the force is attractive (they pull each other towards each other).
    * The force acts along the line connecting the two charges.

* **Vector Form of Coulomb's Law (Optional but good to know):**
    If $\vec{F}_{12}$ is the force on $q_1$ due to $q_2$, and $\vec{r}_{12}$ is the position vector from $q_2$ to $q_1$:
    $$\vec{F}_{12} = \frac{1}{4\pi\epsilon_0} \frac{q_1 q_2}{r^2} \hat{r}_{12}$$
    Here, $\hat{r}_{12}$ is the unit vector pointing from $q_2$ to $q_1$.

---

### 2. Unit of Charge (आवेश की इकाई)

* The SI unit of electric charge is the **Coulomb (C)**.
* One Coulomb is defined as the amount of charge that, when placed one meter away from an identical charge in a vacuum, experiences an electrostatic force of $9 \times 10^9$ Newtons.
* The charge of a single electron is approximately $-1.602 \times 10^{-19}$ C.
* The charge of a single proton is approximately $+1.602 \times 10^{-19}$ C.
* Charge is quantized, meaning it exists in discrete packets, i.e., an integer multiple of the elementary charge ($e = 1.602 \times 10^{-19}$ C). So, $Q = ne$, where $n$ is an integer.

---

### 3. Electric Field (विद्युत क्षेत्र)

An electric field is a region around a charged particle or object within which a force would be exerted on other charged particles. It's an invisible influence that surrounds electric charges.

* **Definition:** The electric field ($\vec{E}$) at a point is defined as the electrostatic force experienced by a unit positive test charge placed at that point.

* **Formula:**
    $$\vec{E} = \frac{\vec{F}}{q_0}$$
    Where:
    * $\vec{E}$ = Electric field vector (in Newtons per Coulomb, N/C, or Volts per meter, V/m)
    * $\vec{F}$ = Electrostatic force experienced by the test charge (in N)
    * $q_0$ = Small positive test charge (in C). The test charge must be infinitesimally small so as not to disturb the original electric field.

* **Electric Field due to a Point Charge ($Q$):**
    If a point charge $Q$ is located at the origin, the electric field at a distance $r$ from it is given by:
    $$E = \frac{1}{4\pi\epsilon_0} \frac{|Q|}{r^2}$$
    The direction of $\vec{E}$ is radially outward if $Q$ is positive and radially inward if $Q$ is negative.

* **Units:** The SI unit of electric field is Newton per Coulomb (N/C) or Volt per meter (V/m).

---

### 4. Electric Lines of Force and their Properties (विद्युत बल रेखाएँ और उनके गुण)

Electric lines of force (also called electric field lines) are imaginary lines or curves drawn in an electric field along which a unit positive test charge would tend to move if left free. They provide a visual representation of the electric field.

* **Properties:**
    1.  **Origin and Termination:** Electric field lines originate from positive charges and terminate on negative charges. If there is a single isolated charge, they may extend to infinity.
    2.  **Direction:** The tangent to an electric field line at any point gives the direction of the electric field at that point.
    3.  **No Intersection:** No two electric field lines can intersect each other. If they did, it would mean that at the point of intersection, the electric field has two directions, which is impossible.
    4.  **Density (Closeness):** The density of electric field lines (how closely packed they are) indicates the strength of the electric field. Where the lines are denser, the field is stronger; where they are sparser, the field is weaker.
    5.  **Perpendicular to Conductors:** Electric field lines are always perpendicular to the surface of a conductor (both charged and uncharged).
    6.  **No Closed Loops:** Electric field lines do not form closed loops. They start from positive charges and end on negative charges (or infinity). This is because the electrostatic field is a conservative field.
    7.  **No Field Inside Conductor:** Electric field lines do not pass through a conductor in static equilibrium; the electric field inside a conductor is zero.

---

### 5. Electric Flux (विद्युत फ्लक्स)

Electric flux ($\Phi_E$) is a measure of the number of electric field lines passing through a given surface. It quantifies the "flow" of the electric field through an area.

* **Definition:** Electric flux through an area element is defined as the product of the magnitude of the electric field component perpendicular to the area and the area itself.

* **Formula:**
    * **For a uniform electric field ($\vec{E}$) and a flat surface with area vector ($\vec{A}$):**
        $$\Phi_E = \vec{E} \cdot \vec{A} = EA \cos\theta$$
        Where $\theta$ is the angle between the electric field vector $\vec{E}$ and the area vector $\vec{A}$ (which is perpendicular to the surface).
    * **For a non-uniform electric field or a curved surface (using calculus):**
        $$\Phi_E = \int \vec{E} \cdot d\vec{A}$$
        This integral is taken over the entire surface.

* **Units:** The SI unit of electric flux is Newton meter squared per Coulomb (N m$^2$/C) or Volt-meter (V m).

---

### 6. Electric Potential and Potential Difference (विद्युत विभव और विभवान्तर)

These concepts are related to the energy associated with electric charges in an electric field.

#### Electric Potential ($V$):

* **Definition:** The electric potential at a point in an electric field is defined as the amount of work done by an external force to bring a unit positive test charge from infinity to that point without acceleration.

* **Formula:**
    $$V = \frac{W}{q_0}$$
    Where:
    * $V$ = Electric potential (in Volts, V)
    * $W$ = Work done (in Joules, J)
    * $q_0$ = Unit positive test charge (in C)

* **Electric Potential due to a Point Charge ($Q$):**
    The electric potential at a distance $r$ from a point charge $Q$ is:
    $$V = \frac{1}{4\pi\epsilon_0} \frac{Q}{r}$$
    Note: Unlike force or field, potential is a scalar quantity (it has magnitude but no direction). Its sign depends on the sign of the charge $Q$.

* **Units:** The SI unit of electric potential is the **Volt (V)**.
    1 Volt = 1 Joule/Coulomb (1 J/C).

#### Electric Potential Difference ($\Delta V$):

* **Definition:** The electric potential difference between two points (say, A and B) in an electric field is the amount of work done by an external force to move a unit positive test charge from point A to point B without acceleration.

* **Formula:**
    $$\Delta V = V_B - V_A = \frac{W_{AB}}{q_0}$$
    Where:
    * $V_B$ = Electric potential at point B
    * $V_A$ = Electric potential at point A
    * $W_{AB}$ = Work done in moving the charge from A to B.

* **Relationship between Electric Field and Electric Potential:**
    The electric field is the negative gradient of the electric potential. For a uniform electric field, the magnitude of the electric field can be related to the potential difference over a distance $d$:
    $$E = -\frac{\Delta V}{\Delta r}$$
    More generally, $\vec{E} = -\nabla V$ (gradient of potential).

---

### 7. Gauss's Law (गॉस का नियम)

Gauss's Law is a fundamental law in electrostatics that relates the electric flux through a closed surface to the net electric charge enclosed within that surface. It's very useful for calculating electric fields for charge distributions with high symmetry.

* **Statement:** The total electric flux passing through any closed surface (called a Gaussian surface) is equal to $1/\epsilon_0$ times the total electric charge enclosed within that surface.

* **Mathematical Form:**
    $$\Phi_E = \oint \vec{E} \cdot d\vec{A} = \frac{Q_{\text{enclosed}}}{\epsilon_0}$$
    Where:
    * $\Phi_E$ = Total electric flux through the closed surface.
    * $\oint \vec{E} \cdot d\vec{A}$ = Surface integral of the electric field over the closed surface.
    * $Q_{\text{enclosed}}$ = Net electric charge enclosed by the Gaussian surface.
    * $\epsilon_0$ = Permittivity of free space.

* **Key Idea:** Gauss's Law states that the flux through a surface depends only on the charge *inside* that surface, not on charges outside it.

#### Applications of Gauss's Law to find electric field intensity:

Gauss's Law simplifies the calculation of electric fields for symmetric charge distributions by choosing an appropriate Gaussian surface.

##### a) Electric Field Intensity due to a Straight Charged Conductor (Infinite Line Charge):

* **Setup:** Consider an infinitely long, thin, straight conductor with a uniform linear charge density $\lambda$ (charge per unit length).
* **Gaussian Surface:** We choose a cylindrical Gaussian surface with radius $r$ and length $L$, coaxial with the charged conductor.
* **Flux Calculation:**
    * The electric field $\vec{E}$ is radial and perpendicular to the curved surface of the cylinder.
    * The flux through the top and bottom circular ends of the cylinder is zero because $\vec{E}$ is parallel to these surfaces (or perpendicular to their area vectors).
    * The flux through the curved surface is $E \times (\text{area of curved surface}) = E (2\pi r L)$.
* **Enclosed Charge:** The charge enclosed within the Gaussian cylinder is $Q_{\text{enclosed}} = \lambda L$.
* **Applying Gauss's Law:**
    $$E (2\pi r L) = \frac{\lambda L}{\epsilon_0}$$   $$E = \frac{\lambda}{2\pi\epsilon_0 r}$$
* **Conclusion:** The electric field intensity due to an infinite line charge is inversely proportional to the distance $r$ from the line.

##### b) Electric Field Intensity due to a Plane Charged Sheet (Infinite Plane Sheet):

* **Setup:** Consider an infinitely large, thin, non-conducting plane sheet with a uniform surface charge density $\sigma$ (charge per unit area).
* **Gaussian Surface:** We choose a cylindrical Gaussian surface (or a rectangular box) that passes through the sheet, with its flat ends (cross-sectional area $A$) perpendicular to the sheet.
* **Flux Calculation:**
    * The electric field $\vec{E}$ is perpendicular to the sheet and points away from it (if positive charge) or towards it (if negative charge).
    * The flux through the curved surface of the cylinder is zero because $\vec{E}$ is parallel to the curved surface.
    * The flux passes only through the two flat ends of the cylinder. Since the field is uniform and perpendicular to these ends, the flux through each end is $EA$. Total flux is $EA + EA = 2EA$.
* **Enclosed Charge:** The charge enclosed by the Gaussian cylinder is $Q_{\text{enclosed}} = \sigma A$.
* **Applying Gauss's Law:**
    $$2EA = \frac{\sigma A}{\epsilon_0}$$   $$E = \frac{\sigma}{2\epsilon_0}$$
* **Conclusion:** The electric field intensity due to an infinite plane charged sheet is uniform (independent of distance from the sheet) and directed perpendicular to the sheet.

##### c) Electric Field Intensity due to a Charged Sphere (Spherical Shell or Solid Sphere):

Let's consider a uniformly charged non-conducting spherical shell of radius $R$ with total charge $Q$.

* **Case 1: Outside the Sphere ($r > R$)**
    * **Gaussian Surface:** A spherical Gaussian surface of radius $r$ concentric with the charged sphere.
    * **Flux Calculation:** The electric field $\vec{E}$ is radial and uniform over this surface. So, $\Phi_E = E (4\pi r^2)$.
    * **Enclosed Charge:** The total charge enclosed is $Q$.
    * **Applying Gauss's Law:**
        $$E (4\pi r^2) = \frac{Q}{\epsilon_0}$$       $$E = \frac{1}{4\pi\epsilon_0} \frac{Q}{r^2}$$
    * **Conclusion:** For points outside a uniformly charged sphere (or spherical shell), the electric field is the same as if all the charge were concentrated at its center (like a point charge).

* **Case 2: On the Surface of the Sphere ($r = R$)**
    * Substituting $r=R$ in the above formula:
        $$E = \frac{1}{4\pi\epsilon_0} \frac{Q}{R^2}$$

* **Case 3: Inside the Sphere ($r < R$)**
    * **For a uniformly charged *spherical shell* (charge only on the surface):**
        * **Gaussian Surface:** A spherical Gaussian surface of radius $r$ inside the shell.
        * **Enclosed Charge:** The charge enclosed within this Gaussian surface is $Q_{\text{enclosed}} = 0$, as all the charge is on the outer surface.
        * **Applying Gauss's Law:**
            $$E (4\pi r^2) = \frac{0}{\epsilon_0}$$           $$E = 0$$
        * **Conclusion:** The electric field inside a uniformly charged spherical shell is zero.

    * **For a uniformly charged *solid non-conducting sphere* (charge distributed throughout its volume):**
        * Let $\rho$ be the volume charge density ($Q = \frac{4}{3}\pi R^3 \rho$).
        * **Gaussian Surface:** A spherical Gaussian surface of radius $r < R$ inside the sphere.
        * **Enclosed Charge:** $Q_{\text{enclosed}} = \rho \times (\text{volume of Gaussian sphere}) = \rho (\frac{4}{3}\pi r^3)$.
        * **Applying Gauss's Law:**
            $$E (4\pi r^2) = \frac{\rho (\frac{4}{3}\pi r^3)}{\epsilon_0}$$           $$E = \frac{\rho r}{3\epsilon_0}$$
            Substituting $\rho = \frac{Q}{\frac{4}{3}\pi R^3}$:
            $$E = \frac{Q r}{4\pi\epsilon_0 R^3}$$
        * **Conclusion:** Inside a uniformly charged non-conducting solid sphere, the electric field intensity is directly proportional to the distance $r$ from the center. At the center ($r=0$), $E=0$.

---

### 8. Capacitor and its Working (संधारित्र और उसका कार्य)

A **capacitor** is a passive two-terminal electrical component that stores electrical energy in an electric field. It consists of two conducting plates separated by a dielectric (insulating material).

* **Working Principle:**
    * When a capacitor is connected to a battery (a voltage source), electrons flow from the negative terminal of the battery to one plate of the capacitor, making it negatively charged.
    * Simultaneously, electrons are pulled from the other plate of the capacitor by the positive terminal of the battery, leaving that plate positively charged.
    * This process continues until the potential difference across the capacitor plates becomes equal to the voltage of the battery.
    * An electric field is established between the plates, and electrical energy is stored in this electric field.
    * The capacitor now holds a charge ($Q$) and has a potential difference ($V$) across its plates.
    * When the capacitor is disconnected from the battery and connected to a load (e.g., a bulb), it discharges, releasing the stored energy.

* **Key Property:** Capacitors store charge and energy. They can release this energy quickly, making them useful for applications like flash photography, smoothing out voltage fluctuations, and tuning circuits.

---

### 9. Types of Capacitors (संधारित्र के प्रकार)

Capacitors come in various types, categorized by their dielectric material, construction, and applications. Some common types include:

1.  **Parallel Plate Capacitor:** The most basic and common type, consisting of two parallel conducting plates separated by a dielectric. (We will study this in detail).
2.  **Cylindrical Capacitor:** Consists of two coaxial cylinders separated by a dielectric.
3.  **Spherical Capacitor:** Consists of two concentric spherical shells separated by a dielectric.
4.  **Electrolytic Capacitors:** Have a very high capacitance for their size. They are polarized (have positive and negative terminals) and must be connected correctly. Used in power supplies for filtering.
5.  **Ceramic Capacitors:** Use ceramic material as dielectric. Small, inexpensive, and widely used in electronics.
6.  **Film Capacitors:** Use a plastic film as dielectric. Stable over temperature and frequency.
7.  **Variable Capacitors:** Allow their capacitance to be changed mechanically. Used in radio tuning circuits.

---

### 10. Capacitance and its Units (धारिता और उसकी इकाई)

* **Capacitance (C):**
    * **Definition:** Capacitance is a measure of a capacitor's ability to store electric charge. It is defined as the ratio of the magnitude of the charge ($Q$) on either conductor plate to the potential difference ($V$) between the conductors.
    * It indicates how much charge a capacitor can store for a given potential difference.
    * **Formula:**
        $$C = \frac{Q}{V}$$
        Where:
        * $C$ = Capacitance (in Farads, F)
        * $Q$ = Magnitude of charge on one plate (in Coulombs, C)
        * $V$ = Potential difference between the plates (in Volts, V)

* **Units:** The SI unit of capacitance is the **Farad (F)**.
    * One Farad is defined as the capacitance of a capacitor that stores one Coulomb of charge when the potential difference across its plates is one Volt.
    * 1 Farad = 1 Coulomb/Volt (1 C/V).
    * The Farad is a very large unit. Typically, capacitance is measured in sub-multiples:
        * microfarad ($\mu\text{F} = 10^{-6}$ F)
        * nanofarad ($\text{nF} = 10^{-9}$ F)
        * picofarad ($\text{pF} = 10^{-12}$ F)

---

### 11. Capacitance of a Parallel Plate Capacitor (समानांतर प्लेट संधारित्र की धारिता)

A parallel plate capacitor consists of two large, flat, parallel conducting plates, each of area $A$, separated by a small distance $d$.

* **Derivation:**
    1.  **Electric Field between Plates:**
        When charges $+Q$ and $-Q$ are on the plates, a uniform electric field $E$ is created between them. For large plates and small separation, we can use the formula for the electric field due to a plane charged sheet, but here we have two sheets (one positive, one negative). The field due to the positive plate is $\sigma/(2\epsilon_0)$ away from it, and due to the negative plate is $\sigma/(2\epsilon_0)$ towards it. Both fields add up in the region between the plates.
        So, the total electric field $E$ between the plates is:
        $$E = \frac{\sigma}{\epsilon_0}$$
        Where $\sigma = Q/A$ is the surface charge density.
        $$E = \frac{Q}{A\epsilon_0}$$
    2.  **Potential Difference between Plates:**
        For a uniform electric field, the potential difference $V$ between the plates separated by distance $d$ is:
        $$V = Ed$$
        Substituting the value of $E$:
        $$V = \left(\frac{Q}{A\epsilon_0}\right) d$$       $$V = \frac{Qd}{A\epsilon_0}$$
    3.  **Capacitance:**
        Now, use the definition of capacitance $C = Q/V$:
        $$C = \frac{Q}{\left(\frac{Qd}{A\epsilon_0}\right)}$$       $$C = \frac{A\epsilon_0}{d}$$

* **Formula:** The capacitance of a parallel plate capacitor in vacuum or air is:
    $$C_0 = \frac{\epsilon_0 A}{d}$$
    Where:
    * $C_0$ = Capacitance in vacuum/air (in Farads)
    * $\epsilon_0$ = Permittivity of free space ($\approx 8.854 \times 10^{-12}$ F/m)
    * $A$ = Area of one of the plates (in m$^2$)
    * $d$ = Distance between the plates (in m)

* **Factors Affecting Capacitance:**
    * **Area of plates ($A$):** Capacitance is directly proportional to the area of the plates. Larger plates store more charge.
    * **Distance between plates ($d$):** Capacitance is inversely proportional to the distance between the plates. Smaller separation allows for a stronger field and thus more charge storage for a given voltage.
    * **Dielectric medium:** The presence of a dielectric material between the plates significantly affects capacitance (explained below).

---

### 12. Series and Parallel Combination of Capacitors (संधारित्रों का श्रेणी और समानांतर संयोजन)

Capacitors can be combined in circuits in series or parallel configurations.

#### a) Series Combination (श्रेणी क्रम संयोजन):

* **Arrangement:** Capacitors are connected end-to-end, forming a single path for charge flow.
* **Key Properties:**
    * **Charge:** The charge ($Q$) on each capacitor in a series combination is the *same*.
    * **Voltage:** The total potential difference ($V$) across the combination is the *sum* of the potential differences across individual capacitors: $V = V_1 + V_2 + V_3 + \ldots$.
* **Equivalent Capacitance ($C_{\text{eq}}$) Derivation:**
    We know $V = Q/C$. So, $V_1 = Q/C_1$, $V_2 = Q/C_2$, etc.
    Substituting into the voltage sum:
    $$\frac{Q}{C_{\text{eq}}} = \frac{Q}{C_1} + \frac{Q}{C_2} + \frac{Q}{C_3} + \ldots$$
    Dividing by $Q$:
    $$\frac{1}{C_{\text{eq}}} = \frac{1}{C_1} + \frac{1}{C_2} + \frac{1}{C_3} + \ldots$$
* **Formula:** For capacitors in series, the reciprocal of the equivalent capacitance is the sum of the reciprocals of individual capacitances.
    * The equivalent capacitance in series is *always less* than the smallest individual capacitance.

#### b) Parallel Combination (समानांतर क्रम संयोजन):

* **Arrangement:** Capacitors are connected across the same two points, so their plates are effectively connected to the same voltage source.
* **Key Properties:**
    * **Voltage:** The potential difference ($V$) across each capacitor in a parallel combination is the *same*.
    * **Charge:** The total charge ($Q$) stored in the combination is the *sum* of the charges stored on individual capacitors: $Q = Q_1 + Q_2 + Q_3 + \ldots$.
* **Equivalent Capacitance ($C_{\text{eq}}$) Derivation:**
    We know $Q = CV$. So, $Q_1 = C_1 V$, $Q_2 = C_2 V$, etc.
    Substituting into the charge sum:
    $$C_{\text{eq}} V = C_1 V + C_2 V + C_3 V + \ldots$$
    Dividing by $V$:
    $$C_{\text{eq}} = C_1 + C_2 + C_3 + \ldots$$
* **Formula:** For capacitors in parallel, the equivalent capacitance is the direct sum of the individual capacitances.
    * The equivalent capacitance in parallel is *always greater* than the largest individual capacitance.

---

### 13. Dielectric and its Effect on Capacitance (परावैद्युत और उसका धारिता पर प्रभाव)

A **dielectric** is an electrical insulator that can be polarized by an applied electric field. When a dielectric material is inserted between the plates of a capacitor, it enhances the capacitor's ability to store charge.

* **How Dielectrics Work:**
    * When an external electric field is applied across a dielectric material, the molecules within the dielectric (which can be polar or non-polar) reorient or stretch.
    * This reorientation/stretching leads to the formation of induced dipoles within the dielectric.
    * These induced dipoles create an *internal electric field* within the dielectric that opposes the applied external electric field.
    * The net electric field *inside* the dielectric is therefore reduced compared to the field in vacuum.
    * Since $V = Ed$, if $E$ is reduced for the same distance $d$, the potential difference $V$ across the capacitor plates for a given charge $Q$ is reduced.
    * As $C = Q/V$, if $V$ decreases for a given $Q$, the capacitance $C$ **increases**.

* **Dielectric Constant ($\kappa$ or $\epsilon_r$):**
    * The dielectric constant (also called relative permittivity) is a dimensionless factor that describes how much the capacitance of a capacitor increases when a dielectric material fills the space between its plates, compared to when there is a vacuum.
    * **Definition:** $\kappa = \frac{C_{\text{dielectric}}}{C_{\text{vacuum}}}$
    * It is also defined as the ratio of the permittivity of the dielectric material ($\epsilon$) to the permittivity of free space ($\epsilon_0$):
        $$\kappa = \frac{\epsilon}{\epsilon_0}$$
* **Capacitance with Dielectric:**
    If a dielectric with dielectric constant $\kappa$ is completely filled between the plates of a parallel plate capacitor, its capacitance becomes:
    $$C = \kappa C_0 = \frac{\kappa \epsilon_0 A}{d}$$
    * Since $\kappa > 1$ for all dielectrics, the capacitance always increases when a dielectric is inserted.

* **Energy Storage with Dielectric:** A dielectric also helps in storing more energy for a given voltage, as $U = \frac{1}{2}CV^2$. Since C increases, U increases.

---

### 14. Dielectric Breakdown (परावैद्युत भंजन)

* **Definition:** Dielectric breakdown is the phenomenon where an insulating dielectric material, under the influence of a very strong electric field, suddenly loses its insulating properties and starts conducting electricity.
* **Mechanism:** When the electric field across the dielectric becomes excessively strong, it can pull electrons away from the atoms or molecules of the dielectric material. These free electrons gain enough energy to collide with other atoms, ionizing them and creating more free electrons. This avalanche process leads to a sudden large flow of current through the dielectric, effectively turning it into a conductor.
* **Dielectric Strength:** The **dielectric strength** of a material is the maximum electric field an insulating material can withstand without undergoing dielectric breakdown. It is usually measured in Volts per meter (V/m) or kV/mm.
* **Consequences:** Dielectric breakdown permanently damages the dielectric material in most cases, making the capacitor useless. It often leads to a short circuit in the capacitor.
* **Importance:** Understanding dielectric strength is crucial in designing capacitors and other electrical components to ensure they can operate safely within their voltage limits without failure.

---

This covers all the topics from Unit 3: Electrostatics in detail. Let me know if you need more clarity on any specific point or have further questions!
