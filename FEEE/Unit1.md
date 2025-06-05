# 📘 UNIT I: Overview of Electronic Components & Signals

## 🔹 1. Passive and Active Components

### 🔸 Passive Components
These components **do not generate energy** but can **store or dissipate** it.

#### 🔹 (a) Resistor
- Opposes the flow of electric current.
- Follows **Ohm’s Law**:
  ```
  V = I × R
  ```
- **Unit:** Ohm (Ω)
- **Types:** Fixed, Variable (e.g., Potentiometer)
- **Applications:** Voltage division, current limiting, biasing

#### 🔹 (b) Capacitor
- Stores electrical energy in an electric field.
- Charge and voltage relation:
  ```
  Q = C × V
  ```
- **Unit:** Farad (F)
- **Types:** Ceramic, Electrolytic, Film
- **Applications:** Filtering, AC coupling, timing circuits

#### 🔹 (c) Inductor
- Stores energy in a magnetic field when current flows through it.
- Voltage-current relation:
  ```
  V = L × (dI/dt)
  ```
- **Unit:** Henry (H)
- **Types:** Air-core, Iron-core
- **Applications:** Filters, transformers, energy storage in power supplies

---

### 🔸 Active Components
These components **can amplify, control, or generate** electrical signals.

#### 🔹 (a) Diode
- Allows current to flow in **one direction only**.
- **Symbol:** →|—
- **Types:** PN junction, Zener, LED, Photodiode
- **Applications:** Rectification, voltage regulation, signal demodulation

#### 🔹 (b) BJT (Bipolar Junction Transistor)
- Current-controlled device used for amplification and switching.
- **Types:** NPN and PNP
- **Basic formula:**
  ```
  IC = β × IB
  ```
- **Applications:** Amplifiers, switches, oscillators

#### 🔹 (c) FET (Field Effect Transistor)
- Voltage-controlled device with high input impedance.
- **Types:** JFET, MOSFET

#### 🔹 (d) MOSFET (Metal-Oxide-Semiconductor FET)
- Widely used in digital circuits and power electronics.
- **Types:** Enhancement-mode, Depletion-mode
- **Applications:** Switching, power control, logic gates

#### 🔹 (e) CMOS (Complementary MOS)
- Combination of p-type and n-type MOSFETs.
- **Low power consumption** and high noise immunity.
- **Applications:** Microprocessors, digital ICs

---

## 🔹 2. Signals

### 🔸 (a) Types of Signals

#### 🔹 DC (Direct Current)
- Constant value over time.
- Example: Battery voltage

#### 🔹 AC (Alternating Current)
- Varies with time, usually in sine wave form.
- Example: Household supply (230V, 50Hz)

#### 🔹 Voltage vs Current
- **Voltage (V):** Potential difference
- **Current (I):** Rate of charge flow

#### 🔹 Periodic Signals
- Repeats after a fixed time period (T)
- Examples: Sine, square, triangular waves

#### 🔹 Non-Periodic Signals
- Do not repeat
- Examples: Random or noise signals

---

### 🔸 (b) Signal Values

#### 🔹 Average Value (V_avg)
- Mean value over one cycle (mainly for rectified signals)

#### 🔹 RMS Value (V_rms)
- Equivalent DC value that produces same power
  ```
  V_rms = V_peak / √2  (for sine wave)
  ```

#### 🔹 Peak Value (V_peak)
- Maximum value of the signal waveform

---

## 🔹 3. Sources

### 🔸 (a) Ideal Sources
- Provide constant voltage or current regardless of load.
- **Ideal voltage source:** Zero internal resistance
- **Ideal current source:** Infinite internal resistance

### 🔸 (b) Non-Ideal Sources
- Real sources have internal resistance, so output varies with load.

### 🔸 (c) Independent Sources
- Provide voltage or current without depending on other circuit variables.

### 🔸 (d) Dependent (Controlled) Sources
- Output depends on some voltage or current in the circuit.
- Types:
  - Voltage-Controlled Voltage Source (VCVS)
  - Voltage-Controlled Current Source (VCCS)
  - Current-Controlled Voltage Source (CCVS)
  - Current-Controlled Current Source (CCCS)

---

✅ **Summary Points:**
- Understand each component's function and symbol.
- Memorize key formulas (Ohm’s law, capacitor, inductor).
- Know waveform characteristics and values (RMS, average, peak).
- Understand ideal vs practical sources and signal types.

📚 Ideal for short and long answer questions in exams!

