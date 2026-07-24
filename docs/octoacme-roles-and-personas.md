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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas

To reduce ambiguity, improve cross-functional handoffs, and make operational responsibilities explicit, add the following personas. For each persona below we include: Role Summary, Responsibilities, Typical Communication, and Interaction notes with PM, PdM, Developers, and QA.

### Release Manager

Role Summary
- Coordinates release windows and executes release runbooks to ensure safe, observable deployments.

Responsibilities
- Maintain and execute the release checklist and rollback plan.
- Coordinate deployment windows and stakeholder communications.
- Validate release readiness (CI, QA, feature flags).
- Confirm post-release verifications and monitor for regressions.

Typical Communication
- Release planning meetings, deployment notifications, post-release summaries.

Interactions
- PM: Align on release scope and stakeholder comms.
- PdM: Confirm acceptance criteria and feature readiness.
- Developers: Coordinate deployment steps and rollback procedures.
- QA: Ensure smoke tests and verification tasks are complete.
- Support/SRE: Communicate on-call readiness and monitoring.

### Delivery Lead

Role Summary
- Drives day-to-day delivery execution, removing blockers and ensuring work meets the Definition of Done.

Responsibilities
- Orchestrate delivery across teams and validate backlog readiness.
- Manage sprint flow and escalate impediments.
- Ensure acceptance criteria and DoD are enforced.

Typical Communication
- Daily touchpoints with team leads, sprint planning facilitation, escalation reports.

Interactions
- PM/PdM: Translate priorities into execution plans.
- Developers & QA: Coordinate handoffs and acceptance activities.
- Release Manager: Coordinate release timing and readiness.

### SRE / Reliability Engineer

Role Summary
- Owns system reliability, SLIs/SLAs, and operational readiness.

Responsibilities
- Define SLIs, error budgets, and runbooks.
- Review deployability, observability, and incident runbooks.
- Lead incident response for production issues and coordinate post-incident actions.

Typical Communication
- On-call handovers, incident bridges, reliability reviews.

Interactions
- Developers: Collaborate on architecture and remediation.
- PM: Advise on reliability trade-offs and release risk.
- Release Manager: Validate operational readiness for releases.
- QA: Advise on testing and monitoring required for reliability.

### Data Analyst / Product Analyst

Role Summary
- Provides measurement, instrumentation, and analysis to validate outcomes and guide prioritization.

Responsibilities
- Define success metrics and instrumentation requirements.
- Produce dashboards, experiment analyses, and decision-focused reports.
- Support validation of features through telemetry.

Typical Communication
- Metric reports, dashboard updates, experiment summaries.

Interactions
- PdM: Set measurable goals and acceptance metrics.
- Developers: Provide instrumentation specs and validate data capture.
- QA: Help validate data-driven acceptance criteria.

### Design Researcher / UX Lead

Role Summary
- Ensures product decisions are grounded in user research and usability validation.

Responsibilities
- Run user research, usability testing, and synthesize findings.
- Provide UX acceptance criteria and design guidance.
- Advocate for accessibility and usability in scope and DoD.

Typical Communication
- Research summaries, design reviews, UX acceptance notes.

Interactions
- PdM: Collaborate on problem framing and prioritization.
- Developers: Handoff designs and acceptance details.
- QA: Highlight usability test cases and accessibility checks.

### Security / Compliance Lead

Role Summary
- Ensures security and compliance considerations are integrated into planning and delivery.

Responsibilities
- Review threat models and compliance requirements.
- Own security checklists and scan remediation guidance.
- Participate in design reviews and pre-release security gating.

Typical Communication
- Security reviews, compliance checklists, remediation tickets.

Interactions
- Developers: Review implementations and advise on fixes.
- PM/PdM: Communicate compliance impacts and timelines.
- Release Manager: Gate releases when security issues are unresolved.

### Customer Success / Support Liaison

Role Summary
- Represents customer-facing perspectives and enables successful rollouts and support readiness.

Responsibilities
- Capture support trends and customer feedback.
- Prepare customer-facing communications and enablement content.
- Support incident prioritization based on customer impact.

Typical Communication
- Support summaries, onboarding materials, release notes for customers.

Interactions
- PM: Provide customer impact context for prioritization.
- Release Manager: Coordinate customer communications and known issues.
- Developers & QA: Provide reproduction details and impact context for fixes.

---

## Interaction matrix (summary)

A concise matrix helps teams quickly identify primary collaborators for common activities:

| Activity / Role | PM | PdM | Dev | QA | Release Mgr | SRE | Data | UX | Security | Support |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Define success metrics | C | A | C | C | I | I | R | I | I | C |
| Release coordination | I | C | R | C | A/R | I | I | I | I | C |
| Incident response | I | I | R | I | C | A/R | I | I | C | C |
| Pre-release security review | I | I | C | I | I | I | I | I | A/R | I |
| Usability validation | I | A | C | C | I | I | I | R | I | C |

Legend: R = Responsible, A = Accountable, C = Consulted, I = Informed

---
