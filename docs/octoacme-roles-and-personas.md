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

## DevOps Engineer

### Role Summary
DevOps Engineers own the CI/CD pipelines, infrastructure, deployment automation, and observability stack. They bridge development and operations to ensure reliable, repeatable delivery.

### Responsibilities
- Design, build, and maintain CI/CD pipelines and deployment automation
- Manage cloud infrastructure, environments (dev/staging/prod), and access controls
- Implement and monitor observability tooling (logs, metrics, alerts, dashboards)
- Ensure release checklists are followed and rollback playbooks are current
- Support incident response and post-incident root-cause analysis
- Collaborate with Developers on containerization, environment parity, and dependency management

### Goals
- Reduce deployment lead time and rollback risk
- Maintain high availability and reliability of production systems
- Enable developers to ship with confidence through automated quality gates

### Typical Communication
- Coordinates with Project Manager on deployment windows and release schedules
- Pairs with Developers on build/deploy issues and environment configuration
- Participates in release readiness reviews and incident retrospectives
- Updates runbooks and deployment docs as infrastructure evolves

### Lifecycle Participation
- **Planning**: contributes infrastructure estimates and environment readiness timeline
- **Execution**: maintains pipelines and resolves environment or deployment blockers
- **Release**: leads deployment execution, monitors post-deploy health, and triggers rollback if needed
- **Retrospective**: identifies reliability and automation improvement action items

---

## Security Lead

### Role Summary
The Security Lead oversees security reviews, compliance requirements, and incident response. They ensure that security is integrated into the development lifecycle rather than bolted on at release time.

### Responsibilities
- Conduct security design reviews and threat-modeling sessions during planning
- Review PRs and release artifacts for security risks (dependency vulnerabilities, misconfigurations)
- Maintain the security incident runbook and coordinate security-specific escalations
- Ensure compliance with internal standards and applicable regulations
- Sign off on releases that include security-sensitive changes
- Partner with Developers to remediate vulnerabilities identified in CI security scans

### Goals
- Shift security left by embedding reviews early in the lifecycle
- Minimize the risk surface of every release
- Ensure the team can respond quickly and confidently to security incidents

### Typical Communication
- Works with Product Manager to incorporate security requirements into acceptance criteria
- Escalates unresolved security risks to Project Manager and Product Lead
- Provides security sign-off as a pre-release gate (see cross-functional handoffs checklist)
- Reports on security posture during weekly delivery syncs when relevant

### Lifecycle Participation
- **Initiation**: flags regulatory or compliance constraints that affect scope
- **Planning**: participates in threat modeling and risk register entries for security risks
- **Execution**: reviews security-sensitive PRs and monitors CI scanning results
- **Release**: provides explicit security sign-off before production deployment
- **Retrospective**: contributes security learnings and hardening action items

---

## UX Designer

### Role Summary
UX Designers shape the user experience, ensure accessibility and usability standards are met, and validate designs with users and stakeholders before and during development.

### Responsibilities
- Conduct user research, usability tests, and design critiques
- Create wireframes, prototypes, and design specifications
- Maintain a shared design system and ensure consistency across features
- Contribute usability and accessibility requirements to acceptance criteria
- Partner with Developers during implementation to answer design questions and review built UI
- Validate final implementations against design specifications before release

### Goals
- Ensure product changes improve usability and meet accessibility standards
- Reduce rework caused by late-stage design changes
- Build a shared understanding of user needs across the team

### Typical Communication
- Collaborates with Product Manager on roadmap priorities and feature discovery
- Works directly with Developers during implementation sprints
- Presents designs to stakeholders for feedback and sign-off
- Participates in retrospectives to improve design-development collaboration

### Lifecycle Participation
- **Initiation**: contributes user research insights to the project one-pager
- **Planning**: delivers design specs and acceptance criteria inputs before development starts
- **Execution**: available for design Q&A, reviews built UI, and validates usability
- **Release**: confirms UX review is complete as a pre-release gate
- **Retrospective**: identifies improvements to the design handoff process

---

## Support Specialist

### Role Summary
Support Specialists represent the voice of the customer within the team. They gather user feedback, manage post-release communications, and ensure support documentation is current so customers and support staff are ready for changes.

### Responsibilities
- Maintain and update support documentation, FAQs, and help center articles
- Gather and relay user feedback and recurring support issues to the product team
- Ensure support team readiness before feature releases (training, runbooks, escalation paths)
- Manage external release communications and user-facing changelogs
- Participate in incident triage to provide customer impact context

### Goals
- Reduce support ticket volume through clear documentation and proactive communication
- Ensure customers and internal support staff are prepared for every release
- Surface user pain points that inform product prioritization

### Typical Communication
- Coordinates with Project Manager on release timing and announcement schedules
- Collaborates with Product Manager to shape user-facing release notes and FAQs
- Provides a support readiness sign-off before production deployment
- Shares support trends and feedback in monthly retrospectives or stakeholder updates

### Lifecycle Participation
- **Planning**: identifies documentation and training work needed for new features
- **Execution**: drafts support docs and FAQs in parallel with development
- **Release**: confirms support readiness as a pre-release gate; announces to users
- **Retrospective**: brings user feedback and support metrics to drive continuous improvement

---

## Data Analyst

### Role Summary
Data Analysts track success metrics, analyze project outcomes, and provide data-informed insights to support decision-making. They ensure the team measures what matters and acts on evidence.

### Responsibilities
- Define and instrument key metrics aligned to success criteria from the project one-pager
- Build and maintain dashboards and reports that reflect project health
- Analyze post-release data to validate outcomes against goals
- Identify anomalies and surface actionable insights during execution
- Partner with Product Manager on data-driven roadmap prioritization

### Goals
- Ensure every project has clear, measurable success criteria and the data to assess them
- Accelerate evidence-based decision-making across the team
- Track continuous improvement by measuring the impact of process and product changes

### Typical Communication
- Works closely with Product Manager to align metrics with product goals
- Presents data summaries at sprint reviews and stakeholder updates
- Contributes outcome data to retrospectives as a basis for improvement action items
- Coordinates with DevOps Engineer on instrumentation and data pipeline needs

### Lifecycle Participation
- **Initiation**: helps define measurable success criteria in the project one-pager
- **Planning**: ensures instrumentation and tracking are in scope
- **Execution**: monitors leading indicators and flags anomalies to the team
- **Release**: validates post-release metrics against baseline targets
- **Retrospective**: presents outcome data and trend analysis to inform action items

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [`octoacme-cross-functional-handoffs-checklist.md`](octoacme-cross-functional-handoffs-checklist.md) for how these roles interact at key hand-off points across the project lifecycle.

