# 📘 UNIT II: Overview of Analog Circuits

## 🔹 1. Operational Amplifiers (Op-Amps)

### 🔸 What is an Op-Amp?
An **Operational Amplifier (Op-Amp)** is a high-gain voltage amplifier with **differential inputs** and usually a **single-ended output**.

- Symbol:

       +Vcc
         |
     In- |\
         | >---- Output
     In+ |/
         |
       -Vcc

- **Inverting Input**: (–)
- **Non-Inverting Input**: (+)

---

### 🔸 Ideal Op-Amp Characteristics
An ideal Op-Amp is a **theoretical model** with perfect behavior:

| Parameter                     | Ideal Value      |
|------------------------------|------------------|
| Input Impedance              | ∞ (infinite)      |
| Output Impedance             | 0                |
| Open-Loop Gain (A_OL)        | ∞                |
| Bandwidth                    | ∞                |
| Offset Voltage               | 0                |
| Common Mode Rejection Ratio | ∞                |
| Slew Rate                    | ∞                |

---

### 🔸 Practical Op-Amp Characteristics
Real Op-Amps (like 741 IC) differ slightly from ideal:

| Parameter                     | Typical Value     |
|------------------------------|-------------------|
| Input Impedance              | ~1 MΩ to 10 MΩ     |
| Output Impedance             | ~100 Ω             |
| Open-Loop Gain               | ~10⁵ to 10⁶        |
| Bandwidth                    | Limited (~MHz)     |
| Slew Rate                    | Limited (~0.5V/µs) |

---

## 🔹 2. Op-Amp Configurations

### 🔸 (a) Open-Loop Configuration
- No feedback is used.
- Extremely high gain (~10⁵), output saturates easily.
- Not used for linear applications.

### 🔸 (b) Closed-Loop Configuration
- Feedback is applied from output to input.
- Controlled gain, stable operation.
- **Used in amplifiers, filters, integrators, etc.**

---

## 🔹 3. Applications of Op-Amps

### 🔸 (a) Inverting Amplifier
- Input applied to inverting terminal.
- Gain is negative → output is 180° out of phase.

```
Voltage Gain: A_V = -Rf / Rin
```

- Rf = Feedback resistor
- Rin = Input resistor

### 🔸 (b) Non-Inverting Amplifier
- Input applied to non-inverting terminal.
- Output is in-phase with input.

```
Voltage Gain: A_V = 1 + (Rf / Rin)
```

---

### 🔸 (c) Adder (Summing Amplifier)
- Adds multiple input voltages.
- Usually inverting type.

```
Vout = -Rf × (V1/R1 + V2/R2 + V3/R3 + ...)
```

- Used in audio mixers, analog computers

---

### 🔸 (d) Differentiator
- Output = derivative of input.
- Circuit uses capacitor at input.

```
Vout = -RC × (dVin/dt)
```

- **Use:** Edge detectors, wave shaping

---

### 🔸 (e) Integrator
- Output = integral of input.
- Capacitor is used in feedback.

```
Vout = -(1/RC) × ∫Vin dt
```

- **Use:** Signal integration, waveform generation

---

## ✅ Summary Points for Exams:
- Know the **symbol and terminals** of Op-Amp.
- Memorize **ideal vs practical** differences.
- Learn **gain formulas** for inverting/non-inverting.
- Understand **adder, integrator, differentiator circuits** with use cases.
- Draw and label **circuit diagrams** if asked in theory.

📘 *Perfect for both short answers (definitions, formulas) and long answers (diagrams, derivations).*
