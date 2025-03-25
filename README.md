# Audio Amplifier Design

## Project Overview
This project involves the design, analysis, and implementation of an **audio amplifier** with the following specifications:

- **Gain**: 500 (Pre-amp and Gain stage)
- **Input Signal**: 10–20 mV peak-to-peak
- **Output Power**: 1.5 W
- **Frequency Range**: Audible range (20 Hz–20 kHz)
- **Filter**: Should not attenuate the input signal
- **Power Amplifier**: Should not provide voltage gain
- **Load Resistance**: 10 Ω

The system consists of multiple stages, including a **pre-amplifier, gain stage, filter stage, and a class AB power amplifier**, optimized to minimize distortion and maximize efficiency.
View the report for detailed analysis of the project.
---

## System Design

### 1️. **Pre-Amplifier Stage**
- A **common-emitter differential amplifier** is used for initial signal amplification.
- Ensures **high input impedance and low noise**.
- Uses a **capacitor for AC coupling** to remove DC components.
- Designed to **match impedance** between the microphone and the next stage.

### 2️. **Gain Stage**
- A **common-emitter amplifier** is used for voltage amplification.
- Provides the **majority of the gain** required for the amplifier.
- Biasing resistors **stabilize gain** and improve performance.

### 3️. **Filter Stage**
- A **band-pass filter** limits the signal to the **audible frequency range (20 Hz – 20 kHz)**.
- An **active filter with an OpAmp** is used to ensure impedance matching.
- Reduces unwanted noise while **maintaining signal integrity**.

### 4️. **Power Amplifier Stage**
- A **Class AB amplifier** is used for power amplification.
- Provides **current gain** while maintaining efficiency.
- Reduces **crossover distortion** found in Class B amplifiers.

---

## Key Performance Metrics
- **Total Harmonic Distortion (THD)**: Measured using Fast Fourier Transform (FFT).
- **Slew Rate**: Ensures high-frequency signals are not distorted.
- **Phase Shift Analysis**: Verified at each stage.

---

## Tools & Technologies
- **LTSpice**: Circuit simulation
- **Hardware Components**: BJTs, Resistors, Capacitors, OpAmps, MOSFETs, Mic circuit, speaker, UA741 IC, TIP 31, TIP 32

---

## How to Run Simulations
1. Open **LTSpice**.
2. Load the provided **.asc** simulation files.
3. Run the simulations to observe gain, frequency response, and THD.

---
