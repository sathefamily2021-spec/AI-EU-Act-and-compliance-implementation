
# Business Requirements Document (BRD)

**Project:** Enterprise AI Governance Readiness Workbench  
**Document ID:** BRD-001  
**Version:** 1.0  
**Status:** Draft for stakeholder validation  
**Business owner:** AI Governance Lead  
**Delivery owner:** AI Implementation Project Manager  
**Classification:** Fictional portfolio simulation

---

## 1. Business Background

The organisation operates 15 AI systems across several business functions.

AI system information, ownership, supplier documentation, risk assessments and approval evidence are not consistently maintained in one location.

The organisation requires a repeatable process to collect information, identify potential regulatory and operational risks, assign specialist reviews and monitor remediation actions.

The proposed solution is an AI Governance Readiness Workbench.

## 2. Problem Statement

The current simulated process has five key problems:

1. AI system information is fragmented.
2. Assessment questions differ between departments.
3. Potential risk indicators are not consistently escalated.
4. Evidence and decisions are difficult to trace.
5. Management cannot easily see outstanding governance actions.

The project will address these problems through a structured workflow supported by AI-assisted analysis.

## 3. Business Outcomes

| Outcome | Measurement |

| Centralised AI inventory | 15 of 15 systems registered |
| Consistent intake | 100% of submissions use standard fields |
| Evidence visibility | Every assessment has an evidence status |
| Review accountability | Every case has a named reviewer |
| Risk visibility | Open risks and overdue actions are reported |
| Assessment quality | AI outputs evaluated against a human-reviewed test set |

Targets are proposed acceptance criteria, not achieved business results.

## 4. Stakeholder Needs

### CIO — Executive Sponsor
Needs:
- Consolidated programme status.
- Significant risks and decisions.
- Budget and delivery progress.
- Confidence in governance controls.

### AI Governance Lead — Business Owner
Needs:
- Central AI system inventory.
- Consistent assessment process.
- Risk and action visibility.
- Review and approval tracking.

### Legal / Compliance
Needs:
- Relevant regulatory questions.
- Traceable evidence and references.
- Clear distinction between preliminary screening and legal conclusions.
- Ability to review and correct AI-generated outputs.

### Data Protection Officer
Needs:
- Personal data processing information.
- Purpose and data-category details.
- DPIA screening indicators.
- Ability to request further information.

### CISO
Needs:
- Data flows and hosting details.
- Supplier and access information.
- Security review status.
- Incident and control information.

### Business System Owner
Needs:
- Simple intake form.
- Clear responsibilities.
- Ability to submit supporting documents.
- Visibility of review actions and decisions.

## 5. User Personas

| Persona | Main activity |

| System Owner | Submits AI system information |
| AI Governance Analyst | Reviews preliminary assessments |
| Legal Reviewer | Reviews regulatory questions |
| DPO | Reviews privacy concerns |
| Security Reviewer | Reviews security concerns |
| AI Governance Lead | Approves internal governance decisions |
| CIO | Reviews management dashboard |

## 6. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR-001 | User can register an AI system | Must |
| FR-002 | System captures owner and business purpose | Must |
| FR-003 | System captures provider, deployer and supplier details where known | Must |
| FR-004 | System captures intended use and affected people | Must |
| FR-005 | System captures data categories and processing details | Must |
| FR-006 | AI can generate a preliminary assessment from submitted information | Must |
| FR-007 | AI must identify missing or contradictory information | Must |
| FR-008 | Assessment must identify supporting evidence and sources | Must |
| FR-009 | Potential prohibited-practice indicators must trigger specialist escalation | Must |
| FR-010 | Potential high-risk indicators must be flagged for human review | Must |
| FR-011 | Privacy concerns must be routed to the DPO | Must |
| FR-012 | Security concerns must be routed to the CISO | Must |
| FR-013 | Users can record human review decisions | Must |
| FR-014 | System maintains an assessment history | Must |
| FR-015 | Management can view inventory and outstanding actions | Should |
| FR-016 | System can export an assessment summary | Should |

## 7. Non-Functional Requirements

| ID | Requirement | Proposed acceptance test |
|---|---|---|
| NFR-001 | Security | No API secrets exposed in repository |
| NFR-002 | Privacy | Synthetic data used in demonstration |
| NFR-003 | Traceability | Each assessment has a unique identifier |
| NFR-004 | Explainability | AI output includes rationale and evidence references |
| NFR-005 | Human oversight | No automatic final legal approval |
| NFR-006 | Reliability | Failed requests produce a visible error status |
| NFR-007 | Usability | Business user can complete intake without technical support |
| NFR-008 | Maintainability | Rules and prompts are version-controlled |
| NFR-009 | Auditability | Review status and decisions are recorded |
| NFR-010 | Performance | Prototype target: assessment response within 60 seconds under defined test conditions |

## 8. AI-Specific Requirements

The AI component must:

