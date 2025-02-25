# Digital Engineering Tools Repository

Welcome to the **Digital Engineering Tools** repository! This repo organizes all tool definitions, model schemas, and Digital Engineering Ecosystems (DEEs) for our organization, focused on **DoD aircraft design** and beyond.

## Structure Overview

1. **`docs/`**  
   - Contains in-depth usage instructions (`USAGE.md`) and contribution guidelines (`CONTRIBUTING.md`).

2. **`schema/`**  
   - Houses JSON schema or classification files (like `families_and_types.json`) that define how we categorize Digital Engineering tools.

3. **`ecosystems/`**  
   - Defines **Digital Engineering Ecosystems (DEE)**, each referencing multiple tool instances for a specific program scope (e.g., `DEE_Simple.json`, `DEE_Moderate.json`, `DEE_Comprehensive.json`).

4. **`model-classes/`**  
   - Organized by **Model Classes** (e.g., PhysicalSystemRepresentation, Simulations, MBSE, etc.), each containing **Model Types** (CAD, ECAD, PLM, etc.).  
   - Every Model Type folder has:
     - A `README.md`
     - A subfolder of `instances/` with JSON files for each tool instance
     - Two JSON files describing the **input** (`*_Loading_Input_Data.json`) and **output** (`*_Extraction_Output_Data.json`) data for that Model Type.

## Getting Started

1. **Clone** this repository:
   ```bash
   git clone https://github.com/YourOrg/digital-eng-tools.git

2.  **Review** the relevant model-classes/ folder to see tool definitions for your domain (e.g., CAD, PLM, Requirements).

3.  **Check** ecosystems/ to understand how multiple tools combine to form a Digital Engineering environment.

4.  **Refer** to [docs/USAGE.md](docs/USAGE.md) for in-depth instructions, and [docs/CONTRIBUTING.md](docs/CONTRIBUTING.md) if you plan to submit changes.
