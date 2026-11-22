# AI Implementation Delivery Management Playbook

**Project:** AI Governance Readiness Workbench  
**Version:** 1.0  
**Role:** AI Implementation Project Manager  
**Status:** Portfolio simulation

## 1. Requirements Traceability

Every approved business requirement must be traceable through:

Business objective → Requirement ID → User story → Design → Implementation task → Test case → Evidence → Business acceptance.

Example:

- Requirement: FR-009
- Jira issue: AIW-24
- Story: Escalate potential prohibited-practice indicators.
- Design reference: ARCH-04.
- Test case: TC-009.
- Evidence: Recorded synthetic test output.
- Acceptance: Authorised Legal reviewer decision.

A Jira issue marked Done is not sufficient evidence of business acceptance.

## 2. Jira Delivery Structure

- Epic: AI Regulatory Screening.
- Story: FR-009 — Potential indicator escalation.
- Subtasks: Configure screening logic, source references and routing.
- Bug: Incorrect result found during testing.
- Evidence: Test register and assessment record.

Use requirement IDs in Jira issue descriptions and maintain links to test evidence.

## 3. Requirements Traceability Metrics

- Requirements coverage = requirements linked to design and implementation / total approved requirements × 100.
- Test coverage = requirements with executed tests / total approved requirements × 100.
- Test pass rate = passed tests / executed tests × 100.
- Acceptance rate = accepted requirements / requirements due for acceptance × 100.

Report each metric separately.

## 4. Budget Baseline

Illustrative eight-week project budget: €53,590.

| Stage | Budget |
|---|---:|
| Initiation | €5,000 |
| Discovery | €8,000 |
| Design | €10,000 |
| Build | €16,000 |
| Validation | €9,000 |
| Handover | €5,590 |
| Total | €53,590 |

These figures are planning assumptions, not actual expenditure or a supplier quotation.

Track approved budget, actual cost, forecast at completion, estimate to complete and contingency separately.

## 5. Estimation and Capacity

Use:
- Bottom-up estimates for work packages.
- Three-point PERT for uncertainty.
- CPM for dependency and critical-path analysis.
- Fibonacci story points for relative backlog complexity.
- Team capacity and historical velocity for sprint planning.

PERT formula:

E = (Optimistic + 4 × Most likely + Pessimistic) / 6.

Story points are relative estimates, not hours.

## 6. Workshop Facilitation

90-minute discovery workshop:
- 10 minutes: objectives.
- 15 minutes: current-state process.
- 15 minutes: pain points and root causes.
- 15 minutes: future-state workflow.
- 10 minutes: risk and controls.
- 10 minutes: MoSCoW prioritisation.
- 10 minutes: decisions and owners.
- 5 minutes: recap.

Outputs: process map, requirements, decision log, action log, dependencies and open questions.

## 7. Delivery KPIs

- Requirement traceability coverage.
- Test coverage and pass rate.
- Milestone adherence.
- Cost variance and forecast.
- Critical open defects.
- AI evaluation performance.
- Critical scenario escalation performance.
- Human review completion.
- UAT acceptance.
- Operational handover completion.

Targets must be agreed before execution and supported by evidence.

## 8. Governance and Reporting

Weekly:
- Delivery status.
- Milestones.
- Risks and issues.
- Budget and forecast.
- Dependencies.
- Decisions required.

Fortnightly Steering Committee:
- Executive summary.
- RAG status.
- Schedule and cost.
- Scope changes.
- Critical risks.
- Decisions and escalations.
- Next milestones.

Retrospective:
- What went well?
- What did not go well?
- What should we change?
- What actions will we own?
- How will we measure improvement?

## 9. AI CDR Framework

Compliance:
- Regulatory screening.
- Evidence and source traceability.
- Privacy and specialist review.

Delivery:
- Requirements.
- Architecture.
- Integration.
- Testing and handover.

Risk:
- AI quality.
- Security and privacy.
- Human oversight.
- Monitoring and incident management.

CDR is a project-specific operating framework, not a formal regulatory standard.

## 10. Portfolio Evidence Standard

Do not claim a result until it has been demonstrated.

Distinguish:
- Planned.
- Configured.
- Tested.
- Accepted.
- Deployed.

All company information and test data in this portfolio are fictional and synthetic.
