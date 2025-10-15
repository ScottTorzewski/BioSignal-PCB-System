# Engineering Design Document
## Fluorescence-Based Spectrometer for Biophotonic Signal Acquisition
Author: Scott Torzewski

## Rationale
Studying analog/mixed-signal (AMS) design is crucial for biotechnology applications because it enbales the precise and efficient processing of delicate biological signals. These signals are often extremely weak and operate within noisy physiological environments, which presents a challenge for detection and analysis. Optical analog front-end circuits are the first point of contact for the raw, continous data from our physical world and play a critical role in determining the system sensitivity and accuracy before the signal is converted to the digital domain. 

At a higher-level, exploring AMS design is essential for bioprocessing systems because it enables the development of high-performance sensors needed for real-time monitoring and control. As an engineer in the biopharmaceuitcal manufacturing industry, I am constanty exposed to Process Analytical Technology (PAT) such as the RamanRxN4, a high-performance Raman spectroscopy system that includes a specialized bIO-PRO probe for sterile integration with bioreactors.  As biprocessing shifts towards this data-driven paradigm, AMS technology provides the electronics that can accurately acquire sensor signals within challenging bioreactor enviornments. 

## Background

Fluorophores are photoreactive chemical compounds that absorb light energy of a certain wavelength and emit that light at a longer wavelength. This occurs due to the movements of electrons from a ground state to an excited state, and back to a ground state. The action of falling back to a ground state emits photons that can be measured. The emission light spectrum has a slightly longer wavelength than the absorption specturm due to the phenomenon of Stokes shift. In sensing applications the fluorophore's emission changes in a predictable way when it interacts with a target substance.

The funamental process of fluorescence sensing involves three steps.

  1) Excitation: A light source shines on a sample, which excites the electrons in the fluorophore to a higher energy state.
  2) Interaction: When a speciic target analyte is present, it binds to or otherwise interacts with the fluorophore, which       alters the fluorophore's emission properties.
  3) Emission and detection: The excited electrons return to their ground state and emitt photons that are detected and          measured by a sensor.

Fluorescence sensing is a useful tool for biomarker detection due to its high sensitivity and selectivty, which enables the measurement of very low analyte concentrations. For example, in the context of Alzheimer's detection, enhanced fluorescence platforms are used to detect trace levels of biomarkers like amyloid-β and tau proteins in blood samples. 

There are several reasons for why it is important to explore fluorescence sensing technologies.

  1) Early disease diagnosis: Fluorescence sensing can detect minute changes in biomarker levels longer before symptoms          appear. For Alzheimer's disease, detecting alterations in amyloid-β and tau years in advance allows for earlier             intervention.
  2) Less invasive testing: For diseases like Alzheimer's spinal fluid analysis is often used despite its highly-invasive        nature. Fluorescence-based assays allow for the sensitive detection of biomarkers using more accessible blood samples.
  3) Real-time monitoring and imaging: Fluorescen probes can be used for real-time, high-resolution imaging in living cells      and tissues. This is crucial for exploring disease progression in cellular processes and the efficacy of drug               therapies.

Aside from the fluorophore itself, there are five main components required for a spectrometer. 

  1) Light excitation source: This is the light source that emits light at a specific wavelength to excite the fluorochrome.
  2) Optical filters: Spectrometers require two filters. An excitation filter selects the specific wavelength from               the light source that will excite the sample, while an emission filter blocks the excitation light while allowing the       longer-wavelength fluorescence to pass through the detector.
  3) Photodetector: This component measures the lighted emitted by the fluorescent sample and converts the photons into an       electrical signal, generating a "photocurrent."
  4) Analog front-end (AFE): The AFE processes the raw electrical signal from the photodetector for digitization. The goal       is to convert the current to a stable voltage signal that an analog-to-digital converter (ADC) can read for                 quantization.
  5) Microcontroller Unit (MCU): The MCU is the digital brain of the system. It is responsible for processing the digitzied      signal and outputting the final result as data that we can interpret.

## Terminology
Spectrometer
Stokes shift
Analyte

## Proposed Design

## System Architecture

## Detailed Design

## Test Plan

## BOM

## Business Logic

## Impact

## Risks

## Alternatives 


