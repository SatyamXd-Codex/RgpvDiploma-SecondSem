# 🔌 UNIT I: Overview of Electronic Components & Signals
## इलेक्ट्रॉनिक कॉम्पोनेंट्स और सिग्नल्स का ओवरव्यू

### 📚 Unit Introduction | यूनिट परिचय

This comprehensive unit introduces the fundamental concepts in electronics, covering both the basic building blocks (components) and the nature of electrical quantities (signals). Ye unit electronics ki foundation hai - components aur signals ko detail mein samjhayenge.

**यह यूनिट क्यों महत्वपूर्ण है? (Why is this unit important?)**
- Electronics के basic building blocks समझने के लिए
- Circuit analysis ki foundation बनाने के लिए
- Practical applications में components कैसे काम करते हैं
- Exam preparation के लिए core concepts

### 🎯 Learning Objectives | सीखने के उद्देश्य

After completing this unit, students will be able to:
- Classify and understand passive vs active components
- Analyze different types of electrical signals
- Calculate average, RMS, and peak values
- Understand ideal and practical sources
- Apply component knowledge in circuit analysis

**इस यूनिट के बाद आप जान जाएंगे:**
- Passive aur active components में क्या अंतर है
- Different signals कैसे काम करते हैं
- Calculations कैसे करते हैं
- Real-world applications कहाँ मिलते हैं

---

## 🧩 I. Passive & Active Components | पैसिव और एक्टिव कॉम्पोनेंट्स

Electronic components are broadly classified into two categories based on their ability to control or generate power.

**Components का classification क्यों जरूरी है?**
- Circuit design में proper selection के लिए
- Power requirements समझने के लिए  
- Cost और efficiency optimize करने के लिए

```
📊 Component Classification:
    ┌─────────────────────────────────────┐
    │        Electronic Components        │
    └─────────────┬───────────────────────┘
                  │
        ┌─────────┴─────────┐
        │                   │
   ┌────▼────┐       ┌─────▼─────┐
   │ PASSIVE │       │  ACTIVE   │
   └─────────┘       └───────────┘
        │                   │
   ┌────▼────┐       ┌─────▼─────┐
   │R, L, C  │       │Diode,Transistor│
   └─────────┘       └───────────┘
```

### 🔋 A. Passive Components | पैसिव कॉम्पोनेंट्स

**Definition | परिभाषा:**
Passive components are those that do not require an external power source to operate and cannot amplify or generate a signal. They either dissipate, store, or filter electrical energy.

**Passive components वे होते हैं जो:**
- बाहरी power source की जरूरत नहीं होती
- Signal को amplify नहीं कर सकते
- केवल energy को dissipate, store या filter करते हैं

**🔑 Key Characteristics:**
- No external power needed
- Cannot provide gain
- Linear behavior (mostly)
- Energy storage or dissipation

**मुख्य विशेषताएं:**
- कोई external power नहीं चाहिए
- Gain प्रदान नहीं कर सकते
- ज्यादातर linear behavior
- Energy store या dissipate करते हैं

#### 🎯 1. Resistances (Resistors) | प्रतिरोध (रेसिस्टर)

**Definition | परिभाषा:**
A resistor is a two-terminal passive electronic component that opposes the flow of electric current. It dissipates electrical energy as heat.

**Resistor एक ऐसा component है जो:**
- Current के flow को oppose करता है
- Electrical energy को heat में convert करता है
- Circuit में current को control करता है

**Symbol | चिह्न:** 
```
   ----/\/\/\/\----  (Zig-zag line)
   या
   ----[    ]----    (Rectangle)
```

**Unit | इकाई:** Ohm (Ω) - ओम

**🔬 Working Principle | कार्य सिद्धांत:**

Based on Ohm's Law. When voltage is applied across a resistor, current flows through it, and energy is lost as heat due to collisions between electrons and atoms in the material.

**काम कैसे करता है:**
- Voltage apply करने पर current flow होता है
- Electrons और atoms के बीच collision होती है
- Energy heat के रूप में निकलती है
- यही resistance का principle है

**📐 Fundamental Formulas | मूल सूत्र:**

**Ohm's Law | ओम का नियम:**
```
V = I × R
```
Where | जहाँ:
- V = Voltage across resistor (Volts) | रेसिस्टर के across voltage
- I = Current through resistor (Amperes) | रेसिस्टर से होकर बहने वाला current  
- R = Resistance (Ohms) | प्रतिरोध

**Power Dissipation | शक्ति अपव्यय:**
```
P = V × I = I² × R = V²/R
```

