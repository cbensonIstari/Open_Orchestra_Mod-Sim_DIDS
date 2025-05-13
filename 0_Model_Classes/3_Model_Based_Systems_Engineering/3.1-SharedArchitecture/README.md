# 3.1 Shared Architecture

This folder contains **multi-user, collaborative model repository tools** under the **Model-Based Systems Engineering** class. These solutions manage concurrency, branching, and versioning for UML/SysML or related architectures, enabling distributed teams to collaborate on the same model(s) simultaneously.

---

## Structure

1. **`3.1.1-instances/`**  
   - JSON definitions for each platform that supports **shared architecture**:
     - Teamwork Cloud (No Magic/Cameo)
     - IBM Rhapsody Model Manager
     - Sparx Pro Cloud Server
     - PTC Windchill Modeler
     - Siemens Teamcenter SE
     - Eclipse Papyrus CDO
     - Capella Team (for Capella)

2. **`Example_DiD/`** *(optional)*  
   - Demo references or Data Item Description artifacts for collaborative environment deliverables.

3. **`images/`**  
   - Place screenshots illustrating multi-user concurrency, branching, merges, etc.

4. **`3.1.2-Shared_Architecture_Models_Loading_Input_Data.json`**  
   - Defines typical **input** data (repository snapshots, user/team config, partial model imports, branch definitions).

5. **`3.1.3-Shared_Architecture_Models_Extraction_Output_Data.json`**  
   - Outlines **outputs** from these repositories (revision logs, merges, user collaboration artifacts, version snapshots).

6. **`Shared_Architecture_Extraction_Output.owl`** *(optional)*  
   - If adopting a semantic approach, captures branching/versioning, collaboration logs, etc. in an ontology for advanced queries.

---

## Shared Architecture Tools Overview

- **Teamwork Cloud** (`3.1.1.1-SharedArchitecture_TeamworkCloud.json`):
  - Central DB for MagicDraw/Cameo, managing branching and versioning.  
- **IBM Rhapsody Model Manager** (`3.1.1.2-SharedArchitecture_IBMModelManager.json`):
  - Jazz-based repository enabling multi-user concurrency on Rhapsody models.  
- **Sparx Pro Cloud Server** (`3.1.1.3-SharedArchitecture_SparxProCloudServer.json`):
  - Cloud-based repository for Sparx Enterprise Architect, supporting collaborative UML/SysML.  
- **PTC Windchill Modeler** (`3.1.1.4-SharedArchitecture_PTCWindchillModeler.json`):
  - Formerly Integrity Modeler, integrates with Windchill for PLM synergy and MBSE concurrency.  
- **Siemens Teamcenter SE** (`3.1.1.5-SharedArchitecture_SiemensTeamcenterSE.json`):
  - Extended Teamcenter for systems engineering, bridging MBSE with PLM.  
- **Eclipse Papyrus CDO** (`3.1.1.6-SharedArchitecture_EclipsePapyrusCDO.json`):
  - Open source collaborative solution using CDO for multi-user UML/SysML on Eclipse Papyrus.  
- **Capella Team** (`3.1.1.7-SharedArchitecture_CapellaTeam.json`):
  - Thales extension for Capella, enabling shared model repository and concurrency on the Capella MBSE solution.

---

## How to Use

1. **Loading/Extraction Schemas**  
   - `3.1.2-Shared_Architecture_Models_Loading_Input_Data.json`: input data (branch configs, user roles, partial model merges).  
   - `3.1.3-Shared_Architecture_Models_Extraction_Output_Data.json`: output data (revision logs, user collaboration threads, version snapshots).

2. **Add/Update Instances**  
   - If a new version of any tool emerges, or a different platform is introduced, create or edit a JSON in `3.1.1-instances/`.

3. **Optional Ontology**  
   - `Shared_Architecture_Extraction_Output.owl` can capture branching, versioning, merges, concurrency logs in a semantic manner.

---

## Relationship to Other MBSE Tools

- Integrates with:
  - **Architecture Tools** (3.2) for storing the UML/SysML models,
  - **Requirements Tools** (3.3) if linking requirements or OSLC references,
  - Potential synergy with **Simulations** or **Physical System Representation** if those models are also stored or referenced in collaborative frameworks.

---

## Questions or Feedback

- See `[../../README.md](../../README.md)` for the overall MBSE structure.
- Check `[docs/USAGE.md](../../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../../docs/CONTRIBUTING.md)` for instructions on adding or updating these collaborative platforms.

**Harness the power of multi-user concurrency** for your MBSE environment—ensuring consistent, centralized **architecture** models and streamlined collaboration across your teams!
