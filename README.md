Here’s the same write-up rewritten in a **standard, professional format** for a **Buck-Boost Converter** project:

---

## **Design and Implementation of a Buck-Boost Converter**

### **Abstract**

This project focuses on the **design, simulation, and hardware implementation** of a DC–DC Buck-Boost Converter to analyze its performance under different operating conditions. The primary objectives were to examine the behavior of circuit waveforms, evaluate the **efficiency**, and determine the **Total Harmonic Distortion (THD)** of the converter in both buck and boost modes.

### **Simulation Phase**

The design process began with **simulation in MATLAB/Simulink and PLECS** to study the converter’s dynamic response and validate theoretical calculations. An **open-loop model** was first developed to observe the switching characteristics, inductor current, and output voltage variations in both step-up and step-down operations. Simulation results aided in optimizing the component values and validating the control parameters before hardware development.

### **Hardware Implementation**

Following the simulation stage, a **hardware prototype** of the buck-boost converter was constructed. The **MOSFET gate pulses** were generated using a **Wavect controller**, interfaced with a **custom-designed gate driver board**. The driver circuit was designed using **Altium Designer** and fabricated through a **PCB printing process**.

The prototype was initially tested in **open-loop configuration**, powered by a **Chroma programmable DC power supply** with an adjustable input voltage range of **0–48 V**. An **electronic load** was employed to simulate various load conditions. Input and output voltage and current waveforms were measured using a **power analyzer**, while the **switching pulses and gate signals** were monitored on an **oscilloscope** for validation.

During initial testing, one of the gate pulse patterns was found to be irregular. The issue was identified and resolved by modifying the pulse timing parameters in the Wavect controller configuration. After successful debugging, the system was operated in **closed-loop mode** to achieve stable voltage regulation and improved transient response.

### **Analysis and Results**

Comprehensive analysis of the hardware prototype was carried out to evaluate:

* Input and output voltage and current waveforms
* MOSFET switching behavior
* Converter efficiency under different load and input conditions
* THD of the output voltage

The experimental results were compared with the simulation outcomes, showing close correlation and confirming the validity of the design. The buck-boost converter demonstrated reliable performance in both buck and boost modes, meeting the intended design objectives.