**📊 Practical Examples | व्यावहारिक उदाहरण:**

1. **LED Current Limiting:**
   - अगर LED को 20mA current चाहिए और supply 5V है
   - LED का forward voltage 2V है
   - R = (5V - 2V) / 0.02A = 150Ω

2. **Voltage Divider:**
   ```
   Input ----[R1]----+----[R2]---- Ground
                     |
                   Output
   ```
   - Output = Input × (R2/(R1+R2))

**🎯 Applications | अनुप्रयोग:**
- Current limiting (LED circuits में)
- Voltage division (sensor circuits में)
- Pull-up/pull-down resistors (digital circuits में)
- Timing circuits (capacitors के साथ)
- Heat generation (heaters में)

**💡 Exam Important Points:**
- Ohm's law सबसे important है
- Power formulas याद रखें
- Color code पढ़ना आना चाहिए
- Series में resistance add होते हैं
- Parallel में 1/R add होते हैं

#### ⚡ 2. Capacitors | संधारित्र (कैपेसिटर)

**Definition | परिभाषा:**
A capacitor is a two-terminal passive electronic component that stores electrical energy in an electric field. It consists of two conductive plates separated by a dielectric (insulating) material.

**Capacitor एक ऐसा component है जो:**
- Electric field में energy store करता है
- दो conducting plates होती हैं
- Dielectric material से separated होती हैं
- Sudden voltage changes को oppose करता है

**Symbol | चिह्न:** 
```
   ----| |----  (Parallel lines - Non-polarized)
   ----| (----  (Curved line - Polarized/Electrolytic)
```

**Unit | इकाई:** Farad (F) - फैराड

**🔬 Working Principle | कार्य सिद्धांत:**

When voltage is applied across a capacitor, charge accumulates on the plates, creating an electric field between them. The capacitor stores this charge and thus energy. It opposes sudden changes in voltage.

**काम कैसे करता है:**
- Voltage apply करने पर plates पर charge जमा होता है
- Plates के बीच electric field बनता है
- Energy store होती है electric field में
- Sudden voltage changes को oppose करता है

**📐 Fundamental Formulas | मूल सूत्र:**

**Charge Storage | चार्ज संग्रहण:**
```
Q = C × V
```
Where | जहाँ:
- Q = Charge stored (Coulombs) | संग्रहीत चार्ज
- C = Capacitance (Farads) | धारिता
- V = Voltage across capacitor | कैपेसिटर के across voltage

**Current-Voltage Relationship:**
```
I = C × (dV/dt)
```
**Energy Stored | संग्रहीत ऊर्जा:**
```
E = ½CV² = ½QV = ½Q²/C
```

**📊 Types of Capacitors | कैपेसिटर के प्रकार:**

1. **Ceramic Capacitors:**
   - Small values (pF to μF)
   - Non-polarized
   - सबसे common type

2. **Electrolytic Capacitors:**
   - Large values (μF to F)
   - Polarized (+ और - terminal)
   - Power supply filtering में use

3. **Tantalum Capacitors:**
   - Stable और reliable
   - छोटे size में high capacitance

**🎯 Behavior in Circuits:**

**DC Circuit में:**
- Initially acts as short circuit
- Finally acts as open circuit
- Charging और discharging होता है

**AC Circuit में:**
- Continuously charges and discharges
- Reactive power consume करता है
- Capacitive reactance: Xc = 1/(2πfC)

**📊 Practical Examples | व्यावहारिक उदाहरण:**

1. **Power Supply Filtering:**
   - Ripple voltage को smooth करता है
   - DC supply में AC components को filter करता है

2. **Coupling/Decoupling:**
   - AC signals को pass करता है
   - DC को block करता है

3. **Timing Circuits:**
   - RC time constant = R × C
   - Charging time = 5RC (approximately)

**🎯 Applications | अनुप्रयोग:**
- Power supply filtering (smooth DC output)
- Coupling/decoupling circuits (AC pass, DC block)
- Timing circuits (delays और oscillators)
- Energy storage (camera flash, power backup)
- Motor starting (single phase motors)
- Frequency selection (tuned circuits)

**💡 Exam Important Points:**
- Q = CV formula must remember
- Energy formula = ½CV²
- DC में final state open circuit
- AC में reactance Xc = 1/(2πfC)
- Series में 1/C add होते हैं
- Parallel में C add होते हैं

#### 🌀 3. Inductors | प्रेरकत्व (इंडक्टर)

**Definition | परिभाषा:**
An inductor is a two-terminal passive electronic component that stores energy in a magnetic field when electric current flows through it. It typically consists of a coil of wire.

