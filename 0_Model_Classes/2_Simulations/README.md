# 2. Simulations

This directory encompasses **simulation-focused** Digital Engineering Model Types, used to analyze or predict system behavior across various domains (aerodynamic, structural, electromagnetic, mission-level, etc.).

## Subfolders

Within **`2-Simulations`**, you may see:

1. **2.1-LowFidelitySimulations/**  
   - Early, approximate analyses (e.g., OpenVSP, spreadsheet-based trade studies) for conceptual design.
2. **2.2-CFD/** (Computational Fluid Dynamics)  
   - Tools like ANSYS Fluent, Star-CCM+, or OpenFOAM for fluid/thermal flow analyses.
3. **2.3-FEA/** (Finite Element Analysis)  
   - Tools such as MSC Nastran, Abaqus, Calculix for structural, thermal, or vibration studies.
4. **2.4-EM/** (Electromagnetics)  
   - Tools like CST Studio Suite, Ansys HFSS, OpenEMS for EMI, antenna design, and radar cross-section.
5. **2.5-Dynamic/** (Motion / Rigid-Body Dynamics)  
   - Tools such as MSC ADAMS, Simscape, MBDyn for mechanical system dynamics.
6. **2.6-MissionModels/**  
   - Tools like AFSIM, STK, or custom in-house for mission-level or operational scenario analyses.
7. **2.7-SimulationManagers/**  
   - Tools for orchestrating and managing large or multi-domain simulations (ANSYS Workbench, Phoenix ModelCenter, OpenMDAO).

Each **Model Type** folder has:
- A `README.md` explaining the simulation domain,
- An `instances/` subfolder with JSON definitions for specific tools (e.g., `CFD_ANSYSFluent.json`),
- Two JSON schema files describing typical **loading** (`*_Loading_Input_Data.json`) and **extraction** (`*_Extraction_Output_Data.json`) processes.

## Usage

1. **Identify the Simulation Domain**  
   - If you need aerodynamic analysis, head to `2.2-CFD/`. For structural studies, see `2.3-FEA/`.

2. **Check Tool Instances**  
   - Look in `instances/` for each subfolder to see how we define a simulation tool’s version, licensing, and deployment.

3. **Review Input/Output Schemas**  
   - Each model type has a pair of JSON files describing what data is loaded (e.g., geometry, mesh files) and what data is extracted (e.g., stress plots, flow fields).

## Integration with Other Classes

Simulations often integrate with:
- **Physical System Representation** (CAD or ECAD geometry),
- **MBSE** (system-level architectures that define parametric or mission analyses),
- **Productivity Tools** (Excel for data manipulation, Word/PowerPoint for reporting).

## Contributing

Please see the main [CONTRIBUTING.md](../../docs/CONTRIBUTING.md) for guidelines on adding or updating simulation tool definitions.
