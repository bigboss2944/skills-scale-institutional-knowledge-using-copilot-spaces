# Cross-Cutting Checklists

## Purpose
These checklists help teams address common cross-cutting concerns that span multiple roles and disciplines. Use these to ensure nothing critical is missed before releases and major milestones.

---

## Release Readiness Checklist

**Owner**: Release / Platform Engineer (with input from all teams)

**When to use**: Before any production deployment

### Pre-Release Gates
- [ ] **CI/CD**: All CI pipelines passing (build, unit tests, integration tests)
- [ ] **Code Quality**: Code reviews completed, linting passed, no critical static analysis warnings
- [ ] **Smoke Tests**: Smoke tests executed successfully on staging environment
- [ ] **Observability**: Monitoring dashboards configured and validated
- [ ] **Observability**: Key metrics and alerts are firing correctly in staging
- [ ] **Observability**: Runbooks updated with new features and troubleshooting steps
- [ ] **Rollback Plan**: Rollback procedure documented and tested
- [ ] **Rollback Plan**: Rollback criteria defined (when to trigger, who approves)
- [ ] **Support Readiness**: Support team trained on new features
- [ ] **Support Readiness**: Customer-facing documentation updated (FAQs, knowledge base)
- [ ] **Support Readiness**: Escalation paths confirmed for potential issues
- [ ] **Communications**: Release notes drafted and reviewed
- [ ] **Communications**: Stakeholders notified of deployment window
- [ ] **Communications**: Change management plan executed (if significant changes)

### Acceptance Criteria
- All pre-release gates passed and documented
- Sign-offs obtained from Release Engineer, QA, SRE, and PM
- Deployment window scheduled and communicated
- On-call team briefed and ready to respond

---

## Security & Compliance Gating Checklist

**Owner**: Security / Compliance Lead

**When to use**: Before merging security-sensitive changes or at release milestones

### Security Review Gates
- [ ] **Threat Modeling**: Threat model completed for new features or architectural changes
- [ ] **Threat Modeling**: Security risks identified and mitigations documented
- [ ] **Code Scanning**: SAST (Static Application Security Testing) scans passed
- [ ] **Code Scanning**: DAST (Dynamic Application Security Testing) completed for web interfaces
- [ ] **Dependency Security**: Dependency vulnerability scans passed (npm audit, Snyk, Dependabot)
- [ ] **Dependency Security**: High/critical vulnerabilities remediated or accepted with risk documentation
- [ ] **Authentication & Authorization**: Access controls reviewed and tested
- [ ] **Authentication & Authorization**: Privilege escalation scenarios validated
- [ ] **Data Protection**: Sensitive data handling reviewed (encryption at rest and in transit)
- [ ] **Data Protection**: PII/PHI compliance verified (GDPR, HIPAA, etc. as applicable)
- [ ] **Security Testing**: Penetration testing completed (if required for release)
- [ ] **Security Testing**: Security acceptance tests passed

### Compliance Gates
- [ ] **Regulatory Compliance**: SOC2/ISO27001 controls validated (if applicable)
- [ ] **Regulatory Compliance**: Audit trail and logging requirements met
- [ ] **Privacy**: Privacy impact assessment completed (if handling user data)
- [ ] **Privacy**: Data retention and deletion policies implemented
- [ ] **Legal Review**: Terms of service and privacy policy updates reviewed (if applicable)

### Acceptance Criteria
- All security scans passed or exceptions documented and approved
- Compliance requirements met and evidence collected
- Security sign-off obtained from Security Lead
- Risk register updated with any accepted risks

---

## Observability & SLO Readiness Checklist

**Owner**: Site Reliability / Observability Engineer

**When to use**: Before launching new services or features with user-facing impact

### Monitoring & Alerting
- [ ] **Metrics**: Key service metrics instrumented (latency, error rate, throughput)
- [ ] **Metrics**: Business metrics instrumented (user actions, conversions, engagement)
- [ ] **Logging**: Structured logging implemented with appropriate log levels
- [ ] **Logging**: Log aggregation configured (e.g., Splunk, ELK, CloudWatch)
- [ ] **Tracing**: Distributed tracing enabled for request flows (if applicable)
- [ ] **Dashboards**: Real-time dashboard created for service health
- [ ] **Dashboards**: Dashboard includes key SLIs (Service Level Indicators)
- [ ] **Alerting**: Alerts configured for critical thresholds (error rate, latency, availability)
- [ ] **Alerting**: Alert routing configured to on-call team
- [ ] **Alerting**: Alert runbooks created for common scenarios

### SLO Definition
- [ ] **SLIs Defined**: Service Level Indicators identified (e.g., 99th percentile latency, error rate)
- [ ] **SLOs Set**: Service Level Objectives defined with target thresholds
- [ ] **SLOs Set**: Error budget calculated and tracking mechanism in place
- [ ] **SLAs**: Service Level Agreements documented (if customer-facing)
- [ ] **Baseline**: Historical performance baseline established for comparison

