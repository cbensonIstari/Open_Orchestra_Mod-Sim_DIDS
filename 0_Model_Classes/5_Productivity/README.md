# 5. Productivity and Digital Engineering

This directory covers **office productivity** and **collaboration** tools that, while not engineering-domain-specific, are essential for daily workflows, document creation, scheduling, communication, and file sharing.

## Subfolders

1. **5.1-Email/**  
   - Tools like Outlook, Thunderbird, Zimbra for messaging and email.
2. **5.2-WordProcessing/**  
   - Tools for creating formal documents, proposals, and reports (Word, Google Docs, LibreOffice Writer).
3. **5.3-Presentations/**  
   - Slide creation and presentation tools (PowerPoint, Google Slides, LibreOffice Impress).
4. **5.4-Spreadsheets/**  
   - Data tracking, quick calculations, cost estimates (Excel, Google Sheets, LibreOffice Calc).
5. **5.5-TaskManagement/**  
   - Organize sprints, tasks, or project milestones (Jira, Trello, Taiga).
6. **5.6-SharedDrives/**  
   - Cloud-based or on-prem file sharing (OneDrive, Google Drive, Nextcloud).

Each subfolder has:
- A `README.md` describing that specific productivity domain,
- An `instances/` directory with tool JSON definitions (e.g., `Email_Outlook.json`),
- Two JSON schema files showing how data is loaded/extracted for each domain.

## Why Include These in DE?

- **Collaboration**: Documents, email, and file sharing are vital for cross-functional teams in DoD aircraft programs.
- **Integration**: Tools like MS Project or Excel may feed schedule/cost data into MBSE or PLM systems.  
- **Simplicity**: Standard office tools remain critical even as advanced engineering tools multiply.

## Interaction with Other Classes

- **Simulations**: Results or data might be exported to spreadsheets for quick analyses or cost breakdowns.
- **MBSE**: Exports model diagrams into presentations or doc deliverables.
- **Physical Representation**: BOM data from PLM might be summarized in Excel or Word for management reviews.

## Contributing

- Maintain numeric structure (e.g., `5.2-WordProcessing/`).  
- Keep the JSON schemas up to date (`*_Loading_Input_Data.json`, `*_Extraction_Output_Data.json`).  
- Check `[docs/CONTRIBUTING.md](../../docs/CONTRIBUTING.md)` for more on naming conventions, references, or pull request guidelines.
