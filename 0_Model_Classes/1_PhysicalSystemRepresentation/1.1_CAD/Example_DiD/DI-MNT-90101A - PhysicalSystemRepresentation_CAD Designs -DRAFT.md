**DATA ITEM DESCRIPTION** 

**Title:** PHYSICAL SYSTEM REPRESENTATION / CAD DESIGNS 

**Number:** DI-MNT-90101A			**Approval Date:** TBD		 **AMSC Number:** 10057 			**Limitation**:    
**DTIC Applicable:** No 			**GIDEP Applicable**: No   
**Preparing Activity:** MI 			**Project Number**: TBD   
**Applicable Forms**:  

**Use/relationship:** A Physical System Representation – CAD Data Item Description (DID) defines the authoritative digital engineering description of a system’s CAD models, ensuring they are clear, complete, and accurate. This DID supports design, simulation, manufacturing, verification, and lifecycle management of CAD-based systems. It consists of relevant engineering data such as 3D models, associated metadata, input/output definitions, and applicable standards.

This DID establishes the minimum required content, format, and interoperability for CAD-based digital engineering workflows within DoD and defense industry applications.

**Requirements**:  

1\. Reference Documents

The applicable issue of the documents cited herein, including their approval dates and any applicable amendments, shall be specified in the contract.

2\. Format

* All CAD model data shall conform to ISO, ANSI, and MIL-STD specifications as applicable. Deliverable formats include:  
* Native CAD formats: (e.g., .prt, .asm, .sldprt, .catpart, .x\_t)  
* Neutral exchange formats: (e.g., .step (ISO 10303), .iges, .stl, .dwg, .dxf)  
* Metadata and configuration files: (e.g., .xml material definitions, simulation boundary conditions)

3\. Content

A CAD-based Technical Data Package (TDP) shall include one or more of the following elements:

a. CAD Model Data (per MIL-STD-31000B 5.4.1.x)

* Parametric 3D models and 2D drawings  
* Model hierarchy and assembly structure  
* Associative relationships between parts  
* Surface and solid geometry definitions  
* Reference dimensions, tolerances, and GD\&T per ASME Y14.5  
* Bill of Materials (BOM) per ISO 8000, IPC-2578

b. CAD Loading/Input Data (DI-MNT-90101.01A)

* Metadata: Project name, author, creation date  
* Configuration Files: XML-based setup files  
* Material Definitions: Standardized material properties  
* Imported Neutral Geometry: STEP, IGES, OpenUSD

c. CAD Extraction/Output Data (DI-MNT-90101.02A)

* Mass Properties: Bounding box, volume, center of gravity  
* Material Properties: Extracted metadata  
* BOM and Components List: Exportable structured format  
* Applicable Standards Compliance: ISO, ANSI, MIL-STD

d. CAD Instances

* DI-MNT-90101.10A: Creo Parametric  
* DI-MNT-90101.11A: Siemens NX  
* DI-MNT-90101.12A: CATIA  
* DI-MNT-90101.13A: FreeCAD (Open Source)

**Critical Data Fields**  
The CAD models must include the following critical data fields for engineering validation, digital continuity, and compliance:

* Mass Properties  
  * Bounding Box: Spatial dimensions (e.g., Length: 250mm, Width: 150mm, Height: 75mm)  
  * Density: Material-specific density (e.g., Aluminum 6061-T6: 2.70 g/cm³, Titanium Grade 5: 4.43 g/cm³)  
  * Volume: Computed volume (e.g., 3,500 cm³ for a solid part)  
  * Surface Area: Total external area of the part (e.g., 2,450 mm² for a machined bracket)  
  * Mass: Weight of the object (e.g., 2.5 kg for a steel bracket)  
* Material Properties  
  * Extracted material assignments (e.g., Steel: AISI 4140, Aluminum: 7075-T6, Plastic: PEEK)  
* Bill of Materials (BOM)  
  * Detailed part listings (e.g., Item 1: Wing Rib, Qty: 4, Material: 7075 Aluminum)  
* 3D Rendering  
  * OBJ format for visualization (e.g., .obj file can be imported into rendering tools like Blender)

