# 2.1 Low-Fidelity Simulations

This folder focuses on **low-fidelity simulation** tools under the **Simulations** class. These tools provide **early, approximate analyses** for conceptual design, trade studies, or quick parametric evaluations in domains like aerodynamics, flight performance, or general system behavior.

---

## Structure

1. **`2.1.1-instances/`**  
   - JSON definitions for each low-fidelity simulation tool, including:
     - **OpenVSP** (geometry-based aerodynamic analysis)
     - **AVL** (Athena Vortex Lattice)
     - **XFLR5** or other conceptual aero codes
     - **ExcelTradeStudy** (Excel-based parametric or performance calculations)
     - **Matlab** (scripts or quick M-files for analyses)
     - **Simulink** (conceptual block diagrams for dynamic or control)
     - **PythonParametric** (Python-based parametric analyses)
     - **ModelCenter** (quick trade study environment)

2. **`Example_DiD/`** *(optional)*  
   - Could store demonstration Data Item Descriptions or sample input scripts.

3. **`images/`**  
   - Place screenshots or diagrams illustrating **low-fidelity** analysis flows (e.g., geometry in OpenVSP, Excel-based trades, etc.).

4. **`2.1.2-LowFidelitySim_Loading_Input_Data.json`**  
   - Defines typical **input** data for these low-fidelity simulations (geometry files, spreadsheets, param scripts, etc.).

5. **`2.1.3-LowFidelitySim_Extraction_Output_Data.json`**  
   - Details the **outputs** from these simulation runs (results spreadsheets, basic aerodynamic polars, performance metrics, etc.).

6. **`LowFidelitySim_Extraction_Output.owl`** *(optional)*  
   - If adopting a **semantic** approach, captures the fundamental concepts (input geometry, param sets, basic result fields) for advanced queries or cross-domain synergy.

---

## Low-Fidelity Tools Overview

In **`2.1.1-instances/`**, you’ll find:

- **OpenVSP** (`2.1.1.1-LowFidelitySim_OpenVSP.json`): NASA’s open-source parametric geometry tool for quick aero shaping.  
- **AVL** (`2.1.1.2-LowFidelitySim_AVL.json`): Athena Vortex Lattice for aerodynamic or stability derivatives.  
- **ExcelTradeStudy** (`2.1.1.3-LowFidelitySim_ExcelTradeStudy.json`): Using Excel spreadsheets to do quick trade or param analyses.  
- **Matlab** (`2.1.1.4-LowFidelitySim_Matlab.json`): Script-based or basic function-based modeling.  
- **Simulink** (`2.1.1.5-LowFidelitySim_Simulink.json`): Conceptual block diagrams or simplified dynamic/controls.  
- **PythonParametric** (`2.1.1.6-LowFidelitySim_PythonParametric.json`): Scripts with NumPy, SciPy, or custom param libraries.  
- **ModelCenter** (`2.1.1.7-LowFidelitySim_ModelCenter.json`): A multi-tool environment for quick trades or integrator-based simulation.

---

## How to Use

1. **Loading vs. Extraction Schemas**  
   - **`2.1.2-LowFidelitySim_Loading_Input_Data.json`**: typical input data (geometry, param config, spreadsheets, etc.).  
   - **`2.1.3-LowFidelitySim_Extraction_Output_Data.json`**: typical output (aero coefficients, performance metrics, lightweight data for quick iteration).

2. **Add/Update Instances**  
   - If you adopt a new conceptual tool or script set, create an instance JSON (e.g., `2.1.1.8-LowFidelitySim_CustomPyScript.json`) referencing the same format.

3. **Ontology**  
   - `LowFidelitySim_Extraction_Output.owl` can represent how geometry or param sets map to results in a semantic manner for advanced queries or cross-domain synergy with MBSE or HPC.

---

## Relationship to Other Simulation Classes

- **2.2-CFD** or **2.3-FEA**: The low-fidelity results might feed or lead into more advanced domain analyses.  
- **3-ModelBasedSystemEngineering**: Requirements or param constraints might come from SysML, bridging to these quick conceptual runs.  
- **1.1-CAD**: Geometry can be simplified or exported to low-fidelity tools (like **OpenVSP** to refine shape prior to higher fidelity CAD).

---

## Future Extensions

- Linking **low-fidelity** environment to HPC or advanced multi-disciplinary optimization.  
- Storing these param sets or results in a consistent **semantic** approach if you need cross-organization trade studies.

---

## Questions or Feedback

- Refer to the main `[../README.md](../README.md)` in the `2-Simulations/` folder for overall simulation structure.
- Check `[docs/USAGE.md](../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../docs/CONTRIBUTING.md)` if you’re adding new JSON definitions or adjusting naming conventions.

**Leverage these simpler, faster** analyses for **rapid iteration** and conceptual decisions—key to the **Open Orchestra** digital engineering approach!
