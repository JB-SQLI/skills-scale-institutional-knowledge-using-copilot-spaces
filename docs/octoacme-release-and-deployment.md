# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability. See also: [Roles & Personas](octoacme-roles-and-personas.md) for role responsibilities during release, and [Risks & Communication](octoacme-risks-and-communication.md) for release communication templates.

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

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Role Handoff Checklist for Release
- [ ] **Quality Advocate/Test Engineer** — QA sign-off complete; no open P1/P2 defects
- [ ] **UX Designer** — UI acceptance review complete
- [ ] **Technical Writer** — Release notes, user guides, and FAQs finalized and delivered to Customer Success
- [ ] **DevOps Engineer** — Pipeline passing; rollback plan confirmed; deployment window communicated to Project Manager
- [ ] **Business Analyst** — UAT sign-off obtained from business stakeholders
- [ ] **Project Manager** — Go/no-go decision recorded; stakeholder communication sent (see [Risks & Communication](octoacme-risks-and-communication.md))
- [ ] **Customer Success** — Notified of release, known issues, and support escalation path

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
