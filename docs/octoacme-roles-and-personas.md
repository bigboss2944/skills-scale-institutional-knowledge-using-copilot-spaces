# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

---

## Release / Platform Engineer

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

---

## Site Reliability / Observability Engineer

### Role Summary
SRE / Observability Engineers ensure system reliability, performance, and visibility. They define SLOs, implement monitoring and alerting, and lead incident response.

### Responsibilities
- Define and track Service Level Objectives (SLOs) and error budgets
- Design and implement monitoring, logging, and alerting systems
- Build dashboards for system health and business metrics
- Lead incident response and post-incident reviews
- Create and maintain runbooks for common operational scenarios
- Identify reliability risks and drive mitigation efforts

### Goals
- Maintain system uptime and performance within SLO targets
- Reduce mean time to detection (MTTD) and resolution (MTTR)
- Ensure observability across all critical system components
- Foster a culture of reliability and proactive monitoring

### Typical Communication
- Incident reports and post-mortems
- SLO reviews and reliability metrics
- On-call handoffs and runbook updates
- Collaboration in architecture and design reviews

### How they interact with existing roles
- **PM**: Reports on system reliability and helps prioritize reliability work
- **PdM**: Provides data on user-facing performance and availability
- **Developers**: Collaborates on instrumentation, logging, and performance optimization
- **QA**: Shares insights from production monitoring to inform test strategies
- **Stakeholders**: Communicates system health and incident impact

---

## Security / Compliance Lead

### Role Summary
Security / Compliance Leads ensure products meet security standards and regulatory requirements. They conduct threat modeling, security reviews, and oversee compliance processes.

### Responsibilities
- Conduct threat modeling and security design reviews
- Coordinate security scans (SAST, DAST, dependency checks)
- Ensure compliance with regulatory standards (SOC2, GDPR, etc.)
- Review and approve security-sensitive changes
- Manage vulnerability response and remediation tracking
- Provide security training and awareness to teams

### Goals
- Prevent security vulnerabilities from reaching production
- Maintain compliance certifications and audit readiness
- Minimize time to remediate identified vulnerabilities
- Foster security-aware engineering practices

### Typical Communication
- Security review requests and findings
- Compliance status reports and audit preparations
- Vulnerability disclosures and remediation plans
- Security advisories and best practices

### How they interact with existing roles
- **PM**: Advises on security timeline impacts and compliance milestones
- **PdM**: Ensures security and privacy considerations are in product requirements
- **Developers**: Reviews code for security issues and provides remediation guidance
- **QA**: Collaborates on security testing and penetration testing efforts
- **Stakeholders**: Provides compliance status and security posture updates

---

## UX Researcher / Product Designer

### Role Summary
UX Researchers and Product Designers advocate for user needs, design intuitive experiences, and validate solutions through research and testing.

### Responsibilities
- Conduct user research to understand needs, pain points, and behaviors
- Create wireframes, prototypes, and high-fidelity designs
- Define interaction patterns and user flows
- Collaborate with Product and Engineering on feasibility and trade-offs
- Conduct usability testing and iterate based on feedback
- Maintain design systems and UI component libraries

### Goals
- Deliver intuitive, accessible, and delightful user experiences
- Validate solutions with real users before implementation
- Maintain design consistency across the product
- Reduce friction in user journeys and increase engagement

### Typical Communication
- User research findings and personas
- Design mockups and prototypes
- Usability test reports and recommendations
- Design critiques and stakeholder demos

### How they interact with existing roles
- **PM**: Aligns project timelines with design and research activities
- **PdM**: Collaborates on problem definition and validates solutions with users
- **Developers**: Partners on implementation feasibility and design handoff
- **QA**: Ensures acceptance criteria include design specifications
- **Stakeholders**: Presents design concepts and gathers feedback

---

## Data Analyst / Insights Lead

### Role Summary
Data Analysts / Insights Leads collect, analyze, and interpret product and business data to inform decision-making and measure success.

### Responsibilities
- Define analytics requirements and instrumentation plans
- Build and maintain dashboards for product and business metrics
- Analyze user behavior, feature adoption, and funnel metrics
- Conduct A/B tests and experiments to validate hypotheses
- Generate insights and recommendations for product improvements
- Ensure data quality and governance standards

