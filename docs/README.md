# OctoAcme Project Management Docs

OctoAcme's project management approach is organized around a lightweight, repeatable lifecycle with clear artifacts that serve as the source of truth. Work moves through **Initiation → Planning → Execution → Release → Close/Retrospective**, with an emphasis on iterative delivery, clear ownership, and data-informed decision-making. Teams begin by aligning on a **Project One-pager/Charter** — capturing the problem, objective, and success metrics — before identifying stakeholders, sketching an initial timeline, and confirming that team availability and stakeholder alignment are in place before moving into delivery planning.

Roles are explicitly defined to reduce ambiguity: the **Project Manager (PM)** coordinates delivery, schedules, risks, and communications; the **Product Manager (PdM/Product Lead)** defines outcomes and prioritizes the backlog; **Developers** design, build, and test while contributing to estimation and technical risk mitigation; **QA/Testing** validates acceptance criteria and quality; and **Stakeholders** provide input and approvals. Planning translates an approved initiative into an actionable backlog through a kickoff, breaking work into shippable increments with **acceptance criteria** and a **Definition of Done**, estimating effort, mapping dependencies, and establishing a release and milestone plan.

Execution relies on a structured project board (states: **Backlog → Ready → In Progress → In Review → QA → Done**) and a disciplined pull request workflow — small PRs, linked issues, CI checks (tests, lint, security scanning) passing before review, and at least one team approval required. Delivery is managed through a consistent operating rhythm: daily standups, weekly delivery syncs, and regular demos/reviews, with progress tracked via velocity/burndown, success metrics from the One-pager, and operational dashboards (errors, latency, usage).

Communication and risk management are ongoing practices. Teams maintain a **risk register** (impact, likelihood, owner, mitigation, status) and follow a defined escalation path: team triage → PM/Product Lead and dependent teams → sponsor-level escalation for business-impacting issues. Quality assurance is layered across the lifecycle: unit and integration tests for new logic, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA for acceptance. Releases follow a standardized checklist (acceptance criteria met, CI/security passing, release notes drafted, rollback plan in place, staged deployments with post-deploy verification), and each cycle closes with a retrospective producing owned, time-bound action items tracked back into the backlog.

---

## Docs Directory

| Document | Description |
|---|---|
| [Project Management Overview](./octoacme-project-management-overview.md) | High-level overview of OctoAcme's project management philosophy and lifecycle |
| [Project Initiation](./octoacme-project-initiation.md) | Initiating a project: One-pager/charter, stakeholder alignment, and decision gates |
| [Project Planning](./octoacme-project-planning.md) | Translating an initiative into a backlog, milestones, and a release plan |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Board workflow, PR process, operating rhythm, and progress reporting |
| [Risks & Communication](./octoacme-risks-and-communication.md) | Risk register, escalation paths, and communication cadence |
| [Release & Deployment](./octoacme-release-and-deployment.md) | Release checklist, staged deployments, rollback, and post-deploy verification |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Retrospective format, action item tracking, and improvement backlog |
| [Roles & Personas](./octoacme-roles-and-personas.md) | Defined roles, responsibilities, and personas across the project lifecycle |

---

## Contributing

To propose improvements to any of these process documents, or to suggest new documentation, please use the issue templates in [`.github/ISSUE_TEMPLATE/`](../.github/ISSUE_TEMPLATE/). Submit your request there so it can be reviewed, discussed, and tracked alongside other process improvements.
