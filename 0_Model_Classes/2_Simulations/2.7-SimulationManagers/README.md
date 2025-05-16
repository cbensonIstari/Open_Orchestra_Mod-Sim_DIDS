# 2.7 Simulation Managers

This directory focuses on **tools that orchestrate and manage** large or multi-domain simulations, handling **workflow integration**, **param sweeps**, **optimization**, and **co-simulation**. Examples include **ANSYS Workbench, Phoenix Integration ModelCenter, OpenMDAO, ESTECO modeFRONTIER, Siemens HEEDS, Simulia Isight, Altair HyperStudy, Dakota**, etc.

---

## Structure

1. **`2.7.1-instances/`**  
   - JSON files defining each **simulation manager** or **workflow orchestrator**:
     - ANSYS Workbench  
     - ModelCenter  
     - OpenMDAO  
     - modeFRONTIER  
     - HEEDS  
     - Isight  
     - HyperStudy  
     - Dakota

2. **`2.7.2-SimulationManagers_Loading_Input_Data.json`**  
   - Describes **input** data typically required for these tools (project workflows, solver integration, param definitions).

3. **`2.7.3-SimulationManagers_Extraction_Output_Data.json`**  
   - Summarizes **output** data (param sweeps, optimization results, job logs, final selected design, trade-off curves).

4. **`2.7.4-SimulationManagers_Extraction_Output.owl`** *(optional)*  
   - A semantic representation of the orchestrated tool-chains, param sets, or optimization processes—useful for advanced queries or cross-domain synergy.

---

## Simulation Manager Tools Overview

- **ANSYS Workbench**: Integrates multiple ANSYS solvers in a single workflow.  
- **ModelCenter**: Phoenix Integration for multi-tool orchestration, param sweeps, design optimization.  
- **OpenMDAO**: NASA open-source for MDAO frameworks, plugin-based approach.  
- **modeFRONTIER**: ESTECO environment for robust optimization, param handling.  
- **HEEDS**: Siemens solution for multi-disciplinary design exploration.  
- **Isight**: SIMULIA (Dassault) tool for param-based optimization, linking multiple solvers.  
- **HyperStudy**: Altair’s environment for design exploration and optimization.  
- **Dakota**: Sandia open-source for param sweeps, UQ, optimization across HPC.

---

## How to Use

1. **Loading vs. Extraction Schemas**  
   - **`2.7.2-SimulationManagers_Loading_Input_Data.json`**: typical inputs (workflows, tool references, param definitions, HPC settings).  
   - **`2.7.3-SimulationManagers_Extraction_Output_Data.json`**: typical outputs (optimization runs, best design sets, job logs, trade-off data).

2. **Add/Update Instances**  
   - If a new orchestration tool is introduced or updated, create a new JSON in `2.7.1-instances/`.

3. **Ontology**  
   - `2.7.4-SimulationManagers_Extraction_Output.owl` can represent tool-chains, param sets, or optimization results to facilitate advanced analysis or domain synergy.

---

## Relationship to Other Simulation Classes

- **2.1–2.6**: The simulation manager might orchestrate any combination of low-fidelity, CFD, FEA, EM, dynamic, or mission-level models.  
- **1.1-CAD** or **1.2-ECAD**: Parametrically updated geometry might feed the orchestrated workflows.  
- **3-ModelBasedSystemEngineering**: Ties to SysML param diagrams or requirement constraints for an integrated design loop.

---

## Future Extensions

- HPC-based large param sweeps, reliability-based design, or robust optimization.  
- Linking with **PLM** or **MBSE** for closed-loop product development.

---

## Questions or Feedback

- See `[../README.md](../README.md)` for the overall **Simulations** directory structure.
- Refer to `[docs/USAGE.md](../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../docs/CONTRIBUTING.md)` for how to propose new manager tools or adapt schemas.

**Orchestrate multi-domain** analyses with these **Simulation Managers**, ensuring a cohesive approach in the **Open Orchestra** digital engineering environment!
