# 📡 X-Band Microwave Engineering Laboratory Kit

This repository serves as a comprehensive visual and technical guide to the **U-Series Microwave Training System**. This kit is a modular waveguide-based laboratory setup used to study electromagnetic wave propagation, antenna theory, and microwave measurements in the **X-Band frequency range (8.2 GHz to 124 GHz)**.

<img width="391" height="435" alt="image" src="https://github.com/user-attachments/assets/27a04d68-c891-4501-8c1d-62912f302023" />

<img width="375" height="482" alt="image" src="https://github.com/user-attachments/assets/7af6d466-77f1-4048-b264-0aa88e02ce4c" />

<img width="242" height="357" alt="image" src="https://github.com/user-attachments/assets/ebb927c9-e393-45fd-9958-71b85fe86fc5" />


---

## 📸 Equipment Overview

The system is divided into three primary categories: Signal Generation, Waveguide Passive Components, and Measurement/Antenna Hardware.

### 1. Power Supply & Signal Control
The foundational electronics required to drive the microwave source and modulate signals.

* **Gunn Power Supply:** Provides stable DC bias for the Gunn Oscillator.
* **1kHz Square Wave Generator:** Used for modulating the microwave signal, allowing for easier detection via a VSWR meter.
* **PIN Diode Modulator:** An electronic switch used for pulse modulation of the microwave carrier.

### 2. Waveguide Components (The "Plumbing")
Precision-machined brass and aluminum components designed to guide electromagnetic waves.

| Component | Description |
| :--- | :--- |
| **Slotted Line** | A section of waveguide with a longitudinal slot for a probe to measure standing wave patterns. |
| **Frequency Meter** | A cylindrical cavity resonator used to identify the precise operating frequency. |
| **Directional Coupler** | A 4-port device that samples power flowing in one direction. |
| **E/H-Plane Tees** | Junctions used for splitting or combining power in the E or H plane. |
| **Isolator** | Ensures one-way signal flow to protect the source from reflected power. |



### 3. Termination & Radiation
Components used to either absorb energy or radiate it into free space.

* **Horn Antennas:** Standard gain antennas used for transmitting and receiving signals.
* **Matched Load:** A termination that absorbs all incident power (Zero reflection).
* **Movable Short:** A sliding plunger that reflects 100% of the signal, used to shift the phase of standing waves.

---

## 🧪 Core Laboratory Experiments

This kit is designed to facilitate the following technical procedures:

### A. VSWR & Reflection Coefficient
By using the **Slotted Line**, one can measure the Voltage Standing Wave Ratio ($VSWR$) to determine how well a load is matched to the system.
$$VSWR = \frac{V_{max}}{V_{min}}$$

### B. Guide Wavelength Measurement
Measuring the distance between two successive minima ($d$) on the slotted line allows for the calculation of the Guide Wavelength ($\lambda_g$):
$$\lambda_g = 2 \times d$$



### C. Antenna Radiation Patterns
By mounting the **Horn Antennas** on a rotating stand, students can plot the signal strength vs. angle to determine:
* **Half-Power Beamwidth (HPBW)**
* **Side-Lobe Levels**
* **Front-to-Back Ratio**

---

## ⚠️ Safety Protocols

> [!WARNING]
> **Microwave Radiation Safety:**
> * **Never** look directly into an open waveguide or horn antenna while the source is active.
> * Microwaves at these frequencies can cause internal heating of the eyes (cataracts) without immediate pain.
> * Ensure all flanges are securely bolted to prevent RF leakage.

---

## 🛠 Usage Instructions
1.  **Assembly:** Connect the Gunn Oscillator to the Isolator followed by the Frequency Meter.
2.  **Power Up:** Set the Gunn Power Supply to the threshold voltage (usually ~7V to 10V).
3.  **Tuning:** Use the Frequency Meter to find the "dip" in the SWR meter to identify the resonant frequency.
4.  **Measurement:** Slide the probe along the Slotted Line to record $V_{max}$ and $V_{min}$.

---
