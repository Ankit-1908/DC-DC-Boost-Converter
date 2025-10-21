
# ⚡ DC–DC Boost Converter  


Design and implement a **DC–DC Boost Converter** with the following specifications:  

| Parameter | Specification |
|------------|----------------|
| Input Voltage | 15 V |
| Output Voltage | 25 V |
| Switching Frequency | 7.5 kHz |
| Output Current | 1 A |

### Tasks
1. Simulate and observe the **Diode Current** and **Inductor Voltage** in **Continuous Conduction Mode (CCM)**.  
2. Increase load resistance to demonstrate **Discontinuous Conduction Mode (DCM)** operation.  

---

## ⚙️ Methodology  

1. **PWM Generation:**  
   - A Pulse Width Modulator (PWM) circuit was designed to operate at 7.5 kHz.  
   - The duty cycle was adjusted (around 40%) to achieve the required voltage boost.  

2. **Driver Circuit:**  
   - The driver circuit interfaces the PWM signal with the power MOSFET.  
   - Ensures proper switching and isolation.  

3. **Boost Converter Simulation:**  
   - The converter was simulated using standard power electronics tools (MATLAB/PSIM/Multisim).  
   - Observed inductor current, diode current, and output voltage waveforms in both CCM and DCM.  

---

## 🧩 Theoretical Overview  

The **Boost Converter** is a type of DC–DC converter that steps up the input voltage to a higher level at the output.  

### Operating Modes
- **Continuous Conduction Mode (CCM):**  
  The inductor current never falls to zero during the switching cycle.  
- **Discontinuous Conduction Mode (DCM):**  
  The inductor current falls to zero before the next switching cycle begins, typically under light-load conditions.

---

## 📊 Simulation Results  

### 1. PWM and Driver Integration  
- PWM signal generated at **7.5 kHz**.  
- Driver output verified with **40% duty cycle**.  

### 2. Continuous Conduction Mode (CCM)  
- **Diode Current** and **Inductor Voltage** waveforms observed.  
- **Input Pulse** and **Output Voltage** confirmed proper voltage boosting.  

### 3. Discontinuous Conduction Mode (DCM)  
- Achieved by increasing load resistance.  
- **Inductor Current** and **Voltage** demonstrated zero-current intervals.  

---

## 🧠 Observations  

| Mode | Behavior | Key Observation |
|------|-----------|----------------|
| CCM | Continuous inductor current | Stable output voltage with low ripple |
| DCM | Inductor current drops to zero | Reduced efficiency, higher voltage ripple |

---

## 📈 Conclusions  

- The designed boost converter successfully stepped up **15V to 25V**.  
- The converter operated efficiently at **7.5 kHz switching frequency**.  
- The transition between **CCM and DCM** was clearly observed by varying load resistance.  
- Simulation verified expected waveforms of **diode current**, **inductor voltage**, and **output voltage**.  

---

## 🧰 Tools & Components  

- **Software:** MATLAB (for simulation)  
- **Components:**  
  - MOSFET (Switching device)  
  - Diode (Freewheeling path)  
  - Inductor and Capacitor (Energy storage elements)  
  - PWM Generator and Driver Circuit  
