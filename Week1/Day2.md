## 📈 Progress
Today, I developed the requirements list, a test plan, and researched fluorescence excitation and emission fundamentals for selecting a light excitation source and optical filter. 

---
Requirements - 

Hardware Requirements: 
Excitation Source – LED matched to fluorescein excitation (~490 nm).
Detector – Photodiode sensitive to fluorescein emission (~520 nm) with appropriate bandpass filter.
PCB – Custom layout integrating LED driver, detector circuitry, amplification, and microcontroller interface.
Power – Stable, low-noise supply (battery or USB-powered).
Microcontroller – ADC capability for photodiode readout, capable of logging data via USB/serial.
Optional Optics – Lenses or diffusers for uniform illumination and signal optimization.

Software Requirements: 
Embedded code for LED control, signal acquisition, and basic filtering.
Data logging and visualization (Python, MATLAB, or microcontroller serial output).
Calibration routines to convert raw voltage to fluorescence intensity.

Functional Requirements: 
Detect fluorescein in solution over a range of concentrations (e.g., 1–100 µM).
Generate reproducible and concentration-dependent signals.
Display or log signal in a human-readable format.
Operate safely without hazardous chemicals or human tissue.

---
Test Plan - 

Step 1: Component Validation
Verify LED emits at correct wavelength.
Confirm photodiode responds to emission spectrum.
Test microcontroller ADC and amplification circuit separately.

Step 2: System Integration
Assemble PCB with LED, detector, amplifier, and microcontroller.
Confirm LED control and photodiode readout function together.

Step 3: Functional Testing with Fluorescein
Prepare standard fluorescein solutions at multiple concentrations.
Measure sensor output for each concentration; repeat 3–5 times for reproducibility.
Plot fluorescence intensity vs. concentration to verify linearity and sensitivity.

Step 4: Calibration and Validation
Compare measurements to reference values (literature or spectrometer).
Adjust amplification/filtering to optimize signal-to-noise ratio.

Step 5: Documentation
Log all raw and processed data in weekly PCG folders.
Include notes on challenges, parameter adjustments, and next steps.
Include photos, schematics, and code snippets for reproducibility.

---
FLuorochromes are photoreactive chemical compounds that absorb light energy of a certain wavelength and emit that light at a longer wavelength. This occurs due to the movements of electrons from a ground state to an excited state, and back to a ground state. The action of falling back to a ground state emits photons that can be measured. It is important to note that the emission light spectrum has a slightly longer wavelength than the absorption specturm due to Stoke's Law. 

In determining a fluorochrome to use, we need to consider a readily available solvent, the molecular extinction coefficient (efficiency with which fluorochrome absorbs excitation light), and the quantum yield (ratio of emission wavelength to absorption wavelength). Fluoroscein is a readily available, cheap fluorochrome that is solvent in water. Its excitation wavelength is 437 nm, while its emission wavelength is 515 nm (quantity yield is 0.92). This information has allowed me to make a selection for a light excitation source. The SMD3030 1W Royal Blue 450 nm LED was chosen because its peak emission (450 nm) closely matches fluorescein’s excitation range (around 437 nm), ensuring efficient absorption and strong fluorescence output. Its compact SMD form factor makes it easy to integrate onto a PCB for a portable biosensor platform.

Link: https://www.lumixtar.com/smd3030-1w-royal-blue-450nm-led.html

## 🧩 Challenges
No real challenges were presented today. 

## 🥅 Goals
The goals for tomorrow include continuing the process of selecting components for the PCB. Next up is the photodetector device, analog-front end for signal conversion, and microcontroller for signal processing. 
