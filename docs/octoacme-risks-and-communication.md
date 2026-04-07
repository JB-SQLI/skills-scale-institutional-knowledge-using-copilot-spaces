# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies. See also: [Roles & Personas](octoacme-roles-and-personas.md) for escalation owners, [Release & Deployment](octoacme-release-and-deployment.md) for release-specific communications, and [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) for post-incident learning.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates

### Weekly Status Update Template
**Subject:** [Project Name] — Weekly Status Update (Week of MM/DD)

- **Overall Status:** 🟢 On Track / 🟡 At Risk / 🔴 Off Track
- **Progress this week:**
- **Next steps (coming week):**
- **Risks & blockers:**
- **Ask / decisions needed:**
- **Key metrics / milestones:**

_Owner: Project Manager. Frequency: Weekly. Audience: Stakeholders, Product Manager, sponsor._

---

### Incident Status Communication Template
**Subject:** [INCIDENT] [Severity: P1/P2/P3] — [Short Description] — Status Update

- **Current status:** Investigating / Mitigating / Resolved
- **Impact:** (What is affected and how many users)
- **Timeline:**
  - HH:MM — Issue detected
  - HH:MM — Triage started
  - HH:MM — Mitigation applied (if applicable)
- **Actions being taken:**
- **Next update by:** HH:MM
- **Escalation contact:**

_Owner: Project Manager + DevOps Engineer. Update frequency: Every 30 min for active P1; hourly for P2. Audience: Stakeholders, Customer Success, on-call team._

Post-incident: schedule a blameless retrospective within 48 hours. See [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md).

---

### Release Communication Template
**Subject:** [Project Name] vX.Y — Release Announcement

- **Release date:**
- **What's new:** (summary for non-technical audience)
- **Notable changes / features:**
- **Migration or action required?** Yes / No — (details if yes)
- **Known issues:**
- **Support contact / FAQ link:**

_Owner: Technical Writer (drafts) + Product Manager (approves) + Project Manager (sends). Audience: Customer Success, stakeholders, users. See [Release & Deployment](octoacme-release-and-deployment.md) for full checklist._

---

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
