# 📘 UNIT III: Overview of Digital Electronics

## 🔹 1. Boolean Algebra

### 🔸 What is Boolean Algebra?
A mathematical system to perform logical operations using binary variables (0 or 1).

### 🔸 Basic Boolean Operations:

| Operation | Symbol | Description                        |
|-----------|--------|------------------------------------|
| AND       | A·B or AB | Output is 1 only if both inputs are 1 |
| OR        | A + B  | Output is 1 if at least one input is 1 |
| NOT       | A̅      | Inverts the input (1 becomes 0, 0 becomes 1) |

---

### 🔸 Basic Laws of Boolean Algebra:
- Identity:  
  ```
  A + 0 = A, A · 1 = A
  ```
- Null Law:  
  ```
  A + 1 = 1, A · 0 = 0
  ```
- Inverse Law:  
  ```
  A + A̅ = 1, A · A̅ = 0
  ```
- Idempotent Law:  
  ```
  A + A = A, A · A = A
  ```
- Distributive Law:  
  ```
  A · (B + C) = A·B + A·C
  ```

---

## 🔹 2. Electronic Implementation of Boolean Operations

Boolean logic can be implemented using **logic gates** in hardware, using **transistors and ICs**.

---

## 🔹 3. Logic Gates – Functional Block Approach

### 🔸 Basic Gates:

| Gate | Symbol | Expression | Truth Table (A, B → Output) |
|------|--------|------------|-----------------------------|
| AND  | A·B    | A · B      | 0,0→0 | 0,1→0 | 1,0→0 | 1,1→1 |
| OR   | A+B    | A + B      | 0,0→0 | 0,1→1 | 1,0→1 | 1,1→1 |
| NOT  | A̅     | ¬A         | 0→1   | 1→0                   |

### 🔸 Universal Gates:
- **NAND** and **NOR** can be used to implement any logic function.

### 🔸 Derived Gates:
- **XOR (Exclusive OR):**
  ```
  A ⊕ B = A̅·B + A·B̅
  ```
- **XNOR (Exclusive NOR):**
  ```
  A ⊕ B̅ = A·B + A̅·B̅
  ```

---

## 🔹 4. Storage Elements – Flip-Flops (Functional Block Approach)

### 🔸 What is a Flip-Flop?
A **bistable device** used to store one bit of digital data. Output changes based on input and clock.

### 🔸 Types of Flip-Flops:

| Type | Symbol | Description                     |
|------|--------|---------------------------------|
| SR   | Set-Reset | Sets or resets output         |
| D    | Data     | Transfers input to output on clock |
| T    | Toggle   | Toggles output on each clock cycle |
| JK   | Jack-Kilby | Universal FF (combination of SR + T) |

- **D Flip-Flop Truth Table:**
  | Clock | D | Q (Next State) |
  |-------|---|----------------|
  | ↑     | 0 | 0              |
  | ↑     | 1 | 1              |

---

## 🔹 5. Counters

### 🔸 (a) Ripple Counter
- Also called **Asynchronous counter**
- Flip-flops are triggered one after another.
- Slow, but simple to design.

### 🔸 (b) Up/Down Counter
- Can count **upward or downward** based on control input.
- Used in digital clocks, timers.

### 🔸 (c) Decade Counter
- Counts from 0 to 9 (10 states)
- Resets after reaching 9.
- Used in digital displays.

---

## 🔹 6. Introduction to Digital IC Gates (TTL Type)

### 🔸 TTL (Transistor-Transistor Logic)
- A type of digital logic family built using bipolar junction transistors.

### 🔸 Features of TTL:
- Operates at 5V
- Fast switching speed (~10 ns)
- Low power consumption (compared to earlier technologies)

### 🔸 Examples of TTL ICs:
| IC No.  | Function           |
|--------|--------------------|
| 7400   | Quad 2-input NAND  |
| 7402   | Quad 2-input NOR   |
| 7404   | Hex Inverter       |
| 7486   | Quad XOR Gate      |
| 7476   | JK Flip-Flop       |

---

## ✅ Summary Points for Exam:
- **Boolean laws and gates** form the foundation of digital logic.
- **Flip-flops** are memory elements; types include SR, D, T, JK.
- **Counters** are sequential logic circuits used to count pulses.
- **TTL ICs** are standard gate ICs — learn a few common numbers like 7400, 7404.

🧠 *Useful for MCQs, short/long theory, and logic circuit design questions.*

