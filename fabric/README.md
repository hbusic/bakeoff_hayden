# Azure Fabric Setup — Week 1 & Week 2

## Week 1 — Foundations & Setup

> **Note (RBAC):**  
> Workspace-level permissions (Admin, Member, Contributor, Viewer) could not be edited in this shared environment, so they are documented only.  
> Lakehouse-level RBAC roles (Admin, Engineer, Analyst, Service) were created and assigned.  
> See [../governance/rbac-matrix.md](../governance/rbac-matrix.md) for details.

### Workspace & Lakehouse
- Workspace: `bakeoff_hayden`
- Lakehouse: `bakeoff_hayden`

### Tables
- bronze_sales → 596 rows, 9 columns

### Files
- HR PDFs stored under: `/Files/raw/pdf/hr-docs/`

### Validation
Validated ingestion using the Lakehouse SQL endpoint:

```sql
SELECT TOP 10 * FROM bronze_sales;

Status

✅ Week 1 Fabric setup complete:

Workspace + Lakehouse created  
Bronze Sales table ingested and validated  
HR PDFs uploaded  
RBAC roles documented (workspace) and enforced (Lakehouse)  

---

Week 2 — Data & Governance

Governance Tasks Completed

- Verified Bronze Sales table exists in Lakehouse (596 rows, 9 columns).  
- Verified HR PDFs uploaded into /Files/raw/pdf/hr-docs/.  
- Confirmed Bronze Sales visible in OneLake Catalog.  
- Added description metadata to the Lakehouse.  
- Opened Govern tab in OneLake Catalog and reviewed automatically generated governance insights.  
- Captured screenshots of Bronze Sales, HR PDFs, Lakehouse description, Catalog view, and Govern report.  

Limitations (Documented)

- Run scans to auto-discover tables → ❌ Not available in OneLake (Purview-only).  
- Assign glossary terms → ❌ Not available without Purview.  
- Apply sensitivity labels → ❌ Not enabled (requires MIP + admin).  
- Endorsement (Promoted, Certified, Master Data) → ❌ Disabled (requires admin).  
- Tags → ❌ Not enabled (requires tenant/domain setup).  

➡ In practice: governance simulated using descriptions, catalog visibility, and Govern tab insights. Full Purview/MIP integration not available in this shared tenant.  

Status

✅ Week 2 Fabric governance complete:

- Data ingestion verified (Bronze Sales + HR PDFs)  
- Catalog visibility confirmed  
- Metadata description added  
- Govern tab insights reviewed  
- Limitations documented clearly  
