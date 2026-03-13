# OctoAcme — Cross-Functional Hand-offs Checklist

## Purpose
Define when each role must be involved in a project, what inputs and outputs are expected, and where sign-off or approval is required. This checklist is reusable across projects and integrates with the [Execution & Tracking](octoacme-execution-and-tracking.md), [Risk Management & Communication](octoacme-risks-and-communication.md), and [Release & Deployment](octoacme-release-and-deployment.md) guides.

For full role descriptions see [`octoacme-roles-and-personas.md`](octoacme-roles-and-personas.md).

---

## 1. Initiation Hand-offs

| Trigger | Role to Involve | Required Inputs | Expected Outputs | Sign-off / Approval |
|---------|----------------|-----------------|------------------|---------------------|
| New project or feature proposed | Product Manager, Project Manager | Problem statement, rough scope | Project one-pager, stakeholder list | Sponsor / Product Lead approval to proceed |
| Regulatory or compliance scope identified | Security Lead | Project one-pager | Compliance requirements list, initial risk register entries | Security Lead acknowledgement |
| User-facing feature proposed | UX Designer | Problem statement, user research (if available) | Design discovery notes, initial usability constraints | UX Designer brief confirmed |
| Success metrics need definition | Data Analyst | Project one-pager goals | Measurable success criteria, instrumentation plan | Product Manager + Data Analyst agreement |

### Initiation Checklist
- [ ] Project one-pager reviewed by Project Manager and Product Manager
- [ ] Stakeholder list includes all impacted roles (DevOps, Security, UX, Support, Data as applicable)
- [ ] Security Lead notified if security-sensitive scope is identified
- [ ] Data Analyst has confirmed measurable success criteria

---

## 2. Planning Hand-offs

| Trigger | Role to Involve | Required Inputs | Expected Outputs | Sign-off / Approval |
|---------|----------------|-----------------|------------------|---------------------|
| Backlog creation and estimation | All delivery roles | Approved one-pager, stakeholder inputs | Prioritized backlog with acceptance criteria | Product Manager approval |
| Infrastructure or environment requirements defined | DevOps Engineer | Feature requirements, architecture proposal | Environment plan, CI/CD setup tasks, infra estimates | DevOps Engineer sign-off on feasibility |
| Threat model or security review required | Security Lead | Feature designs, data flow diagrams | Threat model, security requirements added to backlog | Security Lead sign-off on threat model |
| Design specifications required | UX Designer | Accepted user stories, research findings | Wireframes, design specs, accessibility requirements | Product Manager + stakeholder design sign-off |
| Support documentation scope estimated | Support Specialist | Feature scope, release timeline | Support doc list and effort estimates, training plan | Project Manager confirmation in plan |
| Metrics and tracking plan required | Data Analyst | Success criteria, feature scope | Instrumentation tasks added to backlog, dashboard design | Product Manager agreement on metrics |

### Planning Checklist
- [ ] Kickoff held with all required roles present
- [ ] Backlog includes tasks for: infrastructure setup, security review, design specs, support docs, instrumentation
- [ ] DevOps Engineer has confirmed environment and pipeline readiness timeline
- [ ] Security Lead has reviewed designs for security requirements
- [ ] UX Designer has provided initial wireframes or specs before development begins
- [ ] Definition of Done updated to include UX review, security sign-off, and support readiness as applicable

---

## 3. Execution Hand-offs

| Trigger | Role to Involve | Required Inputs | Expected Outputs | Sign-off / Approval |
|---------|----------------|-----------------|------------------|---------------------|
| PR ready for review (security-sensitive change) | Security Lead | PR diff, context on change | Security review comments, vulnerability findings | Security Lead approval on PR |
| PR ready for review (UI/UX change) | UX Designer | PR diff, design spec | UX review comments, acceptance of implementation | UX Designer approval on PR |
| Environment or pipeline issue blocking team | DevOps Engineer | Error logs, reproduction steps | Pipeline fix, environment patch, updated runbook | DevOps Engineer sign-off that blocker is resolved |
| Support doc drafts ready for review | Support Specialist | Feature description, draft docs | Reviewed and approved support articles | Support Specialist sign-off on draft |
| Leading metric anomaly detected | Data Analyst | Dashboard / monitoring alert | Analysis summary, recommended action | PM + Data Analyst agreement on response |

### Execution Checklist
- [ ] Security-sensitive PRs have Security Lead approval before merge
- [ ] UI PRs have UX Designer approval before merge
- [ ] DevOps Engineer has resolved all environment blockers and updated runbooks
- [ ] Support Specialist has reviewed draft support documentation
- [ ] Data Analyst is monitoring leading indicators and has flagged any anomalies

