# 0. Model Classes

This directory contains **all the top-level Model Classes** in our Digital Engineering ecosystem, each serving as a **broad category** of engineering or productivity tools. Under each class, you’ll find **subfolders** for **Model Types** (e.g., CAD, ECAD, PLM, etc.) and their related **tool instances** and **input/output schemas**.

---

## Directory Structure Overview

Within **`0_Model_Classes/`**, you should see **numbered folders** for each major Model Class, for example:

1. `1-PhysicalSystemRepresentation/`  
   - Contains subfolders like **`1.1-CAD/`**, **`1.2-ECAD/`**, **`1.3-PLM/`**  
   - Each of these Model Types has its own **README**, an **instances/** subfolder, and two JSON schema files describing how data is loaded/extracted (e.g., `CAD_Loading_Input_Data.json` and `CAD_Extraction_Output_Data.json`).

2. `2-Simulations/`  
   - Subfolders like **`2.1-LowFidelitySimulations/`**, **`2.2-CFD/`**, **`2.3-FEA/`**, **`2.4-EM/`**, etc.  
   - Each Model Type folder describes how simulations are configured, run, and output results.

3. `3-ModelBasedSystemEngineering/`  
   - Could include **`3.1-SharedArchitecture/`**, **`3.2-ArchitectureTools/`**, **`3.3-RequirementsTools/`**  
   - Model-based tools and SysML-based approaches often reside here.

4. `4-ComputerScienceSoftwareEngineering/`  
   - Might have **`4.1-IDE/`**, **`4.2-VersionControl/`**, **`4.3-CI_CD/`**, **`4.4-AIFoundationModels/`**  
   - Covers software development, version control, continuous integration, and AI foundation models.

5. `5-ProductivityAndDigitalEngineering/`  
   - Typically includes **`5.1-Email/`**, **`5.2-WordProcessing/`**, **`5.3-Presentations/`**, **`5.4-Spreadsheets/`**, **`5.5-TaskManagement/`**, **`5.6-SharedDrives/`**  
   - Tools that support collaboration, communication, and day-to-day productivity.

*(Your repository might have more or fewer classes depending on organizational needs.)*

---

## How to Navigate

1. **Identify Your Model Class**  
   - If you’re looking for CAD/PLM/ECAD tools, go to **`1-PhysicalSystemRepresentation/`**. For advanced simulations, head to **`2-Simulations/`**, and so on.

2. **Open the Appropriate Subfolder**  
   - Each Model Type folder (e.g., **`1.1-CAD/`**) has:
     - A `README.md` explaining the scope of that type.
     - An `instances/` subfolder with JSON files for each tool instance.
     - Two JSON schemas (`*_Loading_Input_Data.json` and `*_Extraction_Output_Data.json`) specifying typical data formats.

3. **Review or Add Tool Instances**  
   - Look in `instances/` to find existing JSON definitions, or create a new one if your organization uses another tool.

---

## Contributing

1. **Branch / Fork**  
   - Follow our [CONTRIBUTING.md](../docs/CONTRIBUTING.md) guidelines before adding or modifying any files.

2. **Maintain Numbering**  
   - Keep the **numeric** folder structure (e.g., **`1.1-CAD/`** for CAD) to ensure a consistent layout.

3. **Follow JSON Schemas**  
   - Each model type folder has **input/output** schemas. Align new tool instance JSON files with these standards for consistency.

---

## Related Directories

- **[schema/](../schema/)**  
  Houses broader classification or JSON schemas that define families, types, or validation rules.

- **[ecosystems/](../ecosystems/)**  
  Contains **Digital Engineering Ecosystem** JSON files (e.g., `DEE_Simple.json`) referencing the tool instances from these Model Classes.

- **[docs/](../docs/)**  
  Where you’ll find the **USAGE.md** and **CONTRIBUTING.md** documentation for deeper repository guidelines.

---

## Questions or Feedback

- If you have questions about adding new Model Classes or modifying existing ones, see **`docs/CONTRIBUTING.md`** or contact the repository maintainers.  
- For domain-specific inquiries (e.g., how to handle advanced simulation data or SysML profiles), reach out to the **domain lead** (e.g., Simulation Lead, MBSE Lead, Productivity Tools SME).

Thank you for contributing to our **Digital Engineering** environment!
