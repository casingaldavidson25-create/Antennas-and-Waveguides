# 📡 X-Band Microwave Engineering & Antenna Laboratory

Welcome to the documentation repository for the **Microwave Training System**. This repository contains technical specifications, component identification, and experimental procedures for the waveguide-based training kits shown in the reference images.

---

## 🛠️ System Architecture

This kit is designed for the study of **X-Band** frequencies ($8.2 \text{ GHz}$ to $12.4 \text{ GHz}$). It uses standard **WR-90** waveguide dimensions to demonstrate electromagnetic theory in a physical, measurable environment.

### 📦 Component Catalog

#### 1. Signal Sources & Control (The Power Tray)
Located in the main control unit, these provide the "heartbeat" of the experiments:
* **Gunn Power Supply (U-3000P):** Provides the specific DC bias required to operate the Gunn Diode oscillator.
* **1kHz Modulator/Generator (U-3000M):** Essential for VSWR measurements; it pulses the microwave signal so it can be detected by narrowband SWR meters.
* **PIN Diode Modulator:** An electronic switch used for high-speed pulse modulation of the carrier wave.

#### 2. Waveguide Passive Components
These are the "pipes" that shape and direct the microwave energy:
* **Slotted Line:** A precision-machined waveguide with a longitudinal slot for a probe. Used to measure the standing wave pattern ($V_{max}$ and $V_{min}$).
* **Frequency Meter:** A cavity resonator used to identify the precise frequency by observing a power dip.
* **Variable Attenuator:** A rotatable vane used to reduce signal power without changing the source frequency.
* **E/H Plane Tees:** Used for power splitting and impedance matching.



#### 3. Antennas & Terminations
* **Horn Antennas (Standard Gain):** Used to transition waves from the waveguide into free space for radiation pattern testing.
* **Matched Termination:** A load that absorbs 100% of the energy, simulating an infinite transmission line.
* **Movable Short:** A sliding metal plunger used to create 100% reflection at a specific phase.

---

## 🧪 Core Laboratory Experiments

This hardware supports several fundamental electromagnetic experiments:

### A. VSWR & Reflection Coefficient
Calculate the **Voltage Standing Wave Ratio (SWR)** to determine the impedance mismatch between the source and the load.
$$SWR = \frac{V_{max}}{V_{min}}$$
$$\Gamma = \frac{SWR - 1}{SWR + 1}$$

### B. Guide Wavelength ($\lambda_g$)
Determine the difference between the wavelength in free space ($\lambda_0$) and the wavelength inside the waveguide ($\lambda_g$).
$$\frac{1}{\lambda_g^2} = \frac{1}{\lambda_0^2} - \frac{1}{\lambda_c^2}$$
*(Where $\lambda_c$ is the cutoff wavelength of the WR-90 waveguide).*

### C. Antenna Radiation Patterns
By rotating the **Horn Antenna** and measuring received power at 5° intervals, we can plot the E-plane and H-plane radiation characteristics.



---

## ⚠️ Safety & Maintenance

> [!CAUTION]
> **RF EXPOSURE:** Never look directly into an open waveguide or horn antenna while the Gunn source is active. Microwave radiation at these frequencies can cause permanent damage to the retina.

1.  **Gunn Diode Care:** Never exceed the maximum voltage specified on the Gunn power supply (usually ~10V).
2.  **Flange Protection:** Ensure the mating surfaces of the flanges are clean. Scratches or dirt can cause significant RF leakage and measurement errors.
3.  **Probe Handling:** The Slotted Line probe is extremely fragile. Do not over-tighten the probe depth.

---

## 📂 Repository Content
* `/Manuals`: PDF scans of the U-3000 series operation manuals.
* `/Calculations`: Python/MATLAB scripts for Smith Chart plotting.
* `/Photos`: High-resolution images of the lab bench setup.
* `/Data`: CSV files from VSWR and Antenna experiments.

---

**Next Step:** Would you like me to generate a **Python script** that takes your lab measurements ($V_{max}$, $V_{min}$, and probe position) and automatically generates a **Smith Chart**?
