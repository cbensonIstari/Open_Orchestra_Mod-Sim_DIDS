# Example Digital DID: Physical System Representation (CAD) — DI-MNT-90101A

This folder contains **digital deliverables** for a **Physical System Representation** Data Item Description (**DID**), specifically aligned with **DI-MNT-90101A** or similar DoD guidelines for CAD designs. 

## Contents

1. **DID Documents**  
   - **DI-MNT-90101A - PhysicalSystemRepresentation-Overview.pdf**  
   - **DI-MNT-90101A - PhysicalSystemRepresentation-Requirements.pdf**  
   - **DI-MNT-90101A - PhysicalSystemRepresentation-Appendix.pdf**  
   These PDF documents provide the official description, scope, and submission requirements for this DID artifact.

2. **CAD/Model Files**  
   - **WING.CATPart**: Native CAD part file for the wing geometry (CATIA format).  
   - **wing.obj**: Neutral or visualization-oriented 3D mesh.  
   - **bill_of_materials.json**: JSON-based BOM (bill of materials) specifying part items, quantities, and references.  
   - **mass_properties.json**: Contains mass, inertia, center of gravity data, possibly extracted from the CAD model.  
   - **parameters.json**: Basic parameter definitions (e.g., chord length, wingspan, sweep angle).

3. **README.md** (This file)  
   Explains how the digital DID is organized, references each deliverable artifact, and describes how they support the contract or program requirements.

4. **Other Supporting Files**  
   - **1.1.2-CAD_Loading_Input_Data.json**: Generic JSON schema describing how data is loaded into CAD (from the parent folder).  
   - **1.1.3-CAD_Extraction_Output_Data.json**: Generic JSON schema describing typical outputs from CAD.

> **Note**: The subfolder structure is part of the broader `1.1-CAD/` hierarchy in the `digital-eng-tools` repository.

## Purpose of the DID

- **Clarity & Consistency**: Provide **standard** mechanical representation data (CAD geometry, BOM, parameters, etc.) to ensure consistent communication and interoperability.
- **Digital-First**: Comply with modern DoD digital engineering practices, offering data in **JSON** and **open** or **standard** file formats (e.g., `.OBJ`, `.CATPart`).
- **Traceability**: Links to higher-level MBSE requirements and simulations in the broader repository.

## File Descriptions

1. **WING.CATPart**  
   - *Format*: CATIA part file.  
   - *Use*: Full-fidelity geometry for the UAV wing.  
   - *Dependencies*: Can be converted to `.step` or `.iges` for interchange with other CAD systems.

2. **wing.obj**  
   - *Format*: Wavefront OBJ, typically for visualization or quick geometry references.  
   - *Use*: 3D rendering in lightweight viewers, AR/VR environments, or digital twin solutions.

3. **bill_of_materials.json**  
   - *Format*: JSON array listing each part/subpart, quantity, part IDs, potential references to MPN (manufacturer part numbers).  
   - *Use*: Integrates with PLM or other BOM-management systems to track items in the wing assembly.

4. **mass_properties.json**  
   - *Format*: JSON object providing mass, center of gravity, moment of inertia, bounding box.  
   - *Use*: Inputs for structural analysis, flight dynamics, or logistic planning (weight & balance checks).

5. **parameters.json**  
   - *Format*: JSON enumerating key design parameters (e.g., chord length, wingspan, airfoil type).  
   - *Use*: Supports parametric updates in CAD or analysis scripts.

6. **DI-MNT-90101A - PhysicalSystemRepresentation-*.pdf**  
   - *Format*: Official DID documentation in PDF format.  
   - *Use*: Defines deliverable scope, data fields, compliance details, and instructions for DoD acquisitions.

## Workflow & Integration

- **CAD Creation**: Wing geometry created in CATIA (represented by `WING.CATPart`).  
- **Neutral/Lightweight Export**: For cross-tool collaboration, an `.obj` file is generated for quick viewing and AR/VR.  
- **Data Extraction**: BOM and mass properties exported as JSON, aligning with `1.1.3-CAD_Extraction_Output_Data.json` guidelines.  
- **Parametric Linking**: `parameters.json` can feed future design automation or parametric trade studies (e.g., in MATLAB or MBSE tools).

## Compliance & InfoSec

- All deliverables align with [ASME Y14.41](https://www.asme.org/codes-standards), [ISO 10303 (STEP)](https://www.iso.org/standard/51379.html) references, and **DI-MNT-90101A** guidelines for model-based deliverables.
- **InfoSec_Level**: *ITAR/CUI sensitivity*—files should remain in secure repositories.  
- Access controlled by role-based IAM as described in the overarching repository.

## Additional Notes

- This example DID supplements the **traditional** PDF approach (see `.pdf` files) with **digital-first** artifacts (`.json`, `.CATPart`, `.obj`).
- Future expansions might include a **configuration** or **revision** XML/JSON (tracking part version, revision notes, or unique IDs).

---

**Questions?**  
- Contact the **CAD Tool POC** or consult the main `[README.md](../README.md)` in the `1.1-CAD/` parent folder for more context on how these files tie into the broader Digital Engineering repository.  
- Refer to the `[docs/USAGE.md](../../../docs/USAGE.md)` for instructions on loading or extracting data from these CAD artifacts.