```
{
  "Extraction_Output_Data": {
    "Proprietary CAD Files": [
      ".prt (Creo Parametric, PTC)",
      ".asm (Creo Assembly, PTC)",
      ".sldprt (SolidWorks part, Dassault Systèmes)",
      ".sldasm (SolidWorks assembly, Dassault Systèmes)",
      ".catpart (CATIA part, Dassault Systèmes)",
      ".catproduct (CATIA assembly, Dassault Systèmes)",
      ".x_t (Parasolid, Siemens NX and Solid Edge)",
      ".ipt (Autodesk Inventor part)",
      ".iam (Autodesk Inventor assembly)"
    ],
    "Neutral Files": [
      ".step (ISO 10303 format for interoperability between CAD software)",
      ".iges (Legacy format for model exchange)",
      ".stl (Stereolithography format for 3D printing)",
      ".dwg (Drawing exchange format for schematics)",
      ".dxf (2D vector format used in CAD/CAM)",
      ".usdz (OpenUSD, Universal Scene Description for AR/VR and digital twins)"
    ],
    "Metadata": [
      "Extracted string-based metadata (e.g., Author: John Doe, Project: Airframe Design V3, Created: 2024-02-19)"
    ],
    "Applicable_Standards": {
      "Geometry_Exchange": [
        "ISO 10303 (STEP, used for CAD model interoperability)",
        "IGES ANSI Y14.26M (Used for CAD model exchange, though being phased out)",
        "OpenUSD (Universal Scene Description, developed by Pixar, for 3D workflows in digital twins and AR/VR)"
      ],
      "CAD_Modeling": [
        "ISO 16792 (Digital product definition data practices)",
        "ASME Y14.41 (3D model annotations & digital product definition)"
      ],
      "Mass_Properties": [
        "ASME Y14.5 (Geometric Dimensioning & Tolerancing)"
      ],
      "Material_Standards": [
        "ASTM E1444 (Nondestructive testing for ferrous materials)",
        "ISO 1043 (Plastics material coding system)",
        "ISO 15608 (Metal classification for manufacturing)"
      ],
      "Bill_of_Materials": [
        "ISO 8000 (Data quality for BOM management)",
        "IPC-2578 (BOM data exchange standard for ECAD/MCAD)"
      ],
      "2D_Drawings": [
        "ASME Y14.1 (Drawing sheet size and format)",
        "ASME Y14.5 (GD&T for part features and tolerances)",
        "ISO 128 (Technical drawing standards for mechanical design)"
      ],
      "3D_Viewing": [
        "ISO 14739-1 (PRC format for 3D PDF visualization)",
        "JT Open (ISO 14306, lightweight 3D model format)",
        "OpenUSD (Pixar’s USD format for 3D model visualization and simulation)"
      ]
    },
    "Critical_Data_Fields": {
      "Mass_Properties": {
        "Bounding_Box": [
          "Spatial dimensions (e.g., Length: 250mm, Width: 150mm, Height: 75mm)"
        ],
        "Density": [
          "Material-specific density (e.g., Aluminum 6061-T6: 2.70 g/cm³, Titanium Grade 5: 4.43 g/cm³)"
        ],
        "Volume": [
          "Computed volume (e.g., 3,500 cm³ for a solid part)"
        ],
        "Surface_Area": [
          "Total external area of the part (e.g., 2,450 mm² for a machined bracket)"
        ],
        "Mass": [
          "Weight of the object (e.g., 2.5 kg for a steel bracket)"
        ]
      },
      "Material_Properties": [
        "Extracted material assignments (e.g., Steel: AISI 4140, Aluminum: 7075-T6, Plastic: PEEK)"
      ],
      "Bill_of_Materials": [
        "Detailed part listings (e.g., Item 1: Wing Rib, Qty: 4, Material: 7075 Aluminum)"
      ],
      "3D_Rendering": [
        "OBJ format for visualization (e.g., `.obj` file can be imported into rendering tools like Blender)",
        "USDZ format (e.g., `.usdz` for Augmented Reality and Digital Twin applications)"
      ]
    }
  }
}

```

End of DI-MNT-90101A.