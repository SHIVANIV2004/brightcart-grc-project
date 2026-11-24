# BrightCart Information Security Assessment Report (Simulated)

> **Fictional exercise.** All results are invented for learning and do not describe a real organisation.

| Field | Detail |
|---|---|
| Assessment period | 2026-07-01 to 2026-09-30 |
| Fieldwork | 2026-10-05 to 2026-10-23 |
| Report date | 2026-10-26 (status as of 2026-11-02) |
| Prepared by | [Your Name], GRC Analyst (learner) |

## 1. Objective and scope
Evaluate selected controls over access management, backups, vendor risk, incident reporting and security awareness, and document risks, findings and corrective actions. See `docs/01_scope_and_business_overview.md`.

## 2. Method
- Risk scoring: 5x5 likelihood x impact (`docs/02_risk_methodology.md`).
- Control assessment: design and operating effectiveness reviewed separately.
- Evidence: requested through an evidence log; each item records what it does and does not demonstrate.
- Testing: judgmental sample of 10 from 34 leavers for the offboarding control.

## 3. Summary of results
| Area | Result |
|---|---|
| Risks | 10 registered: 2 Critical, 6 High, 1 Medium, 1 Low (inherent) |
| Controls | 13 listed: 3 effective, 7 need improvement, 1 design only, 2 not assessed |
| Findings | 6: 2 High, 3 Medium, 1 Low |
| Offboarding test | 3 of 10 sampled leavers exceeded the 1-business-day SLA |
| Remediation | 10 actions: 1 closed and validated, 1 overdue, 8 in progress or open |

## 4. Findings

### F-001 (High): Access not removed within SLA for 3 of 10 sampled leavers
- **Criteria:** Access Control Policy s5.3: access removed within 1 business day of termination.
- **Condition:** 7 of 10 sampled leavers were disabled within the SLA. Two were disabled after 2 and 10 business days. One account was still active at the test date (2026-10-12).
- **Evidence:** EV-002, EV-003.
- **Impact:** Former employees could retain access. No evidence reviewed shows the accounts were used after termination; activity logs were not reviewed.
- **Root cause:** Under investigation. HR notifies IT by email with no ticket or tracking.
- **Recommendation:** Disable remaining access (done, A-001). Link HR ticket to an IT task with the SLA. Reconcile weekly. Review activity logs for the 3 accounts.
- **Owner / target:** IT Manager and HR Manager / 2026-12-15.

### F-002 (High): No evidence of backup restoration testing in 2026
- **Criteria:** Backup Procedure v1.1: restoration tests at least every six months.
- **Condition:** No 2026 restoration test records provided. Backup job reports show successful jobs but do not show recoverability.
- **Impact:** Recoverability is unverified. This does not state that backups are unrecoverable.
- **Recommendation:** Perform and document a restoration test; add tests to a compliance calendar.
- **Owner / target:** Head of Infrastructure / 2026-11-30.

### F-003 (Medium): Q3 privileged access review lacks sign-off and outcomes
- **Criteria:** Access Control Policy s6.2.
- **Condition:** Review list exported 2026-09-12 with 4 accounts marked "to review"; no sign-off or outcomes provided.
- **Impact:** Unnecessary privileged access may persist; extent unknown.
- **Recommendation:** Document outcomes; add sign-off and reminder workflow.
- **Owner / target:** Head of Security / 2027-01-31.

### F-004 (Medium): Payroll vendor approved after contract start; data feed not minimised
- **Criteria:** Vendor Risk Procedure: approval before contract signature; collect only necessary data.
- **Condition:** Contract signed 2026-03-02; approval dated 2026-04-20. Feed includes fields not needed for payroll. DPA excerpt has no breach-notification timeframe.
- **Impact:** Greater exposure of employee personal data if the vendor is compromised.
- **Recommendation:** Remove unneeded fields; seek DPA update (Legal to advise); add approval gate before signature.
- **Owner / target:** Vendor risk owner (HR Director) / 2027-01-15.

### F-005 (Medium): Incident reporting procedure lacks a reporting timeframe
- **Criteria:** Security Policy s8: report suspected incidents promptly.
- **Condition:** Procedure v1.0 does not define "promptly" or an out-of-hours contact.
- **Impact:** Delayed response is possible; actual delays were not tested.
- **Recommendation:** Define timeframe and contact in v2.0; brief staff; test next cycle.
- **Owner / target:** Head of Security / 2026-12-04.

### F-006 (Low): Security awareness training completion below target
- **Criteria:** Security Awareness Standard: 95% completion by 30 Sep.
- **Condition:** 126 of 150 employees (84%) completed training.
- **Recommendation:** Reminders and manager escalation until 95% is reached.
- **Owner / target:** Head of Security / HR Manager / 2026-11-30.

## 5. Strengths observed
- Individual admin accounts mapped to named owners (C-04).
- MFA configuration enforced for admin and remote access at the time of export (C-05).
- Daily backup jobs monitored with failures ticketed (C-06).
- A leaver account found active was disabled and validated (A-001).

## 6. Limitations
- Simulated scenario; small judgmental sample; no real system testing.
- Evidence authenticity and population completeness were not independently verified.
- Patching, vendor contract clauses and cloud configuration were not assessed.
- No legal conclusions are made. Applicable legal and contractual requirements should be confirmed by qualified advisors.
- Framework mappings are illustrative and do not prove compliance.

## 7. Next steps
Owners complete actions by agreed dates; the GRC Analyst validates evidence before closure; a follow-up assessment covers C-09, C-12 and C-13.
