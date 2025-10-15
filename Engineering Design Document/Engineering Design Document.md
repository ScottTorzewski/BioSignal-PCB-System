# Engineering Design Document
## Fluorescence-Based Spectrometer for Biophotonic Signal Acquisition
Author: Scott Torzewski

## Rationale
Studying analog/mixed-signal (AMS) design is crucial for biotechnology applications because it enbales the precise and efficient processing of delicate biological signals. These signals are often extremely weak and operate within noisy physiological environments, which presents a challenge for detection and analysis. Optical analog front-end circuits are the first point of contact for the raw, continous data from our physical world and play a critical role in determining the system sensitivity and accuracy before the signal is converted to the digital domain. 

At a higher-level, exploring AMS design is essential for bioprocessing systems because it enables the development of high-performance sensors needed for real-time monitoring and control. As an engineer in the biopharmaceuitcal manufacturing industry, I am constanty exposed to Process Analytical Technology (PAT) such as the RamanRxN4, a high-performance Raman spectroscopy system that includes a specialized bIO-PRO probe for sterile integration with bioreactors.  As biprocessing shifts towards this data-driven paradigm, AMS technology provides the electronics that can accurately acquire sensor signals within challenging bioreactor enviornments. 

## Background

what is fluorescence sensing, how does it work, why is it important ex. certain biomarkers

Aside from the fluorochrome itself, there are five main components required for a fluorescence spectrometer. 

  1) Light excitation source: This is the light source that emits light at a specific wavelength to excite the fluorochrome.
  2) Optical filters: Spectrometers require two filters. An excitation filter selects the specific wavelength from               the light source that will excite the sample, while an emission filter blocks the excitation light while allowing the       longer-wavelength fluorescence to pass through the detector.
  3) Photodetector: This component measures the lighted emitted by the fluorescent sample and converts the photons into an       electrical signal, generating a "photocurrent."
  4) Analog front-end (AFE): The AFE processes the raw electrical signal from the photodetector for digitization. The goal       is to convert the current to a stable voltage signal that an analog-to-digital converter (ADC) can read for                 quantization.
  5) Microcontroller Unit (MCU): The MCU is the digital brain of the system. It is responsible for processing the digitzied      signal and outputting the final result as data that we can interpret.

## Terminology

## Proposed Design

## System Architecture

## Detailed Design

## Test Plan

## BOM

## Business Logic

## Impact

## Risks

## Alternatives 


