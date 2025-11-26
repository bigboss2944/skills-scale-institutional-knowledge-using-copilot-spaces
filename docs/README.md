# OctoAcme Project Management Docs

Welcome — this folder is the central hub for OctoAcme's project management processes. These concise, versioned guides describe how we initiate, plan, execute, release, and improve projects so teams can onboard quickly and work consistently.

## Project Management Process (Overview)
OctoAcme runs projects using a lightweight, repeatable approach that emphasizes:
- Clear roles and responsibilities
- Data-informed, iterative delivery
- Risk-managed execution
- Regular stakeholder communication

High-level lifecycle and what each phase focuses on:
1. Initiation
   - Validate the business problem and define measurable success criteria
   - Identify primary stakeholders and sponsors
   - Produce a Project One-pager as the single source of truth for the decision to plan
2. Planning
   - Break work into shippable increments, estimate effort, and map milestones
   - Identify dependencies, risks, and an initial release plan
   - Create a prioritized backlog with clear acceptance criteria
3. Execution & Tracking
   - Implement work using small, reviewable PRs and CI checks
   - Track progress with the project board and regular team rhythms (standups, delivery syncs)
   - Escalate blockers through defined paths and maintain a risk register
4. Release & Deployment
   - Follow pre-release checks (CI, security scans, release notes) and smoke tests
   - Deploy via automated pipelines where possible and have rollback plans ready
   - Communicate releases to stakeholders and support teams
5. Retrospective & Continuous Improvement
   - Run retros after milestones or incidents, capture action items with owners and due dates
   - Measure impact of improvements and follow up in weekly PM syncs

## Process Documents
- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

## How to use these docs
- Use the Project One-pager and project README in your repo as the single source of truth for a given project.
- Keep each process doc focused and link to any detailed playbooks or runbooks that live elsewhere.
- Add project-specific artifacts into `.copilot/` if you want Copilot Spaces to use them as context in the future.

## Contributing updates
If you want to add or update content, please use the issue template: `.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml` and open a PR that references the issue for review.

---
Last updated: See the repo history for commit metadata.
