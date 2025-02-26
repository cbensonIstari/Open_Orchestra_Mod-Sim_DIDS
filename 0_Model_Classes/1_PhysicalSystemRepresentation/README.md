# 1. Physical System Representation

This directory contains **Digital Engineering Model Types** and **tool instances** used to describe the **physical aspects** of a system—primarily **mechanical, electrical**, and **lifecycle** elements. Within this folder, you will find **subfolders** corresponding to **major** Physical System Representation categories, such as:

1. **1.1-CAD/**  
   - Tools and schemas for **Computer-Aided Design**, used to create 3D/2D mechanical models (e.g., airframe geometry, structural components).  

2. **1.2-ECAD/** *(if present)*  
   - Tools for **Electronic CAD**, focusing on PCB design, wiring harness layouts, and avionics integration.  

3. **1.3-PLM/** *(if present)*  
   - **Product Lifecycle Management** systems that handle part data, revisions, BOMs, and change processes throughout the product lifecycle.

## Contents

- **README.md**: This file, describing the purpose and organization of the Physical System Representation folder.
- **Subfolders** (e.g., `1.1-CAD/`, `1.2-ECAD/`, `1.3-PLM/`):
  - Each subfolder includes:
    - A `README.md` explaining the **model type** (CAD, ECAD, or PLM).
    - An `instances/` subfolder containing example **tool instance** JSON files (e.g., `CAD_CreoParametric.json`).
    - Two JSON schema files for **Loading (Input)** and **Extraction (Output)** data, describing typical data formats and standards for that **model type**.

## How to Use

1. **Explore a Specific Model Type**  
   - For example, in `1.1-CAD/` you’ll find `instances/` with detailed JSON files for tools like Creo, Siemens NX, CATIA, and FreeCAD.

2. **Review the Input/Output Schemas**  
   - Each model type folder (e.g., `1.1-CAD/`) includes `1.1.2-CAD_Loading_Input_Data.json` and `1.1.3-CAD_Extraction_Output_Data.json`, defining how data is typically loaded into or extracted from those tools.

3. **Extend the Directory**  
   - If you need to add another type of **Physical System Representation** tool (e.g., specialized geometry or mechanical library), create a new subfolder (e.g., `1.4-XYZ`) following the same structure.

4. **Reference in Ecosystems**  
   - Tools listed here are often referenced by **ecosystem** JSON files in `ecosystems/` (e.g., `DEE_Simple.json`). This approach integrates each tool instance (CAD, ECAD, PLM) into an overall Digital Engineering workflow.

## Rationale

The **Physical System Representation** domain ensures a robust foundation for:
- **Mechanical Geometry** (3D design, drawings, parametric models)
- **Electrical Layout** (PCBs, harnesses, avionics integration)
- **Lifecycle Data** (BOMs, versions, change requests)  
providing consistent **configuration management** and **traceability** across the product lifecycle. 

## Contributing

- For guidelines on adding or modifying **tool instance** JSON files, see the main [CONTRIBUTING.md](../../docs/CONTRIBUTING.md).
- Ensure new subfolders and JSON schemas follow the **numbered** pattern and naming conventions in this repository.

---

**Questions?** Contact the **CAD/ECAD/PLM** domain lead or open an issue in the main GitHub repo. 
