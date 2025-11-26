# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

For detailed pre-release checklists covering security, observability, UX, accessibility, and analytics, see [cross-cutting-checklists.md](cross-cutting-checklists.md).

## Owners & Role Interactions

Each step in the release process has recommended owners to ensure clear accountability:

| Activity | Primary Owner | Supporting Roles | Deliverable |
|----------|---------------|------------------|-------------|
| CI/CD pipeline & automation | Release / Platform Engineer | Developers | Passing builds, automated tests |
| Deployment to staging | Release / Platform Engineer | Developers | Deployed staging environment |
| Smoke tests execution | QA | Developers, Release Engineer | Test results, sign-off |
| Observability & monitoring setup | Site Reliability / Observability Engineer | Developers | Dashboards, alerts, runbooks |
| Security scans & compliance | Security / Compliance Lead | Developers | Security approval, scan results |
| Release schedule & communications | Project Manager | Product Manager, Change Manager | Schedule, stakeholder notifications |
| Rollback plan documentation | Release / Platform Engineer | SRE, Developers | Rollback procedures, tested plan |
| Support readiness & runbooks | Customer Success / Support Lead | SRE, Developers | Support documentation, FAQs |
| Release announcements | Change Manager / Communications Owner | PM, PdM | Announcement content, training materials |

## Pre-Release Owner Checklist

Before deploying to production, ensure sign-off from the following owners:

- [ ] **Release / Platform Engineer**: CI/CD pipeline passing, deployment automation tested, rollback plan validated
- [ ] **QA**: Smoke tests passed on staging, acceptance criteria verified, no blocking issues
- [ ] **Site Reliability / Observability Engineer**: Monitoring dashboards configured, alerts set up, runbooks updated
- [ ] **Security / Compliance Lead**: Security scans passed (SAST/DAST), threat model reviewed, compliance requirements met
- [ ] **Project Manager**: Release schedule communicated, stakeholders informed, deployment window confirmed
- [ ] **Customer Success / Support Lead**: Support documentation updated, team trained on new features, escalation path clear
- [ ] **Product Manager**: Release scope approved, success metrics defined, rollback criteria established

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
