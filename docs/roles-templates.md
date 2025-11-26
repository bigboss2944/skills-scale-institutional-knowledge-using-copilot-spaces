# Role and Persona Template

## Purpose
This template provides a consistent format for defining new roles and personas in OctoAcme project documentation. Use this when expanding the team structure or documenting new specialized roles.

## Standard Template

```markdown
## [Role Name]

### Role Summary
[One to two sentences describing what this role does and their primary focus area.]

### Responsibilities
- [Key responsibility 1]
- [Key responsibility 2]
- [Key responsibility 3]
- [Key responsibility 4]
- [Additional responsibilities as needed]

### Goals
- [Primary goal 1]
- [Primary goal 2]
- [Primary goal 3]
- [Additional goals as needed]

### Typical Communication
- [Communication type 1 and frequency]
- [Communication type 2 and frequency]
- [Communication type 3 and frequency]
- [Additional communication channels as needed]

### How they interact with existing roles
- **PM**: [Describe interaction with Project Manager]
- **PdM**: [Describe interaction with Product Manager]
- **Developers**: [Describe interaction with Development team]
- **QA**: [Describe interaction with QA/Testing]
- **Stakeholders**: [Describe interaction with Stakeholders]
```

## RACI Template for Common Activities

When defining a new role, consider documenting their involvement in common activities using RACI notation:
- **R**esponsible: Does the work
- **A**ccountable: Ultimately answerable for completion
- **C**onsulted: Provides input
- **I**nformed: Kept updated

| Activity | PM | PdM | Dev | QA | [New Role] | Notes |
|----------|----|----|-----|----|-----------|----|
| Feature Planning | A | R | C | C | C | [New role's involvement] |
| Release Approval | I | C | I | C | R | [New role's involvement] |
| Incident Response | C | I | C | I | R | [New role's involvement] |

## Example: Release / Platform Engineer

### Role Summary
Release / Platform Engineers own the CI/CD pipeline, deployment automation, and release orchestration. They ensure reliable, repeatable releases with minimal manual intervention.

### Responsibilities
- Design and maintain CI/CD pipelines and deployment automation
- Coordinate release schedules and deployment windows
- Implement deployment strategies (blue-green, canary, feature flags)
- Maintain build and deployment tooling and infrastructure
- Monitor deployment health and assist with rollbacks
- Document deployment procedures and runbooks

### Goals
- Minimize deployment risk and downtime
- Reduce manual effort in the release process
- Ensure fast, safe rollback capabilities
- Maintain audit trails for all deployments

### Typical Communication
- Release schedules and deployment notifications
- Post-mortems for failed deployments
- CI/CD pipeline updates and maintenance windows
- Coordination with DevOps and infrastructure teams

### How they interact with existing roles
- **PM**: Coordinates release schedules and communicates deployment windows
- **PdM**: Aligns feature releases with product roadmap milestones
- **Developers**: Provides CI/CD support and reviews deployment configurations
- **QA**: Collaborates on smoke tests and staging environment validation
- **Stakeholders**: Provides release status updates and deployment reports

### RACI for Release / Platform Engineer

| Activity | PM | PdM | Dev | QA | Release Engineer | Notes |
|----------|----|----|-----|----|-----------------|----|
| CI/CD Pipeline Design | C | I | C | C | R/A | Release Engineer owns pipeline |
| Release Scheduling | A | C | C | C | R | PM accountable, Release Engineer executes |
| Deployment Execution | I | I | C | C | R/A | Release Engineer responsible |
| Rollback Decisions | A | C | C | C | R | PM approves, Release Engineer executes |
| Production Monitoring | I | I | C | I | R | Shared with SRE |

## How to use this template
1. Copy the standard template above
2. Fill in all sections with role-specific details
3. Consider the RACI matrix to clarify responsibilities
4. Review with stakeholders to ensure accuracy
5. Add to octoacme-roles-and-personas.md
