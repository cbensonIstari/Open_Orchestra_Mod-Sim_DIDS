# 1.1 CAD (Computer-Aided Design)

This folder stores **CAD**-related model definitions, which are part of the **Physical System Representation** class. CAD tools focus on **mechanical/structural** design, often in 2D/3D formats.

## Structure

- **1.1.1-instances/**  
  Contains JSON definitions for each CAD tool instance.  
  - `1.1.1.1-CAD_CreoParametric.json`  
  - `1.1.1.2-CAD_SiemensNX.json`  
  - `1.1.1.3-CAD_CATIA.json`  
  - `1.1.1.4-CAD_FreeCAD.json`  
- **1.1.2-CAD_Loading_Input_Data.json**  
  JSON schema describing how data (geometry, material properties, etc.) is **loaded** into CAD tools.  
- **1.1.3-CAD_Extraction_Output_Data.json**  
  JSON schema describing what **outputs** can be extracted (mass properties, neutral files, BOM, etc.) from CAD models.

## Usage

1. **Browse Instances**  
   - If you want to see how we define each CAD tool (e.g., licensing, version), open the corresponding JSON in `1.1.1-instances/`.
2. **Review Schemas**  
   - Check `1.1.2-CAD_Loading_Input_Data.json` for typical input data (like `.step`, `.iges`), and `1.1.3-CAD_Extraction_Output_Data.json` for typical outputs (like `.stl`, bounding box data).
3. **Reference in Ecosystems**  
   - The `ecosystems/` folder may reference these tools in `DEE_Simple.json`, `DEE_Moderate.json`, or `DEE_Comprehensive.json`.

## Why CAD?

- **Geometry Definition**: Precise 3D/2D modeling is vital for mechanical design, stress analysis, and manufacturing.
- **Integration**: CAD geometry often feeds simulation tools (CFD, FEA) or PLM systems for revision tracking.

## Contributing

- Follow the [CONTRIBUTING.md](../../../docs/CONTRIBUTING.md) for naming conventions and JSON structure.
- Keep tool instance files consistent with the input/output schemas in this folder.
