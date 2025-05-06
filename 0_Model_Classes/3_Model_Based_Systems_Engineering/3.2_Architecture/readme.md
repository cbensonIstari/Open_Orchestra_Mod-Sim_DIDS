# 3.2 Architecture Tools

This folder hosts **UML/SysML modeling** tools under the **Model-Based Systems Engineering (MBSE)** class. Architecture tools define system **structure**, **behavior**, **requirements traceability**, and **parametric constraints**, typically using **UML**, **SysML**, **UAF**, or **custom domain profiles**.

---

## Structure

1. **`3.2.1-instances/`**  
   - JSON definitions of each **Architecture Tool** (Cameo Systems Modeler, IBM Rhapsody, Sparx EA, Modelio).  
   - Each file follows the standard format with `"Tool"`, `"Licensing"`, `"Access_Control"`, `"Deployment"`, and `"Plugins"`.

2. **`Example_DiD/`** *(optional)*  
   - Demonstration artifacts or Data Item Description examples, such as a sample `.pdf` detailing how architecture deliverables might be packaged.

3. **`images/`**  
   - Place tool screenshots (e.g., UML diagrams, SysML parametric diagrams) or conceptual MBSE workflows here.

4. **`3.2.2-Architecture_Models_Loading_Input_Data.json`**  
   - Defines **input** data typically loaded into an architecture tool: UML profiles, SysML stereotypes, external requirements (e.g., `.reqif`), versioned model files.

5. **`3.2.3-Architecture_Models_Extraction_Output_Data.json`**  
   - Outlines typical **outputs** from an architecture tool: UML diagrams, SysML diagrams, XMI exports, HTML/PDF reports, etc.

6. **`Architecture_Extraction_Output.owl`** *(optional)*  
   - If adopting a semantic approach, this `.owl` file can represent UML/SysML concepts or relationships in an ontology.  
   - Allows advanced reasoning or cross-tool queries if needed.

---

## UML/SysML Tools Overview

In **`3.2.1-instances/`**, you’ll find:

- **Cameo Systems Modeler** (`3.2.1.1-ArchitectureTools_CameoSystemsModeler.json`)  
- **IBM Rhapsody** (`3.2.1.2-ArchitectureTools_Rhapsody.json`)  
- **Sparx Enterprise Architect** (`3.2.1.3-ArchitectureTools_SparxEA.json`)  
- **Modelio** (`3.2.1.4-ArchitectureTools_Modelio.json`)  

These define each tool’s vendor, version, licensing, deployment, and any plugins (e.g., SysML, UAF, BPMN add-ons).

---

## How to Use

1. **Input/Output Schemas**  
   - `3.2.2-Architecture_Models_Loading_Input_Data.json` details standard UML/SysML model inputs (XMI, UML2 files, .reqif for requirements, etc.).  
   - `3.2.3-Architecture_Models_Extraction_Output_Data.json` covers typical exports (XMI, UML diagrams in `.svg`, HTML/PDF documentation, integrated requirements).

2. **Add/Update Instances**  
   - Create or modify JSON definitions in `3.2.1-instances/`. For example, if you adopt a new version of Cameo or a new plugin, update the `"Version"` or `"Plugins"` array.

3. **Optional Ontology**  
   - If advanced semantic modeling is required, see `Architecture_Extraction_Output.owl` for a demonstration on how UML/SysML elements might be captured in an OWL-based ontology.

---

## Relationship to Other Classes

- MBSE architecture tools often link to:
  - **Requirements** tools in `3.3-RequirementsTools/` for direct traceability.
  - **Simulations** in `2-Simulations/` if parametric or state machine models feed simulation data.
  - **CAD/ECAD** in `1_PhysicalSystemRepresentation/` for morphological or structural alignment.

---

## Questions or Feedback

- Refer to the main `[README](../../README.md)` in the `0_Model_Classes/` folder for overall repository context.
- Consult `[docs/USAGE.md](../../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../../docs/CONTRIBUTING.md)` for guidelines on naming conventions or how to submit a new tool instance.

**Enjoy orchestrating your UML/SysML** models within the broader **Open Orchestra** approach to digital engineering!

