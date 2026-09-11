# microstrip-patch-antenna-with-dgs
Design and CST simulation of a 2.4 GHz microstrip patch antenna with a Defected Ground Structure (DGS)
# 2.4 GHz Microstrip Patch Antenna with Defected Ground Structure

## Overview

This project presents the design and simulation of a rectangular Microstrip Patch Antenna (MPA) operating around the 2.4 GHz ISM band.

Two antenna configurations were investigated:

1. Conventional Microstrip Patch Antenna
2. Microstrip Patch Antenna with a Defected Ground Structure (DGS)

The effect of introducing the DGS on impedance matching, resonant frequency, VSWR, surface fields, and radiation characteristics was studied using CST Studio Suite.

---

## Objectives

- Design a microstrip patch antenna for operation around 2.4 GHz.
- Simulate the antenna using CST Studio Suite.
- Introduce a Defected Ground Structure into the ground plane.
- Compare the conventional and DGS configurations.
- Analyze S11, VSWR, surface-field distribution, directivity, and far-field radiation patterns.
- Study how the DGS affects the impedance characteristics of the antenna.

---

## Antenna Configurations

### Conventional Microstrip Patch Antenna

The first configuration consists of a conventional rectangular microstrip patch antenna.

![Conventional MPA](images/antenna_geometry.png)

### MPA with Defected Ground Structure

A slot was introduced into the ground structure to form the DGS configuration.

![MPA with DGS](images/dgs_geometry.png)

---

## Simulation Setup

The antenna was modeled and simulated using:

| Parameter | Value |
|---|---|
| Simulation Software | CST Studio Suite |
| Antenna Type | Microstrip Patch Antenna |
| Target Frequency | 2.4 GHz |
| Modified Structure | Defected Ground Structure |
| Analysis | S-parameters, VSWR, Surface Fields, Far Field |

---

## Results

### S11 Comparison

The conventional antenna exhibits a resonance around 2.398 GHz with a minimum S11 of approximately -38.9 dB.

After introducing the DGS, the resonance shifts slightly to approximately 2.395 GHz, while the minimum S11 improves to approximately -49.1 dB.

![S11 Comparison](images/s11_comparison.png)

### Summary

| Parameter | Conventional MPA | MPA + DGS |
|---|---:|---:|
| Resonant Frequency | 2.398 GHz | 2.395 GHz |
| Minimum S11 | -38.9 dB | -49.1 dB |
| Directivity | 6.905 dBi | 6.893 dBi |
| 3-dB Beamwidth | 79.7° | 80.0° |
| Side-lobe Level | -13.5 dB | -13.4 dB |

---

## VSWR

The simulated VSWR characteristics of both configurations are compared below.

![VSWR Comparison](images/vswr_comparison.png)

The resonance region corresponds to strong impedance matching, with the DGS configuration showing a deeper S11 minimum.

---

## Surface Field Distribution

### Conventional MPA

![Surface Field - Conventional](images/surface_current_normal.png)

### MPA with DGS

![Surface Field - DGS](images/surface_current_dgs.png)

The field distribution demonstrates strong field concentration around the resonant patch region.

---

## Radiation Characteristics

### Conventional MPA

![Far Field - Conventional](images/farfield_normal.png)

The conventional antenna exhibits a broadside radiation pattern with a main lobe directed at approximately 0°.

### MPA with DGS

![Far Field - DGS](images/farfield_dgs.png)

The DGS configuration maintains a similar broadside radiation characteristic.

---

## Comparison and Discussion

Introducing the DGS produced a noticeable change in the impedance characteristics of the antenna.

The minimum S11 improved from approximately -38.9 dB to -49.1 dB, while the resonant frequency shifted slightly from 2.398 GHz to 2.395 GHz.

The radiation characteristics remained largely unchanged:

- Directivity remained approximately 6.9 dBi.
- The main lobe remained directed at 0°.
- The 3-dB beamwidth remained close to 80°.
- The side-lobe level remained approximately -13.4 to -13.5 dB.

These results indicate that the DGS primarily influenced the impedance behavior of the antenna while producing only a small change in its far-field radiation characteristics.

---

## Key Findings

- Designed a microstrip patch antenna operating near the 2.4 GHz ISM band.
- Investigated the effect of a Defected Ground Structure.
- Obtained a minimum simulated S11 of approximately -49.1 dB with the DGS configuration.
- Observed a small downward resonance shift from 2.398 GHz to 2.395 GHz.
- Achieved approximately 6.9 dBi simulated directivity.
- Compared impedance and radiation characteristics between conventional and DGS configurations.

---

## Tools Used

- CST Studio Suite
- Electromagnetic simulation
- S-parameter analysis
- VSWR analysis
- Far-field radiation analysis

---

## Future Work

Possible extensions of this project include:

- Parametric optimization of the DGS dimensions.
- Investigation of different DGS geometries.
- Bandwidth enhancement.
- Optimization of antenna gain and efficiency.
- Fabrication and experimental validation.
- Comparison between simulated and measured results.
