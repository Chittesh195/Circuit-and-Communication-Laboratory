# 📐 Triangular Wave Generator Using Op-Amp (LM741)

### 🔧 23ECE286 – Circuits and Communication Lab Term Project  

---

## 📘 Project Overview

This project focuses on the **design, simulation, and hardware implementation** of a **triangular wave generator** using **operational amplifiers (LM741)**. The waveform's frequency is **adjustable between 250 Hz and 2.5 kHz**, making it suitable for various signal processing and waveform synthesis applications.

---

## 🎯 Objectives

- Design a **Schmitt Trigger** using LM741 to generate a square wave.
- Build an **Integrator** circuit to convert the square wave into a triangular waveform.
- Achieve a **variable frequency range of 250 Hz to 2.5 kHz**.
- Simulate the circuit using **LTSpice**.
- Implement and test the circuit using **hardware and oscilloscope measurements**.
- Analyze waveform quality and component impact.

---

## 🛠️ Circuit Description

The circuit consists of two main stages:

1. **Schmitt Trigger (Comparator)**
   - Uses LM741 with positive feedback to generate a square wave.
   - Switching thresholds set via voltage divider network.

2. **Integrator**
   - Converts the square wave into a triangular wave.
   - Built with LM741, resistors, and capacitors.

---

## ⚙️ Key Components

| Component           | Specification             |
|---------------------|---------------------------|
| Op-Amp              | LM741 × 2                 |
| Potentiometer       | 4.7 kΩ to 470 kΩ (variable resistor) |
| Resistors           | 1 kΩ, 4.7 kΩ, 12 kΩ        |
| Capacitor           | 0.1 µF                    |
| Power Supply        | ±12 V                     |
| Oscilloscope        | For waveform observation  |
| Breadboard & Wires  | For hardware setup        |

---

## 🔢 Frequency Calculations

Formula used:
```
f = R1 / (4 × R × C × R2)
```

- For **250 Hz**: R = 47 kΩ  
- For **2.5 kHz**: R = 4.7 kΩ  

---

## 🧪 Simulation & Implementation

- **LTSpice** used for waveform validation.
- Hardware circuit implemented on **breadboard**.
- **Oscilloscope** verified clean triangular wave output.
- Adjusting the potentiometer varied the frequency across the desired range.

---

## 📈 Results

- **Waveform Quality**: Stable triangular waveform across entire frequency range.
- **Frequency Range Achieved**: 250 Hz to 2.5 kHz.
- **Simulation and experimental results** closely matched.

| Potentiometer (R) | Frequency (Approx.) |
|-------------------|----------------------|
| 47 kΩ             | 250 Hz               |
| 4.7 kΩ            | 2.5 kHz              |

---

## ⚠️ Challenges & Solutions

| Challenge                    | Solution                                |
|-----------------------------|-----------------------------------------|
| Resistor value mismatches   | Used nearest standard values and recalculated |
| Frequency drift             | Used precision 1% tolerance components  |
| Op-amp limitations          | Optimized for LM741’s bandwidth         |

---

## 📌 Applications

- Signal and function generators  
- Audio waveform synthesis  
- Communication systems (modulation/wave shaping)  

---


## 📚 References

1. Sedra A., Smith K. C., *Microelectronic Circuits*, 6th ed., Oxford University Press, 2010.  
2. Texas Instruments, *Designing With Operational Amplifiers*, [TI Report](https://www.ti.com/lit/pdf/tidu020)