### Goals
- Enable data-driven decision-making across the organization
- Measure product success and identify improvement opportunities
- Reduce time to insight for product and business questions
- Maintain accurate, trustworthy data pipelines

### Typical Communication
- Analytics requirements and event schemas
- Dashboard and report sharing
- Experiment results and insights presentations
- Data quality issues and remediation plans

### How they interact with existing roles
- **PM**: Provides metrics for project success tracking and reporting
- **PdM**: Partners on defining success metrics and analyzing feature performance
- **Developers**: Collaborates on analytics instrumentation implementation
- **QA**: Validates that analytics events are firing correctly in test environments
- **Stakeholders**: Delivers insights and business intelligence reports

---

## Accessibility Champion

### Role Summary
Accessibility Champions ensure products are usable by people with disabilities, meeting WCAG standards and fostering inclusive design practices.

### Responsibilities
- Review designs and implementations for accessibility compliance
- Conduct accessibility audits using automated tools and manual testing
- Provide guidance on ARIA labels, keyboard navigation, and screen readers
- Advocate for accessibility in product requirements and acceptance criteria
- Train teams on accessibility best practices and standards
- Track and remediate accessibility issues

### Goals
- Ensure products meet WCAG 2.1 Level AA standards (or organizational target)
- Prevent accessibility regressions in new features
- Foster a culture of inclusive design across teams
- Reduce accessibility-related support escalations

### Typical Communication
- Accessibility audit reports and remediation plans
- Design and code review feedback on accessibility
- Training sessions and documentation on best practices
- Collaboration with legal and compliance on accessibility requirements

### How they interact with existing roles
- **PM**: Ensures accessibility is included in project timelines and acceptance criteria
- **PdM**: Advocates for accessibility in product requirements and user stories
- **Developers**: Reviews code for accessibility compliance and provides guidance
- **QA**: Collaborates on accessibility testing strategies and tools
- **Stakeholders**: Reports on accessibility compliance and remediation progress

---

## Customer Success / Support Lead

### Role Summary
Customer Success / Support Leads own the post-sale customer experience, providing assistance, gathering feedback, and advocating for customer needs.

### Responsibilities
- Respond to customer inquiries and resolve support tickets
- Maintain support documentation, FAQs, and knowledge base articles
- Escalate and triage critical issues to engineering teams
- Track support metrics (response time, resolution time, satisfaction)
- Gather customer feedback and feature requests for product teams
- Conduct customer training and onboarding sessions

### Goals
- Maintain high customer satisfaction and retention rates
- Reduce time to resolution for support tickets
- Prevent recurring issues through proactive documentation and training
- Serve as the voice of the customer in product discussions

### Typical Communication
- Support ticket updates and resolutions
- Customer feedback summaries and feature requests
- Escalation notifications for critical issues
- Support runbooks and knowledge base updates

### How they interact with existing roles
- **PM**: Coordinates release communications and support readiness for launches
- **PdM**: Shares customer feedback and pain points to inform roadmap priorities
- **Developers**: Escalates bugs and provides context for customer-reported issues
- **QA**: Collaborates on reproducing customer-reported issues
- **Stakeholders**: Reports on customer health metrics and satisfaction trends

---

## Change Manager / Communications Owner

### Role Summary
Change Managers / Communications Owners plan and execute change management strategies, ensuring smooth adoption of new features and organizational changes.

### Responsibilities
- Develop change management and communication plans for releases
- Identify impacted stakeholders and tailor messaging accordingly
- Create training materials, user guides, and announcement content
- Coordinate cross-team communications during launches and incidents
- Measure adoption and gather feedback on changes
- Manage resistance and facilitate smooth transitions

### Goals
- Maximize adoption and minimize disruption during changes
- Ensure clear, timely communication to all stakeholders
- Reduce support volume through proactive education
- Build stakeholder confidence and trust in the change process

### Typical Communication
- Release announcements and stakeholder briefings
- Training session invitations and materials
- Change impact assessments and readiness reports
- Post-launch adoption and feedback summaries

### How they interact with existing roles
- **PM**: Aligns change management activities with project timelines and milestones
- **PdM**: Ensures messaging reflects product value and user benefits
- **Developers**: Gathers technical details to inform user-facing communications
- **QA**: Coordinates on known issues and workarounds to include in announcements
- **Stakeholders**: Serves as the primary communication liaison for organizational updates

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

