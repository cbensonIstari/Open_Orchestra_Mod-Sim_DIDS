# 2.5 Dynamic (Rigid-Body / Mechanical System Dynamics)

This directory focuses on **mechanical system dynamics** tools in the **Simulations** class, often used to simulate **motion**, **kinematics**, and **multibody** interactions. Typical applications include robotics, vehicle dynamics, and machine mechanisms.

---

## Structure

1. **`2.5.1-instances/`**  
   - JSON files for each dynamic or multibody simulation tool (MSC ADAMS, Simscape Multibody, MBDyn, RecurDyn, Siemens Simcenter Motion, Altair MotionSolve, Chrono, Gazebo, MapleSim, Dymola MultiBody).

2. **`2.5.2-Dynamic_Loading_Input_Data.json`**  
   - Describes **input** data typically needed (geometry, joints, constraints, mass/inertia, force/torque definitions).

3. **`2.5.3-Dynamic_Extraction_Output_Data.json`**  
   - Summarizes **output** data from dynamic simulations (joint reaction forces, motion time histories, animations, etc.).

4. **`2.5.4-Dynamic_Extraction_Output.owl`** *(optional)*  
   - Semantic representation of bodies, joints, constraints, motion results, potentially linking to MBSE or HPC.

---

## Dynamic Tools Overview

In **`2.5.1-instances/`**, you’ll find JSON definitions for:

1. MSC ADAMS  
2. Simscape Multibody (MATLAB/Simulink)  
3. MBDyn (Open Source)  
4. RecurDyn  
5. Siemens Simcenter Motion  
6. Altair MotionSolve  
7. Project Chrono  
8. Gazebo (robotics, open source)  
9. MapleSim  
10. Dymola MultiBody

---

## How to Use

1. **Load vs. Extraction Schemas**  
   - **`2.5.2-Dynamic_Loading_Input_Data.json`**: geometry, joints, constraints, solver parameters.  
   - **`2.5.3-Dynamic_Extraction_Output_Data.json`**: motion time-series, reaction forces, energy consumption, or animation frames.

2. **Add/Update Instances**  
   - If a new dynamic solver is introduced or updated, create or modify a JSON in `2.5.1-instances/`.

3. **Ontology**  
   - `2.5.4-Dynamic_Extraction_Output.owl` can capture relationships among bodies, joints, constraints, and time-based solutions for advanced queries or cross-domain synergy.

---

## Relationship to Other Simulation Classes

- **2.1-LowFidelitySimulations**: Could feed early conceptual data for linkages or approximate inertia.  
- **2.3-FEA** or **2.4-EM**: Might co-sim with structural or electromagnetic solvers for advanced multi-physics.  
- **1.1-CAD**: Geometry for dynamic models often comes from mechanical CAD assemblies.

---

## Future Extensions

- HPC-based multi-body runs with large DOF or param sweeps.  
- Robotics or real-time integration with **2.6-MissionModels** for in-situ dynamics.

---

## Questions or Feedback

- Check `[../README.md](../README.md)` for the overall **Simulations** structure.
- See `[docs/USAGE.md](../../docs/USAGE.md)` or `[docs/CONTRIBUTING.md](../../docs/CONTRIBUTING.md)` for how to add or modify instance files or schemas.

**Simulate mechanical motion** effectively with these dynamic tools, uniting them under the **Open Orchestra** digital engineering umbrella!