**Inductor एक ऐसा component है जो:**
- Magnetic field में energy store करता है
- Coil of wire होता है (तार की कुंडली)
- Current के sudden changes को oppose करता है
- Electromagnetic induction के principle पर काम करता है

**Symbol | चिह्न:** 
```
   ----∩∩∩∩----  (Coil/helix shape)
   या
   ----⋀⋀⋀⋀----  (Series of arcs)
```

**Unit | इकाई:** Henry (H) - हेनरी

**🔬 Working Principle | कार्य सिद्धांत:**

When current flows through an inductor, it creates a magnetic field. Any change in current causes a change in magnetic field, which induces an EMF that opposes the change in current (Lenz's Law).

**काम कैसे करता है:**
- Current flow करने से magnetic field बनता है
- Current change होने पर magnetic field भी change होता है
- इससे EMF induce होता है (Faraday's Law)
- यह EMF current change को oppose करता है (Lenz's Law)

**📐 Fundamental Formulas | मूल सूत्र:**

**Magnetic Flux Linkage:**
```
Φ = L × I
```
Where | जहाँ:
- Φ = Magnetic flux linkage (Weber-turns) | चुंबकीय फ्लक्स लिंकेज
- L = Inductance (Henries) | प्रेरकत्व
- I = Current through inductor | इंडक्टर से होकर बहने वाला current

**Voltage-Current Relationship:**
```
V = L × (dI/dt)
```

**Energy Stored | संग्रहीत ऊर्जा:**
```
E = ½LI²
```

**📊 Types of Inductors | इंडक्टर के प्रकार:**

1. **Air Core Inductors:**
   - कोई magnetic core नहीं
   - Low inductance values
   - High frequency applications

2. **Iron Core Inductors:**
   - Iron core के साथ
   - High inductance values
   - Low frequency applications

3. **Ferrite Core Inductors:**
   - Ferrite material core
   - Medium inductance
   - RF applications

**🎯 Behavior in Circuits:**

**DC Circuit में:**
- Initially acts as open circuit
- Finally acts as short circuit
- Current gradually increases

**AC Circuit में:**
- Inductive reactance: XL = 2πfL
- Current lags voltage by 90°
- Reactive power consume करता है

**📊 Practical Examples | व्यावहारिक उदाहरण:**

1. **Choke Coil:**
   - AC को block करता है, DC को pass करता है
   - Power supplies में filtering

2. **Transformer:**
   - दो inductors electromagnetically coupled
   - Voltage step-up या step-down

3. **Motor Windings:**
   - Rotating magnetic field create करने के लिए

**🎯 Applications | अनुप्रयोग:**
- Filters (AC block, DC pass करने के लिए)
- Chokes (unwanted AC components को remove करने के लिए)
- Energy storage (switching power supplies में)
- Resonant circuits (LC oscillators)
- Transformers (voltage conversion)
- Motor windings (electromagnetic motors)

**💡 Exam Important Points:**
- V = L(dI/dt) formula important है
- Energy = ½LI²
- DC में final state short circuit
- AC में reactance XL = 2πfL
- Series में L add होते हैं
- Parallel में 1/L add होते हैं
- Lenz's law - opposes change in current

---

### ⚡ B. Active Components | एक्टिव कॉम्पोनेंट्स

**Definition | परिभाषा:**
Active components are those that require an external power source to operate and can amplify or generate a signal. They exhibit control over current or voltage.

**Active components वे होते हैं जो:**
- External power source की जरूरत होती है
- Signal को amplify कर सकते हैं
- Current या voltage को control कर सकते हैं
- Switching और amplification के लिए use होते हैं

**🔑 Key Characteristics:**
- Need external power supply
- Can provide gain (amplification)
- Non-linear behavior
- Control and switching capabilities

**मुख्य विशेषताएं:**
- External power की जरूरत
- Gain provide कर सकते हैं
- Non-linear behavior
- Control और switching capabilities

```
📊 Active Components Overview:
    ┌─────────────────────────────────────┐
    │        Active Components            │
    └─────────────┬───────────────────────┘
                  │
        ┌─────────┴─────────┐
        │                   │
   ┌────▼────┐       ┌─────▼─────┐
   │ 2-Terminal│      │3-Terminal │
   └─────────┘       └───────────┘
        │                   │
   ┌────▼────┐       ┌─────▼─────┐
   │ Diodes  │       │Transistors│
   └─────────┘       └───────────┘
```

#### 🔺 1. Diodes | डायोड

**Definition | परिभाषा:**
A diode is a two-terminal semiconductor device that essentially acts as a one-way valve for current. It allows current to flow easily in one direction (forward bias) and blocks current flow in the opposite direction (reverse bias).

**Diode एक ऐसा component है जो:**
- एक तरफ से current flow करने देता है
- दूसरी तरफ से current को block करता है
- एक check valve की तरह काम करता है
- P-N junction से बना होता है

**Symbol | चिह्न:** 
```
    Anode    Cathode
      +        -
   ---|>|---   (Arrow pointing towards bar)
```

**🔬 Working Principle | कार्य सिद्धांत:**

Diodes are made from p-n junctions (P-type और N-type semiconductor materials के junction)

**Forward Bias (आगे की दिशा):**
- Anode (+) positive, Cathode (-) negative
- Depletion region shrinks
- Current flows easily
- Voltage drop: ~0.7V (Silicon), ~0.3V (Germanium)

**Reverse Bias (पीछे की दिशा):**
- Anode (-) negative, Cathode (+) positive  
- Depletion region widens
- Very little current flows (leakage current)
- Acts like open circuit

```
📊 Diode I-V Characteristic:
         │ Current (I)
         │     ╱
         │    ╱
         │   ╱ Forward Bias
    ─────┼──╱─────────── Voltage (V)
         │ ╱ 0.7V
         │╱
    Reverse│ Bias
         │
```

**🎯 Types of Diodes | डायोड के प्रकार:**

1. **Silicon Diode:**
   - Forward voltage drop: 0.7V
   - सबसे common type
   - General purpose applications

2. **Germanium Diode:**
   - Forward voltage drop: 0.3V
   - Low voltage applications

3. **Zener Diode:**
   - Reverse breakdown voltage पर constant voltage
   - Voltage regulation के लिए

4. **LED (Light Emitting Diode):**
   - Forward bias में light emit करता है
   - Different colors available

5. **Schottky Diode:**
   - Very low forward voltage drop (0.2-0.3V)
   - High frequency applications

**📐 Mathematical Models:**

**Ideal Diode Model:**
- Forward Bias: Short circuit (0V drop)
- Reverse Bias: Open circuit (∞ resistance)

**Practical Diode Model:**
- Forward Bias: Constant voltage drop (0.7V for Si)
- Reverse Bias: Open circuit

**Shockley Diode Equation:**
```
I = Is(e^(V/ηVt) - 1)
```
Where:
- Is = Reverse saturation current
- V = Diode voltage
- η = Ideality factor (1-2)
- Vt = Thermal voltage (≈26mV at room temperature)

**📊 Practical Examples | व्यावहारिक उदाहरण:**

1. **Rectifier Circuit:**
   - AC को DC में convert करना
   - Half-wave और Full-wave rectifiers

2. **Protection Circuit:**
   - Reverse polarity protection
   - Overvoltage protection

3. **Clipping/Limiting:**
   - Signal को limit करना
   - Unwanted peaks को remove करना

**🎯 Applications | अनुप्रयोग:**
- Rectification (AC to DC conversion)
- Voltage regulation (Zener diodes)
- Signal limiting/clipping
- Switching applications
- Light emission (LEDs)
- Solar cells (photovoltaic diodes)
- Radio frequency mixing

**💡 Exam Important Points:**
- Forward bias में 0.7V drop (Silicon)
- Reverse bias में open circuit
- I-V characteristic curve जानना important
- Different types और applications
- Rectifier circuits में use
- Symbol correctly draw करना

#### 🔄 2. Transistors | ट्रांजिस्टर

**Definition | परिभाषा:**
Transistors are three-terminal semiconductor devices used for amplification or switching electronic signals and electrical power. They are the fundamental building blocks of modern electronics.

**Transistor एक ऐसा component है जो:**
- तीन terminals होते हैं (Three terminals)
- Signal को amplify कर सकता है
- Switch की तरह भी काम करता है
- Modern electronics का heart है

**🎯 Types | प्रकार:**
1. **BJT (Bipolar Junction Transistor)**
2. **FET (Field Effect Transistor)**

```
📊 Transistor Family Tree:
                    TRANSISTORS
                        │
            ┌───────────┴────────────┐
            │                        │
        ┌───▼───┐                ┌───▼───┐
        │  BJT  │                │  FET  │
        └───┬───┘                └───┬───┘
            │                        │
      ┌─────┴─────┐            ┌─────┴─────┐
      │           │            │           │
   ┌──▼──┐     ┌──▼──┐      ┌──▼──┐     ┌──▼──┐
   │ NPN │     │ PNP │      │JFET │     │MOSFET│
   └─────┘     └─────┘      └─────┘     └─────┘
```

---

##### 🔋 a. Bipolar Junction Transistors (BJTs)

**Definition | परिभाषा:**
A BJT is a current-controlled device. A small current at the base terminal controls a larger current flow between the collector and emitter terminals.

**BJT की विशेषताएं:**
- Current controlled device है
- Base current से collector-emitter current control होता है
- दो P-N junctions होते हैं
- High current gain मिलता है

**Terminals | टर्मिनल्स:**
- **Base (B)** - Control terminal
- **Collector (C)** - Output terminal (positive)
- **Emitter (E)** - Output terminal (negative)

**🔬 Types | प्रकार:**

**1. NPN Transistor:**
```
   Collector (C)
        │
        ▼
   ─────┬─────
        │ \
        │  >  (Arrow pointing OUT)
        │ /
   ─────┬─────
        │
        ▼
   Emitter (E)
        │
   Base (B)
```

**2. PNP Transistor:**
```
   Collector (C)
        │
        ▼
   ─────┬─────
        │ \
        │  <  (Arrow pointing IN)
        │ /
   ─────┬─────
        │
        ▼
   Emitter (E)
        │
   Base (B)
```

**🎯 Operating Regions | संचालन क्षेत्र:**

**1. Cut-off Region:**
- Both junctions reverse biased
- No current flow (IB = IC = IE = 0)
- Transistor acts as open switch

**2. Active Region (Amplification):**
- Base-Emitter: Forward biased
- Collector-Base: Reverse biased
- Used for amplification
- Linear operation

**3. Saturation Region:**
- Both junctions forward biased
- Maximum current flow
- Transistor acts as closed switch

```
📊 Operating Regions:
       IC
        │     Active Region
        │    ╱
        │   ╱ (Amplification)
        │  ╱
        │ ╱
   ─────┼╱─────────────── VCE
  Cut-off│    Saturation
        │   (Switch ON)
   (Switch OFF)
```

**📐 Important Equations | महत्वपूर्ण समीकरण:**

**Current Relationships:**
```
IE = IB + IC        (Kirchhoff's Current Law)
IC = β × IB         (β = Current gain, typically 50-200)
IC = α × IE         (α ≈ 0.95-0.99)
```

**Relationship between α and β:**
```
β = α/(1-α)
α = β/(β+1)
```

**📊 Practical Examples | व्यावहारिक उदाहरण:**

**1. Common Emitter Amplifier:**
- Input: Base-Emitter
- Output: Collector-Emitter
- High voltage gain
- Phase inversion होता है

**2. Switching Circuit:**
- Cut-off: Switch OFF
- Saturation: Switch ON
- Digital logic में use

**3. Current Mirror:**
- Constant current source बनाने के लिए
- IC circuits में widely used

**🎯 Applications | अनुप्रयोग:**
- Amplifiers (audio, RF, video)
- Switches (digital circuits)
- Oscillators (signal generation)
- Voltage regulators
- Current sources
- Logic gates (DTL, RTL circuits)

**💡 Exam Important Points:**
- IE = IB + IC (KCL)
- IC = β × IB (current gain)
- Three operating regions
- NPN vs PNP differences
- Common configurations (CE, CB, CC)
- Switch और amplifier applications

#### ⚡ 3. FET (Field-Effect Transistors) | फील्ड इफेक्ट ट्रांजिस्टर

**Definition | परिभाषा:**
FETs are voltage-controlled devices. A voltage applied to the gate terminal controls the current flow between the source and drain terminals. They have high input impedance.

**FET की विशेषताएं:**
- Voltage controlled device है
- Gate voltage से drain-source current control होता है  
- बहुत high input impedance होता है
- Unipolar device (एक type के charge carriers)

**Terminals | टर्मिनल्स:**
- **Gate (G)** - Control terminal (input)
- **Drain (D)** - Output terminal (positive)
- **Source (S)** - Output terminal (negative)

**🔬 Types | प्रकार:**

**1. JFET (Junction Field-Effect Transistor):**
- P-N junction के साथ gate
- Depletion mode operation
- Gate reverse biased रखते हैं

```
JFET Structure:
   Drain (D)
       │
   ┌───▼───┐
   │   N   │ ← Channel
Gate│←─────→│Gate
   │   │   │
   └───▼───┘
   Source (S)
```

**2. MOSFET (Metal-Oxide-Semiconductor FET):**
- Insulated gate (SiO2 layer)
- Enhancement या Depletion mode
- सबसे widely used

```
MOSFET Structure:
   Gate (G)
       │
   ┌───▼───┐ ← Oxide layer
   │   │   │
Drain│   │   │Source
   │ Channel │
   └───────┘
   Substrate
```

**🎯 MOSFET Types:**

**1. Enhancement Mode:**
- Normally OFF (no channel)
- Positive gate voltage creates channel
- Most common type

**2. Depletion Mode:**
- Normally ON (channel exists)
- Negative gate voltage depletes channel

**N-Channel vs P-Channel:**
- **nMOS:** N-channel, positive gate voltage for ON
- **pMOS:** P-channel, negative gate voltage for ON

**📐 Important Characteristics:**

**1. Transconductance (gm):**
```
gm = ΔID/ΔVGS
```

**2. Drain Current (Active region):**
```
ID = K(VGS - VTH)²
```
Where:
- K = Transconductance parameter
- VGS = Gate-Source voltage
- VTH = Threshold voltage

**3. Input Impedance:**
- JFET: ~10¹² Ω
- MOSFET: ~10¹⁴ Ω (practically infinite)

**📊 Practical Examples | व्यावहारिक उदाहरण:**

**1. Voltage Amplifier:**
- High input impedance
- Good voltage gain
- Low input current

**2. Digital Switch:**
- ON/OFF operation
- Low power consumption
- Fast switching speed

**3. Current Source:**
- Constant current applications
- Active loads में use

**🎯 Applications | अनुप्रयोग:**
- Amplifiers (high input impedance needed)
- Digital switches (CMOS logic)
- Voltage followers/buffers
- Oscillators और timers
- Power switching (MOSFETs)
- RF applications (low noise)

**💡 Advantages over BJTs:**
- Higher input impedance
- Lower power consumption
- Better thermal stability
- Easier to manufacture (ICs में)
- No input current needed

**💡 Exam Important Points:**
- Voltage controlled device
- High input impedance
- gm = ΔID/ΔVGS
- Enhancement vs Depletion mode
- nMOS vs pMOS operation
- JFET vs MOSFET differences

#### 💻 4. MOS and CMOS | एमओएस और सीएमओएस

---

##### 🔧 a. MOS (Metal-Oxide-Semiconductor)

**Definition | परिभाषा:**
MOS refers to the fundamental structure of MOSFETs. It describes the layers: Metal (gate electrode), Oxide (insulator, typically silicon dioxide), and Semiconductor (silicon substrate).

**MOS structure में तीन layers होती हैं:**
- **Metal:** Gate electrode (aluminum या polysilicon)
- **Oxide:** Insulator layer (SiO2 - silicon dioxide)
- **Semiconductor:** Silicon substrate (P-type या N-type)

```
📊 MOS Structure:
   ┌─────────────────┐ ← Metal Gate
   │                 │
   ├─────────────────┤ ← Oxide (SiO2)
   │                 │
   │   Semiconductor │ ← Silicon Substrate
   │    (P or N)     │
   └─────────────────┘
```

**🎯 Types | प्रकार:**

**1. nMOS (N-channel MOSFET):**
- N-type channel for current flow
- P-type substrate
- Positive gate voltage for ON state
- Electrons are majority carriers

**2. pMOS (P-channel MOSFET):**
- P-type channel for current flow
- N-type substrate  
- Negative gate voltage for ON state
- Holes are majority carriers

**📐 Working Principle (nMOS Enhancement Mode):**

**OFF State (VGS = 0):**
- No channel exists
- Very high resistance between drain-source
- Practically no current flow

**ON State (VGS > VTH):**
- Positive gate voltage attracts electrons
- N-channel forms under gate oxide
- Low resistance path between drain-source
- Current flows from drain to source

```
📊 nMOS Operation:
         Gate
           │ +VGS
   ┌───────▼───────┐
Drain│  ─ ─ ─ ─ ─  │Source
   │  Electron    │
   │  Channel     │
   └──────────────┘
     P-Substrate
```

**🎯 Advantages | फायदे:**
- Very high input impedance (10¹⁴ Ω)
- Low power consumption (static)
- Good for scaling down (smaller sizes)
- Fast switching speeds
- Easy integration in ICs

**📊 Applications | अनुप्रयोग:**
- Digital logic circuits
- Analog amplifiers
- Memory devices (RAM, ROM)
- Microprocessors
- Power electronics

---

##### ⚡ b. CMOS (Complementary Metal-Oxide-Semiconductor)

**Definition | परिभाषा:**
CMOS technology uses complementary pairs of nMOS and pMOS transistors to implement logic gates and other digital circuits. यह modern digital electronics का backbone है।

**CMOS की विशेषताएं:**
- nMOS और pMOS दोनों का use करता है
- Complementary operation (एक ON तो दूसरा OFF)
- Static power consumption बहुत कम
- Modern computers का foundation

**🔬 Working Principle | कार्य सिद्धांत:**

CMOS circuit में जब nMOS ON होता है, तो pMOS OFF होता है और vice versa। इससे power supply से ground तक कभी direct path नहीं बनता (static state में)।

```
📊 CMOS Inverter:
    VDD (+5V)
      │
   ┌──▼──┐ pMOS (P-channel)
   │     │
Input──┼─────── Output
   │     │
   └──▼──┘ nMOS (N-channel)
      │
     GND
```

**Truth Table (Inverter):**
| Input | pMOS | nMOS | Output |
|-------|------|------|--------|
|   0   |  ON  | OFF  |   1    |
|   1   | OFF  |  ON  |   0    |

**🎯 CMOS Advantages | फायदे:**

**1. Extremely Low Static Power:**
- Static current ≈ 0 (except leakage)
- Power केवल switching के time consume होती है
- Battery life बढ़ती है

**2. High Noise Immunity:**
- Large noise margins
- Reliable operation in noisy environments

**3. Full Rail-to-Rail Swing:**
- Output 0V (logic 0) से VDD (logic 1) तक swing करता है
- Clean digital signals

**4. Good Scalability:**
- Smaller geometries में easily manufacture होता है
- Moore's law को support करता है

**📊 Power Consumption:**
```
P_total = P_static + P_dynamic
P_static ≈ 0 (leakage current only)
P_dynamic = α × CL × VDD² × f
```
Where:
- α = Activity factor
- CL = Load capacitance
- VDD = Supply voltage
- f = Clock frequency

**🎯 Applications | अनुप्रयोग:**
- **Microprocessors:** Intel, AMD processors
- **Memory:** RAM, ROM, Flash memory
- **Digital Signal Processors (DSPs)**
- **Microcontrollers:** Arduino, ARM processors
- **Application Specific ICs (ASICs)**
- **System-on-Chip (SoC):** Smartphones, tablets

**📊 CMOS Logic Gates:**

**NAND Gate:**
```
    VDD
     │
  ┌──▼──┐ pMOS parallel
A──│     │──┐
  └─────┘  │
  ┌──▼──┐  │ Output
B──│     │──┘
  └─────┘ pMOS
     │
  ┌──▼──┐ nMOS series
A──│     │
  └──▼──┘
  ┌─────┐
B──│     │
  └──▼──┘
    GND
```

**💡 Exam Important Points:**
- CMOS = nMOS + pMOS complementary pairs
- Static power consumption ≈ 0
- High noise immunity
- Full rail-to-rail output swing
- Modern digital electronics का backbone
- Inverter का operation समझना जरूरी
- Power consumption formula
- Advantages over other technologies

---

## 📡 II. Signals | सिग्नल्स

### 📚 Signal Introduction | सिग्नल परिचय

Electrical signals are waveforms that convey information. Understanding their characteristics is crucial for analyzing and designing electronic circuits.

**Signal क्या है?**
- Information carry करने वाला electrical quantity
- Voltage या current के form में हो सकता है
- Time के साथ change होता रहता है
- Communication और control systems का basis है

**🔑 Why Study Signals? | सिग्नल्स क्यों पढ़ें?**
- Circuit analysis के लिए जरूरी
- Communication systems समझने के लिए
- Signal processing में applications
- Real-world systems में signals everywhere हैं

```
📊 Signal Classification Overview:
                    SIGNALS
                       │
           ┌───────────┴────────────┐
           │                        │
       ┌───▼───┐                ┌───▼───┐
       │ By    │                │ By    │
       │Nature │                │Pattern│
       └───┬───┘                └───┬───┘
           │                        │
     ┌─────┴─────┐            ┌─────┴─────┐
     │           │            │           │
  ┌──▼──┐     ┌──▼──┐      ┌──▼──┐     ┌──▼──┐
  │ DC  │     │ AC  │      │Periodic│ │Non-  │
  └─────┘     └─────┘      └─────┘  │periodic│
                                    └────────┘
```

### ⚡ A. DC/AC Signals | डीसी/एसी सिग्नल्स

---

#### 🔋 1. DC (Direct Current) Signals | डीसी सिग्नल्स

**Definition | परिभाषा:**
A signal whose magnitude and direction remain constant over time. DC signals have zero frequency.

**DC signal की विशेषताएं:**
- Magnitude constant रहता है
- Direction change नहीं होती
- Frequency = 0 Hz
- Time के साथ value same रहती है

```
📊 DC Signal Waveform:
    Voltage
       │
    5V ├─────────────────────
       │
    0V ├─────────────────────── Time
       │
   -5V ├─────────────────────
       └─────────────────────
```

**🎯 Characteristics | विशेषताएं:**
- **Constant voltage:** Battery से मिलती है constant voltage
- **Constant current:** Magnitude और direction fixed
- **Zero frequency:** कोई oscillation नहीं होती
- **Time independent:** f(t) = constant

**📊 Examples | उदाहरण:**
- **Battery voltage:** 1.5V, 9V, 12V batteries
- **DC power supply output:** Computer SMPS output
- **Solar panel output:** Direct sunlight में constant DC
- **DC motor supply:** Constant speed के लिए

**🎯 Mathematical Representation:**
```
v(t) = V_DC = constant
i(t) = I_DC = constant
```

**Applications | अनुप्रयोग:**
- Electronic devices (laptops, phones)
- LED lighting systems
- Battery powered devices
- DC motors और fans
- Digital circuits (logic levels)

---

#### 🌊 2. AC (Alternating Current) Signals | एसी सिग्नल्स

**Definition | परिभाषा:**
A signal whose magnitude and direction vary periodically with time. AC signals have non-zero frequency and alternate between positive and negative values.

**AC signal की विशेषताएं:**
- Magnitude time के साथ change होता है
- Direction periodically reverse होती है
- Non-zero frequency होती है
- Sinusoidal या other periodic waveforms

```
📊 AC Signal Waveform (Sine Wave):
    Voltage
       │      ╭─╮
    +VP├─────╱───╲─────╱───╲─── Time
       │    ╱     ╲   ╱     ╲
     0 ├───╱───────╲─╱───────╲─
       │          ╱ ╱         ╲
   -VP ├─────────╱─╱───────────╲─
       └──────────────────────────
             T (Period)
```

**🎯 Characteristics | विशेषताएं:**
- **Periodically varying:** Regular intervals में repeat होता है
- **Bidirectional:** Positive और negative values लेता है
- **Non-zero frequency:** f = 1/T Hz
- **RMS value:** Effective value के लिए important

**📐 Mathematical Representation:**
```
v(t) = VP sin(ωt + φ)
```
Where:
- VP = Peak voltage (amplitude)
- ω = Angular frequency = 2πf
- φ = Phase angle
- t = Time

**🎯 Parameters | पैरामीटर:**

**1. Peak Value (VP):**
- Maximum value from zero level
- Amplitude of the waveform

**2. Peak-to-Peak Value (VPP):**
- Difference between +VP and -VP
- VPP = 2VP (for symmetrical waveforms)

**3. Period (T):**
- Time for one complete cycle
- Measured in seconds

**4. Frequency (f):**
- Number of cycles per second
- f = 1/T Hz

**5. Angular Frequency (ω):**
- ω = 2πf rad/second

**📊 Types of AC Waveforms:**

**1. Sinusoidal (सबसे common):**
- Smooth oscillation
- Pure tone in audio
- Power distribution में use

**2. Square Wave:**
- Digital signals में common
- Rapid switching between two levels

**3. Triangular Wave:**
- Linear rise और fall
- Function generators में

**4. Sawtooth Wave:**
- Ramp-like waveform
- Oscilloscope sweep signals

**📊 Examples | उदाहरण:**
- **Household AC supply:** 230V, 50Hz (India)
- **Audio signals:** Music, speech
- **Radio waves:** AM/FM broadcasting
- **Power transmission:** High voltage AC

**🎯 Applications | अनुप्रयोग:**
- Power transmission और distribution
- Audio systems (music, speech)
- Radio frequency communication
- Motor drives (AC motors)
- Transformers (voltage conversion)

**💡 DC vs AC Comparison:**

| Parameter | DC | AC |
|-----------|----|----|
| **Frequency** | 0 Hz | Non-zero |
| **Direction** | Constant | Alternating |
| **Transmission** | High losses | Low losses |
| **Transformation** | Difficult | Easy (transformers) |
| **Storage** | Easy (batteries) | Difficult |
| **Examples** | Batteries, Solar | Mains supply, Audio |

**💡 Exam Important Points:**
- DC frequency = 0 Hz
- AC frequency ≠ 0 Hz
- Sine wave mathematical representation
- Peak, Peak-to-Peak values
- Period और frequency relationship
- Different AC waveform types
- Real-world applications

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
