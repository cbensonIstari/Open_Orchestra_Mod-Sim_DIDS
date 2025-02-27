# Open Orchestra Modeling and Simulation Data Item Description Repository

Welcome to the **Open Orchestra** repository for **Modeling and Simulation Data Item Descriptions (DiDs)**! This repo organizes **model definitions**, **model schemas**, and **Digital Engineering Ecosystems (DEEs)** for our organization, especially focusing on **DoD aircraft design** and beyond.

---

## Hierarchy: Model Classes → Model Types → Model Instances

1. **Model Classes**  
   - The broad **families** (or “sections”) of models that capture high-level domains (e.g., **PhysicalSystemRepresentation**, **Simulations**, **MBSE**, **ComputerScienceSoftwareEngineering**, **ProductivityAndDigitalEngineering**).

2. **Model Types**  
   - Subcategories within each Model Class. For instance:
     - **CAD**, **ECAD**, **PLM** (under PhysicalSystemRepresentation),
     - **CFD**, **FEA**, **EM**, **Dynamic**, **MissionModels**, **SimulationManagers** (under Simulations),
     - **RequirementsTools**, **ArchitectureTools**, **SharedArchitecture** (under MBSE), etc.

3. **Model Instances**  
   - Concrete, vendor-specific model definitions, such as **CAD_CreoParametric.json** or **CFD_OpenFOAM.json**. Each instance includes version, licensing, deployment, and InfoSec details.

This layered approach ensures **consistency**, **discoverability**, and **traceability** across multiple domains and classification levels.

---

## The Orchestra Analogy

Think of these **Model Classes** and **Types** as **instrument sections** and **families** in an **orchestra**:

- **Model Classes** = **Sections** (strings, brass, woodwinds…)  
- **Model Types** = **Families of instruments** (violins, violas, cellos under strings…)  
- **Model Instances** = **Individual instruments** (a specific Stradivarius violin #123)

Our **Data Item Descriptions (DiDs)** and **schema** files serve as the **“sheet music”**, providing a vendor-neutral notation so each “instrument” (model) can **harmonize** within the larger Digital Engineering ecosystem.

---

## Repository Layout

1. **docs/**  
   - Contains usage instructions (`USAGE.md`) and contribution guidelines (`CONTRIBUTING.md`).

2. **schema/**  
   - Holds classification files (e.g., `families_and_types.json`) defining official Model Classes and Types.

3. **ecosystems/**  
   - Defines **Digital Engineering Ecosystems (DEE)** in JSON form, specifying which **Model Instances** come together for particular program phases (e.g., `DEE_Simple.json`, `DEE_Comprehensive.json`).

4. **model-classes/**  
   - Main structure organized by **Model Classes** (level 1).  
   - Within each class folder, subfolders for **Model Types** (level 2).  
   - Each **Model Type** contains:
     - A `README.md` describing that domain,
     - An `instances/` folder holding JSON definitions for **Model Instances** (level 3),
     - Two schema files describing **input** (`*_Loading_Input_Data.json`) and **output** (`*_Extraction_Output_Data.json`) for that domain.

---
## Getting Started

1. **Clone** this repository:
   ```bash
   git clone https://github.com/YourOrg/digital-eng-tools.git

2.  **Review** the relevant model-classes/ folder to see tool definitions for your domain (e.g., CAD, PLM, Requirements).

3.  **Check** ecosystems/ to understand how multiple tools combine to form a Digital Engineering environment.

4.  **Refer** to [docs/USAGE.md](docs/USAGE.md) for in-depth instructions, and [docs/CONTRIBUTING.md](docs/CONTRIBUTING.md) if you plan to submit changes.
