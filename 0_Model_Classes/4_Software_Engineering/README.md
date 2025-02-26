# 4. Computer Science and Software Engineering

This folder encompasses tools and model types **dedicated to software** design, development, version control, and continuous integration/delivery, as well as emerging **AI foundation models**.

## Subfolders

1. **4.1-IDE/** (Integrated Development Environments)  
   - Tools like Visual Studio, MATLAB/Simulink, Eclipse, Xcode for writing and debugging code.
2. **4.2-VersionControl/**  
   - Systems managing source code revisions (GitLab Enterprise, Bitbucket, Git CLI).
3. **4.3-CI_CD/**  
   - Continuous Integration / Continuous Delivery pipelines (Jenkins, GitHub Actions, Bamboo).
4. **4.4-AIFoundationModels/**  
   - Large Language Models or advanced AI engines (BERT, Llama2, SageMaker JumpStart, etc.).

Each subfolder contains:
- A `README.md` explaining that domain,
- An `instances/` subfolder with tool JSON files (e.g., `VersionControl_GitLabEnterprise.json`),
- Two JSON schema files specifying input/output for each domain.

## Why Separate?

- **Software Lifecycle**: IDEs, version control, and CI/CD are crucial for software-based systems, typical in DoD aircraft (avionics, flight software, ground support).
- **AI Foundation Models**: A new domain, requiring specialized workflows for data ingestion, model updates, and ethical usage in engineering contexts.

## Integration with Other Classes

- **MBSE**: Some advanced development integrates SysML auto-coding or requirements management with code repos.  
- **Simulations**: HPC or cloud-based solutions for large-scale simulation are often orchestrated by CI/CD pipelines.  
- **Productivity**: Documentation or data from software systems can feed spreadsheets or Word-based artifacts.

## Contributing

- Use the existing numeric structure (e.g., `4.1-IDE/`) for new subfolders.  
- Check `[docs/CONTRIBUTING.md](../../docs/CONTRIBUTING.md)` for guidelines on adding or editing tool instance JSON files.  
- Adhere to input/output schema patterns for each domain to maintain consistency across the repo.
