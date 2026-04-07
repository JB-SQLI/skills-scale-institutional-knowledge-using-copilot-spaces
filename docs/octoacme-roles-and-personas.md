# OctoAcme Personas

## Purpose
Define the roles and responsibilities of everyone who contributes to OctoAcme projects. Use this document to understand team composition, accountability boundaries, and how roles interact with one another. See also: [Project Management Overview](octoacme-project-management-overview.md), [Risks & Communication](octoacme-risks-and-communication.md).

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

### Handoffs
- **From Product Manager:** Receive prioritized backlog items with acceptance criteria before each sprint.
- **To QA/Test Engineer:** Hand off completed features with test notes; confirm automated tests pass before review.
- **To DevOps Engineer:** Provide deployable artifacts and environment configuration changes; coordinate timing with release windows.

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

### Handoffs
- **To Developers:** Deliver prioritized backlog items with clear acceptance criteria at sprint start.
- **To UX Designer:** Share user research, problem statements, and feature goals to inform design direction.
- **From Customer Success:** Receive user feedback, adoption signals, and support trends to feed into backlog prioritization.
- **From Business Analyst:** Review documented requirements and business rules before committing items to the roadmap.

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

### Handoffs
- **To/From all roles:** Own the cross-team coordination checklist (see [Project Planning](octoacme-project-planning.md)); ensure dependencies are tracked and escalated promptly.
- **To Product Manager:** Escalate scope, timeline, and resource decisions; share risk register updates.
- **From DevOps Engineer:** Receive deployment status and release timing confirmations to include in stakeholder updates.

---

## UX Designer

### Role Summary
UX Designers create intuitive, user-centered workflows and ensure that solutions are accessible, visually consistent, and validated against real user needs before development begins.

### Responsibilities
- Collaborate with Product Managers and Developers on requirements and design feasibility
- Create wireframes, prototypes, and interaction flows
- Conduct usability testing and incorporate findings into design iterations
- Define and maintain design guidelines and component libraries
- Participate in design reviews and provide feedback on implemented UI

### Goals
- Deliver highly usable products with minimal user confusion or rework
- Ensure accessibility and consistency across all surfaces
- Reduce costly late-stage design changes by validating early

### Typical Communication
- Sync with Product Manager to align on feature priorities and user research findings
- Share design specs and prototypes with Developers in sprint planning
- Communicate usability test results at demo/review sessions

### Handoffs
- **From Product Manager:** Receive problem statements, user research, and prioritized feature goals to begin design work.
- **To Developers:** Deliver finalized design specs, prototypes, and interaction guidelines at the start of implementation sprint.
- **To Quality Advocate/Test Engineer:** Share acceptance criteria for visual and interaction standards; flag accessibility requirements.
- **From Developers:** Review implemented UI against design specs and provide sign-off or revision requests.

---

## DevOps Engineer

### Role Summary
DevOps Engineers build and maintain the CI/CD pipelines, automate infrastructure, and enable speedy, reliable, and repeatable deployments across all environments.

### Responsibilities
- Design and manage infrastructure-as-code and deployment pipelines
- Monitor deployment health, alert thresholds, and on-call response
- Provision and maintain development, staging, and production environments
- Implement security scanning, secrets management, and access controls in CI/CD
- Coordinate deployment windows and rollback procedures with the delivery team

### Goals
- Minimize deployment friction and production incidents
- Ensure robust rollback capability and fast mean-time-to-recover (MTTR)
- Keep environments consistent and auditable

### Typical Communication
- Coordinate deployment timing with Project Manager and Developers
- Provide environment status updates in daily standups when releases are in flight
- Document runbooks and post-incident learnings

### Handoffs
- **From Developers:** Receive deployable artifacts and infrastructure change requests; review environment configuration diffs before deployment.
- **To Project Manager:** Confirm deployment completion and post-deploy verification results for inclusion in stakeholder updates.
- **To Quality Advocate/Test Engineer:** Confirm staging environment readiness before QA testing begins.
- **With Customer Success:** Communicate production release status and known issues so support teams can prepare.

---

## Quality Advocate / Test Engineer

### Role Summary
Quality Advocates (Test Engineers) champion quality throughout the delivery lifecycle—defining test strategy, automating regression coverage, and ensuring features meet acceptance criteria before release.

### Responsibilities
- Define and own the test strategy (unit, integration, end-to-end, exploratory)
- Develop and maintain automated test suites in CI
- Perform manual QA for critical features and new releases
- Document and track defects; verify fixes before closure
- Participate in sprint planning to flag testability concerns early

### Goals
- Catch defects as early and cheaply as possible
- Maintain high confidence in release quality
- Reduce production incidents caused by regressions

### Typical Communication
- Attend sprint planning and review sessions to understand scope and acceptance criteria
- Report test results and open defects in daily standups or dedicated QA syncs
- Collaborate with Developers on automated test coverage gaps

### Handoffs
- **From Developers:** Receive feature branches or builds with passing unit tests and test notes; begin QA only after CI passes.
- **From DevOps Engineer:** Confirm environment parity with production before running end-to-end tests.
- **From UX Designer:** Receive visual/interaction acceptance criteria and accessibility requirements.
- **To Project Manager:** Report QA pass/fail status to inform go/no-go decisions for release; see [Release & Deployment](octoacme-release-and-deployment.md).

