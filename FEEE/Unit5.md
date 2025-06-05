# 📘 UNIT V: A.C. Circuits

---

## 🔹 1. Basic Terms of A.C. Circuits

| Term           | Meaning                                             | Formula/Definition                        |
|----------------|-----------------------------------------------------|------------------------------------------|
| **Cycle**      | One complete oscillation of AC waveform              |                                          |
| **Frequency (f)** | Number of cycles per second                          | f = 1 / T (Hz)                           |
| **Periodic Time (T)** | Time for one complete cycle                         | T = 1 / f (seconds)                      |
| **Amplitude (Vm or Im)** | Maximum value of voltage/current                  |                                          |
| **Angular Velocity (ω)** | Rate of change of angle in radians per second     | ω = 2πf (rad/s)                         |
| **RMS Value**  | Root Mean Square value - effective value of AC         | Vrms = Vm / √2                           |
| **Average Value** | Average of instantaneous values over half cycle       | Vavg = (2Vm) / π                         |
| **Form Factor** | Ratio of RMS value to average value                    | Form Factor = Vrms / Vavg ≈ 1.11         |
| **Peak Factor** | Ratio of peak value to RMS value                        | Peak Factor = Vm / Vrms ≈ 1.414           |

---

## 🔹 2. Impedance (Z), Phase Angle (ϕ), and Power Factor (pf)

- **Impedance (Z):** Total opposition to AC, combining resistance and reactance.
```
Z = √(R² + (X_L - X_C)²)
```
Where,
- R = resistance,
- X_L = inductive reactance = ωL,
- X_C = capacitive reactance = 1 / (ωC).

- **Phase Angle (ϕ):**
```
tan ϕ = (X_L - X_C) / R
```
- ϕ indicates phase difference between voltage and current.

- **Power Factor (pf):**
```
pf = cos ϕ = P / (Vrms × Irms)
```
- Power factor shows how effectively the current is converted into useful work.

---

## 🔹 3. Mathematical and Phasor Representation of Alternating emf and Current

- Instantaneous voltage:
```
v = Vm × sin(ωt)
```
- Instantaneous current:
```
i = Im × sin(ωt ± ϕ)
```
- **Phasors** are rotating vectors representing sinusoidal quantities.

---

## 🔹 4. Voltage and Current in Star and Delta Connections

| Connection | Voltage Relation                   | Current Relation                  |
|------------|----------------------------------|---------------------------------|
| Star (Y)   | Phase Voltage (Vph) = Line Voltage (VL) / √3 | Line Current (IL) = Phase Current (Iph) |
| Delta (Δ)  | Line Voltage (VL) = Phase Voltage (Vph)     | Line Current (IL) = √3 × Phase Current (Iph) |

---

## 🔹 5. A.C. Circuits with Different Elements

### 🔸 (a) Resistor (R)
- Voltage and current are **in phase** (ϕ = 0°).
- Impedance: Z = R

### 🔸 (b) Inductor (L)
- Current **lags voltage** by 90° (ϕ = +90°).
- Inductive reactance:  
```
X_L = ωL = 2πfL
```
- Impedance: Z = jX_L

### 🔸 (c) Capacitor (C)
- Current **leads voltage** by 90° (ϕ = -90°).
- Capacitive reactance:  
```
X_C = 1 / (ωC) = 1 / (2πfC)
```
- Impedance: Z = -jX_C

---

## 🔹 6. Series and Parallel AC Circuits

### 🔸 (a) R-L Series Circuit
- Total impedance:  
```
Z = √(R² + X_L²)
```
- Phase angle:  
```
tan ϕ = X_L / R
```

### 🔸 (b) R-C Series Circuit
- Total impedance:  
```
Z = √(R² + X_C²)
```
- Phase angle:  
```
tan ϕ = -X_C / R
```

### 🔸 (c) R-L-C Series Circuit
- Total impedance:  
```
Z = √[R² + (X_L - X_C)²]
```
- Phase angle:  
```
tan ϕ = (X_L - X_C) / R
```

### 🔸 (d) Parallel Circuits
- Total admittance (Y) is sum of admittances of R, L, and C branches.

---

## 🔹 7. Power in AC Circuits and Power Triangle

- **Real Power (P):**  
Power actually consumed  
```
P = Vrms × Irms × cos ϕ
```

- **Reactive Power (Q):**  
Power stored and returned  
```
Q = Vrms × Irms × sin ϕ
```

- **Apparent Power (S):**  
Product of Vrms and Irms  
```
S = Vrms × Irms
```

### Power Triangle:

```
       Q (Reactive Power)
          |
          |  
          |____ P (Real Power)
          \___ S (Apparent Power)
```

- Relationship:  
```
S² = P² + Q²
```

---

## ✅ Exam Tips:
- Understand definitions and differences between RMS, average, peak values.
- Practice impedance and phase angle calculations.
- Know voltage/current relations in Star and Delta connections.
- Be able to draw and explain power triangle.
- Solve problems on series RLC circuits.

---

*This unit is a mix of formulas, concepts, and phasor diagrams, so practice numerical problems along with theory.*

