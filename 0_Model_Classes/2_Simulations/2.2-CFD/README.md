# 2.2 CFD (Computational Fluid Dynamics)

This folder focuses on **CFD** tools under the **Simulations** class. These solutions handle **fluid/thermal flow analyses**, providing detailed aerodynamic, thermal, or multi-physics insights. Examples include **ANSYS Fluent, Star-CCM+, OpenFOAM, Siemens Simcenter FLOEFD, Autodesk CFD, COMSOL CFD, Dassault PowerFLOW, NUMECA FINE, SU2, CFD++**, and more.

---

## Structure

1. **`2.2.1-instances/`**  
   - JSON files for each CFD tool instance, with **full file names** included in the `"Tool"` object for clarity:
     - **`2.2.1.1-CFD_ANSYSFluent.json`**
     - **`2.2.1.2-CFD_StarCCMplus.json`**
     - … etc.

2. **`2.2.2-CFD_Loading_Input_Data.json`**  
   - Defines **input** data typically loaded into CFD tools (geometry meshes, boundary condition files, control dictionaries).

3. **`2.2.3-CFD_Extraction_Output_Data.json`**  
   - Summarizes **output** data from CFD (plots, solution fields, post-processing, mesh stats, logs).

4. **`CFD_Extraction_Output.owl`** *(optional)*  
   - Captures a **semantic** approach (meshes, boundary conditions, result fields) if advanced queries or cross-domain synergy are needed.

---

## CFD Tools Overview

- **ANSYS Fluent** (`2.2.1.1-CFD_ANSYSFluent.json`): A widely used commercial solver for fluid/thermal flows.  
- **Star-CCM+** (`2.2.1.2-CFD_StarCCMplus.json`): Siemens PLM solution for multi-physics, including advanced meshing and flow.  
- **OpenFOAM** (`2.2.1.3-CFD_OpenFOAM.json`): Open-source CFD framework for custom solvers, wide param coverage.  
- **Siemens Simcenter FLOEFD** (`2.2.1.4-CFD_SiemensSimcenterFLOEFD.json`): Embedded CFD into mechanical CAD contexts.  
- **Autodesk CFD** (`2.2.1.5-CFD_AutodeskCFD.json`): Cloud-enabled or local solver for fluid flow, thermal, design iteration.  
- **COMSOL Multiphysics CFD Module** (`2.2.1.6-CFD_COMSOLMultiphysicsCFDModule.json`): Part of COMSOL environment for multi-physics combos.  
- **Dassault PowerFLOW** (`2.2.1.7-CFD_DassaultPowerFLOW.json`): Lattice-Boltzmann approach for automotive/aero external flows.  
- **NUMECA FINE** (`2.2.1.8-CFD_NUMECAFINE.json`): Specialized in turbomachinery, external aero, multi-block meshing.  
- **SU2** (`2.2.1.9-CFD_SU2.json`): Open-source for compressible/incompressible flows, adjoint-based shape optimization.  
- **CFD++** (`2.2.1.10-CFD_CFD++.json`): Another commercial solver known for complex flow cases.

---

## How to Use

1. **Load vs. Extraction Schemas**  
   - **`2.2.2-CFD_Loading_Input_Data.json`**: typical inputs (mesh files, geometry imports, boundary conditions, param files).  
   - **`2.2.3-CFD_Extraction_Output_Data.json`**: typical outputs (solution fields, residual logs, convergence data, post-processed images).

2. **Add/Update Instances**  
   - If new CFD tools appear or versions change, create or edit the corresponding JSON in `2.2.1-instances/`.

3. **Optional Ontology**  
   - `CFD_Extraction_Output.owl` can capture semantic relationships (mesh → boundary condition set → solution field) for advanced queries or cross-domain synergy with MBSE or HPC.

---

## Relationship to Other Simulation Classes

- **2.1-LowFidelitySimulations**: Quick or conceptual analyses might inform CFD boundary conditions or initial geometry shape.  
- **2.3-FEA**: Structural analyses can pair with fluid loads from CFD.  
- **1.1-CAD** or **1.2-ECAD**: Geometry must be consistent with mechanical/electronic design contexts.

---

## Future Extensions

- **HPC Integration**: If large-scale runs are performed, tie HPC cluster job management data.  
- **Multi-Disciplinary**: Coupling with FEA or flight dynamics for co-sim approaches.

---

## Questions or Feedback

- Refer to `[../README.md](../README.md)` for the overall **Simulations** structure.
- Check `[docs/USAGE.md](../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../docs/CONTRIBUTING.md)` for naming conventions or how to propose new tools or file references.

**Delve into these CFD tools** for advanced fluid/thermal simulations, bridging conceptual shapes to robust flow solutions in the **Open Orchestra** digital ecosystem!
