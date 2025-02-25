digital-eng-tools/
├── README.md
├── .gitignore
├── docs/
│   ├── USAGE.md
│   └── CONTRIBUTING.md
├── schema/
│   └── families_and_types.json
├── ecosystems/
│   ├── DEE_Simple.json
│   ├── DEE_Moderate.json
│   └── DEE_Comprehensive.json
└── model-classes/
    ├── 1-PhysicalSystemRepresentation/
    │   ├── README.md
    │   ├── 1.1-CAD/
    │   │   ├── README.md
    │   │   ├── 1.1.1-instances/
    │   │   │   ├── 1.1.1.1-CAD_CreoParametric.json
    │   │   │   ├── 1.1.1.2-CAD_SiemensNX.json
    │   │   │   ├── 1.1.1.3-CAD_CATIA.json
    │   │   │   └── 1.1.1.4-CAD_FreeCAD.json
    │   │   ├── 1.1.2-CAD_Loading_Input_Data.json
    │   │   └── 1.1.3-CAD_Extraction_Output_Data.json
    │   ├── 1.2-ECAD/
    │   │   ├── README.md
    │   │   ├── 1.2.1-instances/
    │   │   │   ├── 1.2.1.1-ECAD_AltiumDesigner.json
    │   │   │   ├── 1.2.1.2-ECAD_OrCAD.json
    │   │   │   └── 1.2.1.3-ECAD_KiCad.json
    │   │   ├── 1.2.2-ECAD_Loading_Input_Data.json
    │   │   └── 1.2.3-ECAD_Extraction_Output_Data.json
    │   └── 1.3-PLM/
    │       ├── README.md
    │       ├── 1.3.1-instances/
    │       │   ├── 1.3.1.1-PLM_Teamcenter.json
    │       │   ├── 1.3.1.2-PLM_Windchill.json
    │       │   └── 1.3.1.3-PLM_OpenPLM.json
    │       ├── 1.3.2-PLM_Models_Loading_Input_Data.json
    │       └── 1.3.3-PLM_Models_Extraction_Output_Data.json
    ├── 2-Simulations/
    │   ├── README.md
    │   ├── 2.1-LowFidelitySimulations/
    │   │   ├── README.md
    │   │   ├── 2.1.1-instances/
    │   │   │   ├── 2.1.1.1-LowFidelity_OpenVSP.json
    │   │   │   ├── 2.1.1.2-LowFidelity_InHouseTool.json
    │   │   │   └── 2.1.1.3-LowFidelity_ExcelTradeStudy.json
    │   │   ├── 2.1.2-LowFidelitySim_Loading_Input_Data.json
    │   │   └── 2.1.3-LowFidelitySim_Extraction_Output_Data.json
    │   ├── 2.2-CFD/
    │   │   ├── README.md
    │   │   ├── 2.2.1-instances/
    │   │   │   ├── 2.2.1.1-CFD_ANSYSFluent.json
    │   │   │   ├── 2.2.1.2-CFD_StarCCMplus.json
    │   │   │   └── 2.2.1.3-CFD_OpenFOAM.json
    │   │   ├── 2.2.2-CFD_Loading_Input_Data.json
    │   │   └── 2.2.3-CFD_Extraction_Output_Data.json
    │   ├── 2.3-FEA/
    │   │   ├── README.md
    │   │   ├── 2.3.1-instances/
    │   │   │   ├── 2.3.1.1-FEA_MSCNastran.json
    │   │   │   ├── 2.3.1.2-FEA_Abaqus.json
    │   │   │   └── 2.3.1.3-FEA_Calculix.json
    │   │   ├── 2.3.2-FEA_Loading_Input_Data.json
    │   │   └── 2.3.3-FEA_Extraction_Output_Data.json
    │   ├── 2.4-EM/
    │   │   ├── README.md
    │   │   ├── 2.4.1-instances/
    │   │   │   ├── 2.4.1.1-EM_CSTStudioSuite.json
    │   │   │   ├── 2.4.1.2-EM_AnsysHFSS.json
    │   │   │   └── 2.4.1.3-EM_OpenEMS.json
    │   │   ├── 2.4.2-EM_Loading_Input_Data.json
    │   │   └── 2.4.3-EM_Extraction_Output_Data.json
    │   ├── 2.5-Dynamic/
    │   │   ├── README.md
    │   │   ├── 2.5.1-instances/
    │   │   │   ├── 2.5.1.1-Dynamic_MSCADAMS.json
    │   │   │   ├── 2.5.1.2-Dynamic_Simscape.json
    │   │   │   └── 2.5.1.3-Dynamic_MBDyn.json
    │   │   ├── 2.5.2-Dynamic_Loading_Input_Data.json
    │   │   └── 2.5.3-Dynamic_Extraction_Output_Data.json
    │   ├── 2.6-MissionModels/
    │   │   ├── README.md
    │   │   ├── 2.6.1-instances/
    │   │   │   ├── 2.6.1.1-MissionModels_AFSIM.json
    │   │   │   ├── 2.6.1.2-MissionModels_STK.json
    │   │   │   └── 2.6.1.3-MissionModels_OpenMission.json
    │   │   ├── 2.6.2-MissionModels_Loading_Input_Data.json
    │   │   └── 2.6.3-MissionModels_Extraction_Output_Data.json
    │   └── 2.7-SimulationManagers/
    │       ├── README.md
    │       ├── 2.7.1-instances/
    │       │   ├── 2.7.1.1-SimulationManagers_PhoenixModelCenter.json
    │       │   ├── 2.7.1.2-SimulationManagers_AnsysWorkbench.json
    │       │   └── 2.7.1.3-SimulationManagers_OpenMDAO.json
    │       ├── 2.7.2-SimulationManagers_Loading_Input_Data.json
    │       └── 2.7.3-SimulationManagers_Extraction_Output_Data.json
    ├── 3-ModelBasedSystemEngineering/
    │   ├── README.md
    │   ├── 3.1-SharedArchitecture/
    │   │   ├── README.md
    │   │   ├── 3.1.1-instances/
    │   │   │   ├── 3.1.1.1-SharedArchitecture_TeamworkCloud.json
    │   │   │   ├── 3.1.1.2-SharedArchitecture_IBMModelManager.json
    │   │   │   └── 3.1.1.3-SharedArchitecture_Papyrus.json
    │   │   ├── 3.1.2-Shared_Architecture_Models_Loading_Input_Data.json
    │   │   └── 3.1.3-Shared_Architecture_Models_Extraction_Output_Data.json
    │   ├── 3.2-ArchitectureTools/
    │   │   ├── README.md
    │   │   ├── 3.2.1-instances/
    │   │   │   ├── 3.2.1.1-ArchitectureTools_CameoSystemsModeler.json
    │   │   │   ├── 3.2.1.2-ArchitectureTools_Rhapsody.json
    │   │   │   └── 3.2.1.3-ArchitectureTools_Modelio.json
    │   │   ├── 3.2.2-Architecture_Models_Loading_Input_Data.json
    │   │   └── 3.2.3-Architecture_Models_Extraction_Output_Data.json
    │   └── 3.3-RequirementsTools/
    │       ├── README.md
    │       ├── 3.3.1-instances/
    │       │   ├── 3.3.1.1-RequirementsTools_DoorsNext.json
    │       │   ├── 3.3.1.2-RequirementsTools_Jama.json
    │       │   └── 3.3.1.3-RequirementsTools_OpenReq.json
    │       ├── 3.3.2-Requirements_Models_Loading_Input_Data.json
    │       └── 3.3.3-Requirements_Models_Extraction_Output_Data.json
    ├── 4-ComputerScienceSoftwareEngineering/
    │   ├── README.md
    │   ├── 4.1-IDE/
    │   │   ├── README.md
    │   │   ├── 4.1.1-instances/
    │   │   │   ├── 4.1.1.1-IDE_VisualStudio.json
    │   │   │   ├── 4.1.1.2-IDE_MATLABSimulink.json
    │   │   │   ├── 4.1.1.3-IDE_Eclipse.json
    │   │   │   └── 4.1.1.4-IDE_Xcode.json            # <-- ADDED
    │   │   ├── 4.1.2-IDE_Loading_Input_Data.json
    │   │   └── 4.1.3-IDE_Extraction_Output_Data.json
    │   ├── 4.2-VersionControl/
    │   │   ├── README.md
    │   │   ├── 4.2.1-instances/
    │   │   │   ├── 4.2.1.1-VersionControl_GitLabEnterprise.json
    │   │   │   ├── 4.2.1.2-VersionControl_BitbucketServer.json
    │   │   │   └── 4.2.1.3-VersionControl_GitCLI.json
    │   │   ├── 4.2.2-VersionControl_Loading_Input_Data.json
    │   │   └── 4.2.3-VersionControl_Extraction_Output_Data.json
    │   ├── 4.3-CI_CD/                             # <-- RENAME from TestingFrameworks
    │   │   ├── README.md
    │   │   ├── 4.3.1-instances/
    │   │   │   ├── 4.3.1.1-CI_CD_Jenkins.json      # <-- NEW
    │   │   │   ├── 4.3.1.2-CI_CD_GitHubActions.json# <-- NEW
    │   │   │   └── 4.3.1.3-CI_CD_Bamboo.json       # <-- NEW
    │   │   ├── 4.3.2-CI_CD_Loading_Input_Data.json
    │   │   └── 4.3.3-CI_CD_Extraction_Output_Data.json
    │   └── 4.4-AIFoundationModels/                # <-- NEW MODEL TYPE
    │       ├── README.md                          # <-- NEW
    │       ├── 4.4.1-instances/                   # <-- NEW
    │       │   ├── 4.4.1.1-AIFoundation_BERT.json     # <-- NEW
    │       │   ├── 4.4.1.2-AIFoundation_Llama2.json   # <-- NEW
    │       │   └── 4.4.1.3-AIFoundation_SageMaker.json # <-- NEW
    │       ├── 4.4.2-AIFoundationModels_Loading_Input_Data.json
    │       └── 4.4.3-AIFoundationModels_Extraction_Output_Data.json
    └── 5-ProductivityAndDigitalEngineering/
        ├── README.md
        ├── 5.1-Email/
        │   ├── README.md
        │   ├── 5.1.1-instances/
        │   │   ├── 5.1.1.1-Email_Outlook.json
        │   │   ├── 5.1.1.2-Email_Thunderbird.json
        │   │   └── 5.1.1.3-Email_Zimbra.json
        │   ├── 5.1.2-Email_Loading_Input_Data.json
        │   └── 5.1.3-Email_Extraction_Output_Data.json
        ├── 5.2-WordProcessing/
        │   ├── README.md
        │   ├── 5.2.1-instances/
        │   │   ├── 5.2.1.1-WordProcessing_MSWord.json
        │   │   ├── 5.2.1.2-WordProcessing_GoogleDocs.json
        │   │   └── 5.2.1.3-WordProcessing_LibreOfficeWriter.json
        │   ├── 5.2.2-WordProcessing_Loading_Input_Data.json
        │   └── 5.2.3-WordProcessing_Extraction_Output_Data.json
        ├── 5.3-Presentations/
        │   ├── README.md
        │   ├── 5.3.1-instances/
        │   │   ├── 5.3.1.1-Presentations_MSPowerPoint.json
        │   │   ├── 5.3.1.2-Presentations_GoogleSlides.json
        │   │   └── 5.3.1.3-Presentations_LibreOfficeImpress.json
        │   ├── 5.3.2-Presentations_Loading_Input_Data.json
        │   └── 5.3.3-Presentations_Extraction_Output_Data.json
        ├── 5.4-Spreadsheets/
        │   ├── README.md
        │   ├── 5.4.1-instances/
        │   │   ├── 5.4.1.1-Spreadsheets_MSExcel.json
        │   │   ├── 5.4.1.2-Spreadsheets_GoogleSheets.json
        │   │   └── 5.4.1.3-Spreadsheets_LibreOfficeCalc.json
        │   ├── 5.4.2-Spreadsheets_Loading_Input_Data.json
        │   └── 5.4.3-Spreadsheets_Extraction_Output_Data.json
        ├── 5.5-TaskManagement/
        │   ├── README.md
        │   ├── 5.5.1-instances/
        │   │   ├── 5.5.1.1-TaskManagement_Jira.json
        │   │   ├── 5.5.1.2-TaskManagement_Trello.json
        │   │   └── 5.5.1.3-TaskManagement_Taiga.json
        │   ├── 5.5.2-TaskManagement_Loading_Input_Data.json
        │   └── 5.5.3-TaskManagement_Extraction_Output_Data.json
        └── 5.6-SharedDrives/
            ├── README.md
            ├── 5.6.1-instances/
            │   ├── 5.6.1.1-SharedStorage_OneDrive.json
            │   ├── 5.6.1.2-SharedStorage_GoogleDrive.json
            │   └── 5.6.1.3-SharedStorage_Nextcloud.json
            ├── 5.6.2-SharedDrives_Loading_Input_Data.json
            └── 5.6.3-SharedDrives_Extraction_Output_Data.json
