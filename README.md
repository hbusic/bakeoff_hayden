bakeoff_hayden
Week 1: Sprint Setup (Fabric focus)

This repo captures the foundational setup for the AI Labs multi-cloud bakeoff project.
Each cloud platform is documented in its own subfolder, with supporting governance and screenshots in docs/.

✅ Completed (Week 1 – Azure Fabric)
Created workspace: bakeoff_hayden
Created lakehouse: bakeoff_hayden
Ingested Sales CSVs → Bronze table (bronze_sales, 596 rows, 9 columns)
Uploaded HR PDFs → /Files/raw/pdf/hr-docs/
Validated ingestion with SQL:
SELECT TOP 10 * FROM bronze_sales;
Documented RBAC roles (design-only; shared workspace) → see governance/rbac-matrix.md
📸 See screenshots & step-by-step guide → docs/10-azure-fabric-setup.md

Repo Structure
fabric/ → Azure Fabric setup (workspace, lakehouse, dataflows, validation)
databricks/ → Databricks setup (coming soon)
watsonx/ → IBM watsonx setup (coming soon)
governance/ → RBAC matrix & access design
docs/ → Documentation & screenshots
