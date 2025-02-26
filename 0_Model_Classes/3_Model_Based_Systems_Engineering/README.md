# 3. Model-Based System Engineering (MBSE)

This directory hosts **MBSE**-related Model Types and tools. MBSE focuses on representing system requirements, architectures, and interfaces in a centralized, structured model.

## Subfolders

1. **3.1-SharedArchitecture/**  
   - Tools that support multi-user, collaborative model repositories (Teamwork Cloud, IBM Rhapsody Model Manager, etc.).
2. **3.2-ArchitectureTools/**  
   - UML/SysML modeling tools (Cameo Systems Modeler, IBM Rhapsody, Sparx EA, Modelio) used to define system structure, behavior, and parametric constraints.
3. **3.3-RequirementsTools/**  
   - Tools for capturing, linking, and managing textual or model-based requirements (DOORS Next, Jama, Polarion).

Each subfolder includes:
- A `README.md` describing that MBSE domain segment,
- An `instances/` folder with specific tool JSON definitions (e.g., `SharedArchitecture_TeamworkCloud.json`),
- Two JSON schema files defining **loading** (`*_Loading_Input_Data.json`) and **extraction** (`*_Extraction_Output_Data.json`) data.

## Why MBSE?

- **Centralized Requirements**: Ensures all stakeholders reference a single model.  
- **Traceability**: Links requirements to architecture and test artifacts.  
- **System Architecture**: Encourages consistent interfaces, parametric analysis, and domain integration.

## Integration with Other Classes

- **Simulations**: MBSE parametric diagrams or constraints can feed advanced simulations (CFD, FEA, mission models).  
- **Physical System Representation**: Architecture sets the context for CAD/ECAD designs.  
- **Productivity Tools**: Requirements or architecture summaries often exported to Word/PowerPoint for reviews.

## Contributing

- Follow the numbering scheme (e.g., `3.1-SharedArchitecture`) when adding new MBSE model types.  
- Maintain the JSON structure in `*_Loading_Input_Data.json` and `*_Extraction_Output_Data.json` for each subfolder.  
- See [CONTRIBUTING.md](../../docs/CONTRIBUTING.md) for more details.