### Incident Readiness
- [ ] **Runbooks**: Operational runbooks created for deployment, rollback, and common issues
- [ ] **Runbooks**: Runbooks tested and validated by team members
- [ ] **On-Call**: On-call rotation established and documented
- [ ] **On-Call**: Incident response procedures defined and team trained
- [ ] **Communication**: Incident communication templates prepared (internal and external)

### Acceptance Criteria
- SLOs defined and tracked
- All monitoring and alerting functional and tested
- Runbooks validated and accessible to on-call team
- SRE sign-off obtained

---

## UX & Accessibility Checks Checklist

**Owner**: UX Researcher / Product Designer (with Accessibility Champion support)

**When to use**: Before releasing user-facing features or UI changes

### Design Quality
- [ ] **Design Review**: Design mockups reviewed and approved by design team
- [ ] **Design Review**: Design aligns with design system and brand guidelines
- [ ] **User Research**: User research conducted to validate problem and solution
- [ ] **Usability Testing**: Usability testing completed with target users
- [ ] **Usability Testing**: Critical usability issues identified and resolved
- [ ] **Interaction Design**: User flows documented and validated
- [ ] **Interaction Design**: Edge cases and error states designed and implemented
- [ ] **Responsive Design**: Design tested across target devices and screen sizes

### Accessibility Standards
- [ ] **WCAG Compliance**: Meets WCAG 2.1 Level AA standards (or organizational target)
- [ ] **Keyboard Navigation**: All interactive elements accessible via keyboard
- [ ] **Keyboard Navigation**: Focus indicators visible and logical tab order
- [ ] **Screen Reader**: Semantic HTML used appropriately (headings, landmarks, lists)
- [ ] **Screen Reader**: ARIA labels provided for custom components
- [ ] **Screen Reader**: Tested with screen readers (NVDA, JAWS, VoiceOver)
- [ ] **Color Contrast**: Text and interactive elements meet contrast ratio requirements (4.5:1 for normal text)
- [ ] **Color Contrast**: Information not conveyed by color alone
- [ ] **Alternative Text**: Images have descriptive alt text
- [ ] **Alternative Text**: Decorative images marked as such
- [ ] **Forms**: Form labels properly associated with inputs
- [ ] **Forms**: Error messages clear and associated with fields
- [ ] **Automated Testing**: Automated accessibility tests passing (axe, Lighthouse)
- [ ] **Manual Testing**: Manual accessibility audit completed

### Acceptance Criteria
- Design sign-off obtained from Product Designer
- Accessibility audit passed with no critical issues
- User acceptance testing completed successfully
- UX and Accessibility Champions provide final approval

---

## Analytics Instrumentation Checklist

**Owner**: Data Analyst / Insights Lead

**When to use**: Before releasing features that require measurement or tracking

### Analytics Planning
- [ ] **Success Metrics**: Success metrics and KPIs defined with Product team
- [ ] **Success Metrics**: Baseline metrics captured (if applicable)
- [ ] **Event Schema**: Analytics events defined with clear naming conventions
- [ ] **Event Schema**: Event properties documented (required and optional fields)
- [ ] **Event Schema**: Event schema reviewed and approved by data team
- [ ] **Implementation Plan**: Instrumentation plan documented (what, where, when to track)

### Instrumentation Implementation
- [ ] **Event Tracking**: Analytics events implemented in code
- [ ] **Event Tracking**: Events firing at correct user interaction points
- [ ] **Event Properties**: Event properties capturing expected data
- [ ] **Event Properties**: No PII or sensitive data included in events (unless approved)
- [ ] **Testing**: Test events validated in development environment
- [ ] **Testing**: Test events validated in staging environment
- [ ] **Testing**: Edge cases and error scenarios tested

### Data & Reporting
- [ ] **Data Pipeline**: Events flowing to analytics platform (e.g., Mixpanel, Amplitude, Google Analytics)
- [ ] **Data Pipeline**: Data quality validated (no missing or malformed events)
- [ ] **Dashboards**: Dashboards created for success metrics
- [ ] **Dashboards**: Dashboards shared with stakeholders
- [ ] **Alerts**: Data quality alerts configured (e.g., sudden drop in events)
- [ ] **Documentation**: Analytics documentation updated (event catalog, dashboards)

### Acceptance Criteria
- All events firing correctly and captured in analytics platform
- Dashboards validated and accessible to stakeholders
- Data quality verified with no critical issues
- Data Analyst sign-off obtained

---

## How to use these checklists
1. **At project kickoff**: Identify which checklists apply to your project
2. **During planning**: Assign owners for each checklist section
3. **Before milestones**: Review relevant checklists and track completion
4. **Before release**: Ensure all applicable checklists are complete with sign-offs
5. **Retrospectives**: Update checklists based on learnings and gaps identified

## Integration with Release Process
These checklists complement the main release checklist in [octoacme-release-and-deployment.md](octoacme-release-and-deployment.md). Use them as detailed expansions of the pre-release requirements, ensuring comprehensive coverage of all cross-cutting concerns.
