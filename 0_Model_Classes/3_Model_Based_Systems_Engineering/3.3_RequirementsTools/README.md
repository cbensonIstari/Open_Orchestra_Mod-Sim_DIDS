# 3.3 Requirements Tools

This folder contains **requirements management** tools within the **Model-Based System Engineering** class. These tools capture, link, and manage **textual or model-based requirements**, often integrating with UML/SysML architecture or other systems for **traceability**.

---

## Structure

1. **`3.3.1-instances/`**  
   - JSON definitions of each **Requirements Tool** (DOORS Next, Jama, Polarion).
   - Each file follows the standard format (`Tool`, `Licensing`, `Access_Control`, `Deployment`, `Plugins`).

2. **`Example_DiD/`** *(optional)*  
   - Stores demonstration Data Item Description examples or extra references. Could also include sample requirement sets, .reqif examples, or custom .xml exports.

3. **`images/`**  
   - Place screenshots or diagrams illustrating **requirement** workflows, linking, or traceability.

4. **`3.3.2-Requirements_Models_Loading_Input_Data.json`**  
   - Defines **input data** typically loaded into these requirements tools: .reqif, .csv/.xlsx, project archives, etc.

5. **`3.3.3-Requirements_Models_Extraction_Output_Data.json`**  
   - Outlines **outputs** from such tools: .reqif exports, .csv or HTML/PDF reports, trace matrices, versioned archives, etc.

6. **`Requirements_Extraction_Output.owl`** *(optional)*  
   - Provides a **semantic** representation of requirement data (IDs, text, attributes, links to design or test) if an ontology-based approach is desired.

---

## Requirements Tools Overview

- **DOORS Next** (`3.3.1.1-RequirementsTools_DoorsNext.json`): IBM’s solution for high-level requirement sets, linking, and enterprise integration.  
- **Jama** (`3.3.1.2-RequirementsTools_Jama.json`): Another modern solution supporting web-based requirements definition and collaboration.  
- **Polarion** (`3.3.1.3-RequirementsTools_Polarion.json`): Siemens’ ALM solution with integrated versioning, workflow, and requirement linking.

Each tool can **import** or **export** data in various formats (.reqif, .csv, .docx) and is typically integrated with MBSE or other system engineering domains.

---

## How to Use

1. **Load/Extraction Schemas**:  
   - `3.3.2-Requirements_Models_Loading_Input_Data.json` describes standard requirement input (e.g., .reqif, .csv, .xlsx, project archives).  
   - `3.3.3-Requirements_Models_Extraction_Output_Data.json` details typical outputs (reports, .reqif, .csv for analysis, metadata).

2. **Add/Update Instances**:  
   - If your organization adopts a new requirements tool or version, create a new instance JSON (e.g., `3.3.1.4-RequirementsTools_MyReqTool.json`), and fill in the appropriate vendor info, deployment details, and licensing type.

3. **Optional Ontology**:  
   - `Requirements_Extraction_Output.owl` can represent core requirement concepts (IDs, priority, status, trace links) for advanced semantic queries.

---

## Relationship to Other Classes

- **MBSE**: Requirements are frequently linked to SysML models in `3.2-ArchitectureTools/` or to system behavior, structure, or parametric constraints.  
- **Simulations**: Requirements might define performance thresholds that feed or govern simulation tasks.  
- **Productivity**: Some teams export or share requirements in Word/Excel (found under Productivity Tools), referencing the same data.

---

## Future Extensions

- **Requirements + Test**: Tools may also link to test management solutions (e.g., TestRail, Jenkins pipeline for verification).
- **Semantic Reasoning**: Ontology-based reasoning could help identify incomplete traceability or conflicting requirements.

---

## Questions or Feedback

- Check `[../../README.md](../../README.md)` in `0_Model_Classes/` for the overall repository structure.
- Refer to `[docs/USAGE.md](../../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../../docs/CONTRIBUTING.md)` for instructions on naming conventions or how to add new tools or file references.

Happy requirements capturing—ensuring a robust **traceability** from concept to design, and linking seamlessly with the **Open Orchestra** approach to digital engineering!
