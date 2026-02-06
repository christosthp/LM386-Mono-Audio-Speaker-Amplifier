# LM386-Mono-Audio-Speaker-Amplifier
A professional-grade hardware project focusing on signal clarity, power stability, and end-to-end hardware development. This project demonstrates a complete engineering workflow from Altium Designer schematics to a handcrafted wooden enclosure.

## 🚀 Technical Deep-Dive

### 1. Schematic Design & Stability
The core of the amplifier is based on the **LM386-N1** IC. To ensure professional-grade performance, the design incorporates:
* **Zobel Network:** A series R-C network at the output stage to compensate for speaker inductance, ensuring amplifier stability and preventing high-frequency oscillations.
* **DC Blocking:** High-quality coupling capacitors are utilized in the signal path to block DC offset while maintaining a linear frequency response.

### 2. Power Conditioning & Noise Mitigation
To tackle EMI and power-rail ripple, a multi-stage decoupling strategy was implemented:
* **Bulk Decoupling:** 470µF Electrolytic capacitor for low-frequency ripple filtering.
* **High-Frequency Bypass:** 100nF Ceramic capacitor to suppress high-frequency noise and EMI.

### 3. Smart Discharge Circuit
Integrated a safety and feedback sub-circuit consisting of a **1kΩ current-limiting resistor** and a status LED. 
* **Visual Feedback:** Real-time operation status.
* **Bleeder Path:** Safely discharges filter capacitors upon power-off, preventing pops or potential damage during maintenance.

### 4. Acoustic Engineering
The output features a unique **dual 4Ω speaker configuration in series**. 
* **Pseudo-Two-Way System:** A parallel capacitor acts as a low-pass filter for one of the drivers, allowing it to focus on low-end punch while the other handles the full range.

---

## 🛠 Prototyping & Assembly
1.  **Verification:** Initial design verified via breadboarding and **Oscilloscope testing**.
2.  **Noise Optimization:** Iterative testing with different capacitor values to achieve the lowest noise floor.
3.  **Physical Layout:** Migrated to a manual perfboard layout with a focus on:
    * Clean solder joints.
    * Optimal component placement to minimize parasitic capacitance.

---
