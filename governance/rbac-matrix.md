| Role     | Workspace Permissions | Lakehouse Tables       | Files            | Dataflows       | Validation Notes                |
|----------|------------------------|------------------------|------------------|-----------------|--------------------------------|
| Admin    | Admin (Workspace)      | Full (Bronze + Silver) | Full             | Full (create/edit) | Me (workspace owner)           |
| Engineer | Member                 | Read/Write Bronze      | Read/Write CSV   | Can create/edit | Not tested (shared workspace)   |
| Analyst  | Viewer                 | Read Silver only       | Read PDFs only   | View only       | Not tested (shared workspace)   |
| Service  | N/A (Service Principal)| Scoped Bronze ingestion| Scoped only      | Jobs only       | Not tested (shared workspace)   |