---

## Business Analyst

### Role Summary
Business Analysts bridge business strategy and technical delivery by eliciting, documenting, and validating requirements so that the right solution is built efficiently.

### Responsibilities
- Facilitate requirements workshops with stakeholders and subject matter experts
- Document business rules, process flows, and data requirements
- Translate business needs into clear, testable user stories and acceptance criteria
- Analyze gaps between current and desired states and recommend solutions
- Support User Acceptance Testing (UAT) coordination and sign-off

### Goals
- Ensure solutions align with business objectives and measurable outcomes
- Reduce ambiguity and rework caused by unclear requirements
- Build shared understanding between business stakeholders and delivery teams

### Typical Communication
- Lead requirements workshops and follow-up meetings with stakeholders
- Share requirement specifications and process diagrams with Product Manager and Developers
- Provide status updates on requirements coverage to Project Manager

### Handoffs
- **To Product Manager:** Deliver documented requirements, business rules, and gap analysis to inform roadmap and backlog decisions.
- **To Developers:** Provide detailed acceptance criteria, data models, and process diagrams at sprint start.
- **To Quality Advocate/Test Engineer:** Share UAT test cases and acceptance criteria for incorporation into the test plan.
- **From Customer Success:** Receive user pain points and workflow friction reports to shape requirements.

---

## Technical Writer

### Role Summary
Technical Writers produce clear, accurate, and user-friendly documentation—covering APIs, process guides, user manuals, and release notes—so that all stakeholders can use and maintain the product effectively.

### Responsibilities
- Author and maintain user guides, API references, onboarding materials, and process documentation
- Collaborate with Developers and Product Managers to ensure technical accuracy
- Update documentation as part of the Definition of Done for each sprint
- Establish and enforce documentation standards and templates
- Support knowledge transfer for new team members and handoffs

### Goals
- Reduce support load by enabling users to self-serve
- Ensure documentation is always current and discoverable
- Improve onboarding time for new team members and contributors

### Typical Communication
- Attend sprint reviews to capture changes requiring documentation updates
- Sync with Developers and Product Managers to review and approve content
- Coordinate with Customer Success on user-facing guides and FAQs

### Handoffs
- **From Developers:** Receive technical details, API changes, and feature descriptions in time to publish docs with the release.
- **From Product Manager:** Receive product messaging, feature context, and release timing to align user-facing content.
- **To Customer Success:** Deliver finalized user guides and FAQs before release; notify of any changes to support playbooks.
- **To Project Manager:** Confirm documentation deliverables are complete as part of the release go/no-go checklist.

---

## Customer Success / Support Representative

### Role Summary
Customer Success and Support Representatives are the voice of the customer post-release. They ensure users can adopt the product successfully, capture feedback and issues, and escalate trends to the delivery team.

### Responsibilities
- Provide first-line user support and triage incoming issues
- Document recurring user pain points and escalate to Product Manager and Project Manager
- Validate that release communications (notes, guides, FAQs) are clear and complete before going live
- Coordinate with the delivery team during and after releases to monitor adoption and incidents
- Contribute user feedback to the backlog and retrospectives

### Goals
- Maximize product adoption and user satisfaction
- Reduce time-to-resolution for user-reported issues
- Provide a continuous feedback loop from users to the product and delivery team

### Typical Communication
- Daily monitoring of support channels; escalate critical issues immediately
- Weekly feedback summary shared with Product Manager and Project Manager
- Participate in retrospectives to surface systemic issues

### Handoffs
- **From DevOps Engineer:** Receive production deployment notifications and known issues so support teams can set expectations with users.
- **From Technical Writer:** Receive updated user guides and FAQs before each release.
- **To Product Manager:** Deliver compiled user feedback, adoption metrics, and recurring issue trends for backlog input.
- **To Project Manager:** Escalate active incidents or user-impacting issues for prioritization and stakeholder communication; see [Risks & Communication](octoacme-risks-and-communication.md).

---

## Role Handoff Checklist

Use this checklist when transitioning work between roles to maintain quality and reduce gaps:

- [ ] Acceptance criteria documented and agreed upon before development starts (Product Manager → Developers → QA)
- [ ] Design specs reviewed and signed off by UX Designer before implementation sprint
- [ ] Automated tests pass in CI before feature is handed to QA (Developers → QA)
- [ ] Staging environment verified as production-equivalent before QA testing (DevOps → QA)
- [ ] QA sign-off obtained before release go/no-go decision (QA → Project Manager)
- [ ] Documentation updated and approved before release (Technical Writer → Project Manager)
- [ ] Deployment confirmed and post-deploy checks passed (DevOps → Project Manager)
- [ ] Release notes and user guides delivered to Customer Success before release (Technical Writer + DevOps → Customer Success)
- [ ] Post-release feedback loop opened: Customer Success reporting back to Product Manager within 1 week of release

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Project Management Overview](octoacme-project-management-overview.md) for how these roles interact across the delivery lifecycle.

