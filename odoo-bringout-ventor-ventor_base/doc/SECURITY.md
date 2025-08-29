# Security

Access control and security definitions in ventor_base.

## Access Control Lists (ACLs)

Model access permissions defined in:
- **[ir.model.access.csv](../ventor_base/security/ir.model.access.csv)**
  - 5 model access rules

## Record Rules

Row-level security rules defined in:

## Security Groups & Configuration

Security groups and permissions defined in:
- **[groups.xml](../ventor_base/security/groups.xml)**
  - 32 security groups defined

```mermaid
graph TB
    subgraph "Security Layers"
        A[Users] --> B[Groups]
        B --> C[Access Control Lists]
        C --> D[Models]
        B --> E[Record Rules]
        E --> F[Individual Records]
    end
```

Security files overview:
- **[groups.xml](../ventor_base/security/groups.xml)**
  - Security groups, categories, and XML-based rules
- **[ir.model.access.csv](../ventor_base/security/ir.model.access.csv)**
  - Model access permissions (CRUD rights)

Notes
- Access Control Lists define which groups can access which models
- Record Rules provide row-level security (filter records by user/group)
- Security groups organize users and define permission sets
- All security is enforced at the ORM level by Odoo
