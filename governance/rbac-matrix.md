| Role     | Workspace Permissions     | Lakehouse Tables            | Files                | Dataflows            | Validation Notes                                      |
|----------|---------------------------|-----------------------------|----------------------|----------------------|------------------------------------------------------|
| Admin    | Admin (documented only)   | Full (Bronze)               | Full                 | Full (create/edit)   | Workspace-level documented only; Lakehouse-level role created & assigned (me) |
| Engineer | Member (documented only)  | Read/Write Bronze           | Read/Write CSV files | Can create/edit      | Workspace-level documented only; Lakehouse-level role created & assigned (me) |
| Analyst  | Viewer (documented only)  | Read-only (Bronze)          | Read PDFs only       | View only            | Workspace-level documented only; Lakehouse-level role created & assigned (me) |
| Service  | N/A (Service Principal)   | Design-only (not enforced)  | Design-only          | Jobs only (design)   | Service role designed; not enforced in this workspace |