1. Use approved regulatory reference material.
2. Distinguish facts supplied by users from inferred information.
3. Avoid inventing legal articles or obligations.
4. Cite supporting sources where available.
5. Return an uncertainty or insufficient-information status.
6. Identify potential issues for human review.
7. Never make a final legal compliance determination.
8. Maintain a version identifier for its prompt and assessment rules.
9. Be evaluated against a fixed test dataset.
10. Allow human reviewers to record corrections.

## 9. Business Rules

BR-001: Every AI system must have a unique inventory ID.

BR-002: An assessment cannot be marked complete when mandatory information is missing.

BR-003: A potentially prohibited practice indicator must be escalated to Legal/Compliance.

BR-004: A potential high-risk classification must be reviewed by an authorised specialist.

BR-005: A GDPR DPIA decision must be made by the accountable privacy function, not the AI assistant.

BR-006: Supplier documentation gaps must be recorded as actions.

BR-007: Final internal governance approval must be recorded by an authorised human.

BR-008: All unresolved critical issues must remain visible in the management report.

## 10. User Stories and Acceptance Criteria

### US-001: Register an AI System

As a System Owner, I want to submit information about an AI system so that it can be included in the central inventory.

Acceptance criteria:
- Unique ID is generated.
- Owner and intended purpose are captured.
- Required fields are validated.
- Submission is stored.
- Confirmation is displayed.

### US-002: Generate a Preliminary Assessment

As an AI Governance Analyst, I want an AI-generated preliminary assessment so that I can review potential risks efficiently.

Acceptance criteria:
- Assessment uses the submitted information.
- Missing information is listed.
- Relevant source references are displayed.
- Uncertainty is explicitly identified.
- Human review is required.

### US-003: Escalate a Potential Risk

As a Governance Analyst, I want potential high-impact or prohibited-practice indicators to be escalated so that specialists can assess them.

Acceptance criteria:
- The relevant issue is flagged.
- A reviewer role is identified.
- The case status becomes Review Required.
- No automatic final classification is made.

### US-004: Review and Approve

As an authorised reviewer, I want to record my decision and comments so that accountability is traceable.

Acceptance criteria:
- Reviewer identity is recorded.
- Decision and comments are stored.
- Date and assessment version are recorded.
- Changes remain traceable.

### US-005: View Management Status

As the CIO, I want a dashboard showing inventory, assessment status and outstanding actions so that I can oversee programme delivery.

Acceptance criteria:
- Total registered systems are visible.
- Assessment completion is visible.
- Open review actions are visible.
- Critical issues are highlighted.
- Dashboard data can be traced to underlying records.

## 11. Discovery Workshop Plan

**Workshop:** AI Governance Process Discovery  
**Duration:** 90 minutes  
**Facilitator:** AI Implementation Project Manager

Participants:
- AI Governance Lead
- Legal / Compliance
- DPO
- CISO
- Business System Owners
- Data / AI Specialist

Agenda:

| Time | Activity |
|---|---|
| 0–10 min | Objectives and introductions |
| 10–25 min | Current-state process mapping |
| 25–45 min | Pain points and root-cause analysis |
| 45–60 min | Future-state workflow |
| 60–70 min | Risk and control discussion |
| 70–80 min | Requirements prioritisation |
| 80–90 min | Decisions, owners and next steps |

Facilitation techniques:
- Open-ended questioning.
- Process mapping.
- Five Whys for root-cause analysis.
- MoSCoW prioritisation.
- Parking lot for out-of-scope items.
- Decision and action log.

## 12. Requirements Prioritisation

MoSCoW:

- Must: essential for a working and safe prototype.
- Should: important but not essential for the first demonstration.
- Could: useful enhancement.
- Won't: excluded from the current release.

Mandatory legal and safety controls cannot be deprioritised merely because of a scoring exercise.

## 13. Requirement Traceability

Every requirement will be connected to:
- A business objective.
- A user story.
- A design component.
- An implementation task.
- A test case.
- A result or defect.
- An acceptance decision.

## 14. Definition of Done

A requirement is complete only when:
- It is implemented or explicitly marked as not implemented.
- The relevant test has passed.
- Evidence is recorded.
- Any defect is documented.
- The business owner has reviewed the result.
- The requirement is traceable to the agreed scope.

## 15. Open Decisions

| ID      | Decision required                         | Owner |                 Status |

| DEC-001 | Confirm approved regulatory source library | Legal                     Open |
| DEC-002 | Confirm mandatory intake fields            | AI Governance Lead       | Open |
| DEC-003 | Confirm human approval roles | CIO / Governance Lead                   | Open |
| DEC-004 | Confirm data retention policy | DPO                                    | Open |
| DEC-005 | Confirm prototype hosting approach        | Technical Lead             | Open |

---

**Document owner:** AI Implementation Project Manager  
**Version:** 1.0  
**Approval:** Simulated draft — stakeholder validation pending