---

## 4. Pre-Release Hand-offs

| Trigger | Role to Involve | Required Inputs | Expected Outputs | Sign-off / Approval |
|---------|----------------|-----------------|------------------|---------------------|
| Release candidate ready | DevOps Engineer | All PRs merged, CI passing | Deployment plan, staging test results, rollback plan | DevOps Engineer sign-off |
| Release contains security-sensitive changes | Security Lead | Release candidate, security scan results | Security sign-off memo or approval comment | **Security Lead sign-off required before production** |
| Release contains user-facing UI changes | UX Designer | Staging environment, design spec | UX acceptance confirmed on staging | **UX Designer sign-off required before production** |
| Release affects customer workflows or documentation | Support Specialist | Release notes draft, support doc updates | Support readiness confirmed, announcement drafted | **Support Specialist sign-off required before production** |
| Post-release metrics baseline established | Data Analyst | Dashboard and alert configuration | Baseline metrics snapshot, monitoring alerts active | Data Analyst confirms monitoring is active |

### Pre-Release Checklist
- [ ] All acceptance criteria met and PRs merged to release branch
- [ ] CI passing: tests, linting, security scans
- [ ] DevOps Engineer has confirmed deployment plan and rollback procedure
- [ ] **Security Lead sign-off** obtained (for security-sensitive changes)
- [ ] **UX Designer sign-off** obtained (for user-facing UI changes)
- [ ] **Support Specialist sign-off** obtained: docs updated, team trained, announcement drafted
- [ ] Data Analyst has confirmed monitoring is active with baseline metrics
- [ ] Release notes reviewed and approved

---

## 5. Release & Post-Release Hand-offs

| Trigger | Role to Involve | Required Inputs | Expected Outputs | Sign-off / Approval |
|---------|----------------|-----------------|------------------|---------------------|
| Production deployment executed | DevOps Engineer | Approved deployment plan | Deployment complete, post-deploy health checks passed | DevOps Engineer confirms production healthy |
| Release announcement needed | Support Specialist | Final release notes | User-facing announcement published | Support Specialist confirms announcement sent |
| Post-release metrics review | Data Analyst | Production metrics, success criteria | Outcome analysis report | Product Manager acknowledges results |
| Post-release security review | Security Lead | Production monitoring, incident queue | Security health summary | Security Lead confirms no outstanding issues |

### Post-Release Checklist
- [ ] DevOps Engineer confirms production is healthy (monitors, alerts, error rates normal)
- [ ] Support Specialist has published release announcement and updated help docs
- [ ] Data Analyst has compared post-release metrics to baseline targets
- [ ] Security Lead has confirmed no new security issues introduced

---

## 6. Retrospective Hand-offs

| Trigger | Role to Involve | Required Inputs | Expected Outputs |
|---------|----------------|-----------------|------------------|
| Sprint or project retrospective | All roles | Sprint/project outcomes, action item backlog | Updated action items with owners and due dates |
| Support trends to review | Support Specialist | Support ticket data | Feedback summary and product improvement suggestions |
| Metric outcome analysis | Data Analyst | Post-release metrics report | Data-driven retrospective inputs and trend analysis |
| Infrastructure or reliability issues | DevOps Engineer | Incident logs, deployment metrics | Reliability improvement action items |
| Security findings review | Security Lead | Security scan history, incident queue | Security hardening action items |

### Retrospective Checklist
- [ ] All relevant roles have contributed inputs before the retro session
- [ ] Support Specialist has shared support ticket trends
- [ ] Data Analyst has presented outcome metrics vs. success criteria
- [ ] Action items from previous retro have been reviewed for completion
- [ ] New action items captured with clear owners, due dates, and success criteria

---

## Escalation Quick Reference

| Situation | Escalation Path |
|-----------|----------------|
| Security vulnerability discovered in production | Security Lead → Project Manager → Product Lead → Sponsor |
| Deployment failure or production incident | DevOps Engineer → Project Manager → on-call (per incident runbook) |
| Accessibility or UX blocker in staging | UX Designer → Project Manager → Product Manager |
| Critical support gap before release | Support Specialist → Project Manager → Product Manager |
| Success metrics cannot be established | Data Analyst → Product Manager → Project Manager |
| Cross-team dependency blocked | Project Manager → Product Lead → Sponsor |

---

## Related Documents
- [Roles & Personas](octoacme-roles-and-personas.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
