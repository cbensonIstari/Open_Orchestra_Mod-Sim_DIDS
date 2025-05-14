# 2.4 EM (Electromagnetics)

This directory covers **EM** tools within the **Simulations** class, addressing **electromagnetic** phenomena like **EMI/EMC**, **antenna design**, and **radar cross-section** analysis. Representative solvers include **CST Studio Suite, ANSYS HFSS, OpenEMS, FEKO, COMSOL EM Module, Altair Feko, Keysight ADS, Remcom XFdtd, NEC, Sonnet**, and more.

---

## Structure

1. **`2.4.1-instances/`**  
   - JSON files for each electromagnetic simulation tool (CST, HFSS, OpenEMS, etc.).  
   - Each instance references **full file name** in `"Tool.File_Name"` for clarity.

2. **`2.4.2-EM_Loading_Input_Data.json`**  
   - Defines **input** data typically loaded (CAD geometry, antenna definitions, boundary conditions, material properties).

3. **`2.4.3-EM_Extraction_Output_Data.json`**  
   - Summarizes **output** data (S-parameters, far-field patterns, near-field distributions, RCS data, etc.).

4. **`2.4.4-EM_Extraction_Output.owl`** *(optional)*  
   - An ontology capturing semantic relationships: geometry → mesh → solver settings → results (like antenna patterns, scattering parameters).

---

## EM Tools Overview

- **CST Studio Suite** (`2.4.1.1-EM_CSTStudioSuite.json`)  
- **ANSYS HFSS** (`2.4.1.2-EM_ANSYSHFSS.json`)  
- **OpenEMS** (`2.4.1.3-EM_OpenEMS.json`)  
- **FEKO** (`2.4.1.4-EM_FEKO.json`)  
- **COMSOL Multiphysics EM Module** (`2.4.1.5-EM_COMSOLMultiphysicsEM.json`)  
- **Altair Feko** (`2.4.1.6-EM_AltairFeko.json`)  
- **Keysight ADS** (`2.4.1.7-EM_KeysightADS.json`)  
- **Remcom XFdtd** (`2.4.1.8-EM_RemcomXFdtd.json`)  
- **NEC (Numerical Electromagnetics Code)** (`2.4.1.9-EM_NEC.json`)  
- **Sonnet** (`2.4.1.10-EM_Sonnet.json`)

---

## How to Use

1. **Loading vs. Extraction Schemas**  
   - **`2.4.2-EM_Loading_Input_Data.json`**: typical input data (antenna geometry, waveguide BCs, material definitions, frequency sweeps).  
   - **`2.4.3-EM_Extraction_Output_Data.json`**: typical output data (S-parameters, antenna patterns, near/far fields, RCS results).

2. **Add/Update Instances**  
   - If adopting another EM solver or new version, create/edit a JSON in `2.4.1-instances/`.

3. **Optional Ontology**  
   - `2.4.4-EM_Extraction_Output.owl` can model advanced concepts (multi-port S-parameters, wave excitations, E/H field distributions) for cross-domain synergy.

---

## Relationship to Other Simulation Classes

- **2.1-LowFidelitySimulations**: Quick param sweeps might guide HPC-based EM runs.  
- **2.2-CFD**: In rare multi-physics contexts (plasma, coupling).  
- **1.1-CAD**: 3D geometry for antennas or enclosures often originates in mechanical CAD.

---

## Future Extensions

- HPC cluster integration for large-scale RCS or full system EMI.  
- Coupling with **thermal** or **structural** solvers for multi-physics (heating, mechanical stresses from EM waves).

---

## Questions or Feedback

- Refer to `[../README.md](../README.md)` for the overall **Simulations** structure.
- Check `[docs/USAGE.md](../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../docs/CONTRIBUTING.md)` for naming conventions or how to add new EM tool definitions.

**Explore these EM solvers** for a wide range of analyses (antenna design, EMI/EMC checks, radar cross-section), ensuring synergy with the broader **Open Orchestra** digital engineering environment!
