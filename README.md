# Current Source Density Analisis for HD-MEA

For the preliminary version of this code, please refer to https://github.com/kzapfe/CSDA


![CentersOfMassTrajectories](https://github.com/LBitn/Hippocampus-HDMEA-CSDA/blob/main/CentersOfMassTrajectories.gif)

- This methodology provides a means to define the center of mass of sinks and sources over time with high spatiotemporal resolution in brain slices, which can help infer transmission information.
Using CSD analysis, a disjoint component analysis allows for the dissection of restricted synaptic activation, which is obscured by high-voltage electrographic elements. Additionally, subthreshold activity, not overtly detected in voltage recordings, can be better defined and quantitatively traced.

---
*First Version, September 2024
---

The following codes contain the methods described in the following article:

- Zapfe, K.W.P., Romero-Maldonado, I., Gutiérrez, R., High Resolution Detection of Stationary and Evolving 2D-Current Source Density within Neuronal Microcircuits.

Created with data extracted from High Density Multielectrode Arrays (HD-MEAs, 3Brain) using slices of rodent hippocampal tissue in mind.

-- Step 00: data preprocessing. Conversion from HDF5 (brw) to jld (native julia) format and segmentation to improve data manageability.

-- Step 01: Detection of recording errors and debugging of discontinuities in the signals.

-- Step 02: Voltage to current flow conversion ( sink and sources ). Detection of centers of mass and tracing of center-of-mass trajectories.

-- ACD: Detection of channels corresponding to viable tissue. Separation of channels providing physiological signal from noise.


This code is released under GPL-3.0.

### Supported systems <a name="systems"></a>

- This software was developed specifically for high density multielectrode arrays [3Brain](http://3brain.com/) BIOCAM X

## How to use <a name="quickstart"></a>

The code has been written and tested in Julia language, versions 1.7.2 and 1.10.2, using Jupyter Notebooks and free text editors, on several Linux distributions as well as on Windows 10.

All the packages and functions are properly described at the beginning of each module or notebook

## Contributors, alphabetical <a name="people"></a>

- [Angel Vazquez Flores](https://github.com/Angeldk16): Parameter optimisation, Test
- Fransisco Victorio Santiago: Test and sugestions
- [Isabel Romero Maldonado](https://github.com/LBitn): Codes and Data Analysis
- Jorge Hernandez Garcia: Test and sugestions
- [Karel Zapfe Aguilar](https://github.com/kzapfe): Author of the concept and source codes
- Luis Ramos Gonzalez: Test and Optimisation
- [Rafael Gutiérrez Aguilar](rafagut@cinvestav.mx): Conceived and designed research
## Contact <a name="contact"></a>

Dr. R. Gutiérrez is based at Department of Pharmacobiology, Centro de Investigación y Estudios Avanzados del Instituto Politécnico Nacional. Please contact the following e-mail:
rafagut@cinvestav.mx
