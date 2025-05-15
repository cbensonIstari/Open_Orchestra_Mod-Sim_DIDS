# 2.6 Mission Models

This directory hosts **mission-level** or **operational scenario** modeling tools within the **Simulations** class. These models often integrate **multiple assets** (air, ground, sea, space) in a **scenario** to evaluate **mission effectiveness**, **CONOPS**, or **system-of-systems** interactions.

---

## Structure

1. **`2.6.1-instances/`**  
   - JSON definitions for each mission-level modeling tool, including:
     - **AFSIM (Air Force Simulation)**,
     - **STK (Systems Toolkit)**,
     - **ExtendSim**,
     - **AnyLogic**,
     - **OneSAF**.

2. **`2.6.2-MissionModels_Loading_Input_Data.json`**  
   - Defines **input** data typically needed to run mission-level analyses (scenarios, environment, entity definitions, timelines).

3. **`2.6.3-MissionModels_Extraction_Output_Data.json`**  
   - Describes **output** data from these simulations (scenario success rates, timelines, kills/losses, resource usage, etc.).

4. **`2.6.4-MissionModels_Extraction_Output.owl`** *(optional)*  
   - Semantic representation of mission assets, engagements, events, or behaviors if you need advanced queries or cross-domain synergy.

---

## Mission Tools Overview

In **`2.6.1-instances/`**, we include five JSON instance files:

- **AFSIM** (Air Force multi-domain scenario modeling),  
- **STK** (Systems Toolkit for orbits, coverage, comm analysis),  
- **ExtendSim** (Discrete-event simulation for mission flows),  
- **AnyLogic** (Agent-based or discrete-event approach to mission/SoS),  
- **OneSAF** (Synthetic environment for ground-based or combined arms simulation).

---

## How to Use

1. **Loading vs. Extraction**  
   - **`2.6.2-MissionModels_Loading_Input_Data.json`**: scenario setup (terrain, threat definitions, routes, comm networks).  
   - **`2.6.3-MissionModels_Extraction_Output_Data.json`**: mission-level outputs (metrics, timelines, logs, success/fail parameters).

2. **Add/Update Instances**  
   - If your org uses another mission-level tool or an updated version, create or edit a JSON in `2.6.1-instances/`.

3. **Ontology**  
   - `2.6.4-MissionModels_Extraction_Output.owl` can represent mission entities, events, or outcomes in a semantic manner for advanced analysis or system-of-systems synergy.

---

## Relationship to Other Simulation Classes

- **2.1-LowFidelitySimulations**: Quick param or operational trade might feed mission-level scenario data.  
- **2.5-Dynamic**: Robotic or vehicle kinematics could be integrated into a mission scenario.  
- **3-ModelBasedSystemEngineering**: Ties to system architecture or requirements at the mission/SoS layer.

---

## Future Extensions

- HPC-based large-scale engagements, multi-domain campaign analyses.  
- Real-time integration with **3.1-SharedArchitecture** or MBSE for concept-of-operations refining.

---

## Questions or Feedback

- Refer to `[../README.md](../README.md)` for the overall **Simulations** structure.
- Check `[docs/USAGE.md](../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../docs/CONTRIBUTING.md)` to propose new mission model definitions or adapt schemas.

**Shape your mission** success with these scenario-level modeling tools, aligning with the **Open Orchestra** digital engineering environment!
