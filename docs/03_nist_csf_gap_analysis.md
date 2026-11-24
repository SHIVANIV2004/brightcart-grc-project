# 03. NIST CSF 2.0 Gap Analysis (Simulated)

> **Fictional exercise.** BrightCart is invented. Ratings and practices are made up for learning. Outcome IDs and wording come from the NIST CSF 2.0 Core (NIST CSWP 29).

## Purpose
Compare BrightCart's **Current Profile** with a **Target Profile**, find the gaps, and turn them into a prioritized plan. This follows the five-step process in NIST SP 1301.

| Step (SP 1301) | What was done here |
|---|---|
| 1. Scope | Whole company, focused on access, backups, vendors, incidents, training and governance |
| 2. Gather information | Findings F-001 to F-006, evidence log, control matrix, risk register, vendor questionnaire |
| 3. Create the Profile | 27 CSF outcomes selected and rated (workbook sheet **CSF Profile**) |
| 4. Analyze gaps, make an action plan | Gap = target rating minus current rating; plan below |
| 5. Implement and update | Actions tracked in the Remediation Tracker; re-rate at next assessment |

## Rating scale
| Rating | Meaning |
|---|---|
| 1 | Not achieved, or no evidence |
| 2 | Partly achieved |
| 3 | Largely achieved, with gaps |
| 4 | Achieved, with evidence |
| 5 | Continuously improved |
| Blank | Not assessed (no conclusion reached) |

Gap levels: **Large** = 2 or more points, **Small** = 1 point, **None** = 0.

## Results
| Measure | Value |
|---|---|
| Outcomes in profile | 27 |
| Outcomes rated | 23 |
| Not assessed | 4 (ID.RA-01, PR.PS-02, PR.PS-04, DE.CM-03) |
| Large gaps | 9 |
| Small gaps | 8 |
| No gap | 6 |
| Average gap (rated outcomes) | 1.1 points |

### The nine large gaps
| Outcome | Current | Target | Priority | Why |
|---|---|---|---|---|
| PR.DS-11 Backups created, protected, maintained, **tested** | 2 | 4 | High | No 2026 restoration test evidence (F-002) |
| PR.AA-05 Access permissions reviewed, least privilege | 2 | 4 | High | Late leaver removal (F-001); review lacks sign-off (F-003) |
| GV.SC-05 Supplier requirements in contracts | 2 | 4 | High | DPA has no breach-notification timeframe (F-004) |
| GV.SC-06 Due diligence before supplier relationships | 2 | 4 | High | Vendor approved after contract (F-004) |
| RS.MA-01 Incident response plan executed | 2 | 4 | High | Procedure has no timeframe; untested (F-005) |
| GV.OC-03 Legal, regulatory and contractual requirements understood | 2 | 4 | High | No obligations register; PCI scope unconfirmed |
| RC.RP-03 Backup integrity verified before restoring | 1 | 3 | Medium | No evidence of integrity checks |
| GV.OV-03 Risk management performance reviewed | 2 | 4 | Medium | No management review cadence |
| ID.AM-02 Inventory of software, services, systems | 2 | 4 | Medium | No maintained inventory |

### Strengths (no gap)
GV.RM-06 (standard risk method), GV.SC-04 (suppliers prioritized), ID.RA-05 and ID.RA-06 (risk register and tracked responses), PR.AA-01 (named admin accounts), PR.AA-03 (MFA, evidence is a point-in-time export).

## Prioritized action plan
| Order | Focus | Outcomes | Actions (tracker ID, or proposed) |
|---|---|---|---|
| 1 | Prove recoverability | PR.DS-11, RC.RP-03 | A-003, A-004 |
| 2 | Fix access removal and review | PR.AA-05 | A-002, A-005, A-006 |
| 3 | Tighten vendor onboarding and contracts | GV.SC-05, GV.SC-06, GV.SC-07 | A-007, A-008; apply the Supplier Target Profile |
| 4 | Make incident response repeatable | RS.MA-01, RS.CO-02 | A-009; run a tabletop exercise (proposed) |
| 5 | Confirm obligations | GV.OC-03 | Proposed: obligations register with Legal |
| 6 | Governance review cadence | GV.OV-03, GV.RM-02 | Proposed: quarterly review; risk appetite statement |
| 7 | Inventories | ID.AM-02, ID.AM-07 | Proposed: system and data inventory |
| 8 | Complete the unassessed areas | ID.RA-01, PR.PS-02, PR.PS-04, DE.CM-03 | Next assessment cycle |

Items marked "proposed" are not yet in the Remediation Tracker. They would need an owner and due date agreed with management before being added.

## Tier proposal (NIST SP 1302)
Tiers describe how rigorous risk governance and management practices are: Partial (1), Risk Informed (2), Repeatable (3), Adaptive (4). Leadership normally selects Tiers; the table is the analyst's proposal. Tiers are set at Function level, not Subcategory level.

| Function | Current | Proposed target | Reason |
|---|---|---|---|
| Govern | 2 | 3 | Policies exist, but no risk appetite statement or review cadence |
| Identify | 2 | 3 | Risk register works; inventories missing |
| Protect | 2 | 3 | Highest-impact risks sit here |
| Detect | Not assessed | 2 | Limited resources; revisit after assessment |
| Respond | 2 | 3 | Procedure untested; notification duties unclear |
| Recover | 1 | 3 | Recovery never proven |

Tier 4 (Adaptive) is not proposed: it would likely cost more than the risk justifies for a company of this size. NIST encourages higher Tiers when risks or mandates require them, or when cost-benefit supports it.

## Supplier requirements (NIST SP 1305)
The workbook sheet **Supplier Target Profile** lists CSF-based requirements for Tier 1 (High) suppliers: contract clauses, assessment before signature, MFA and named accounts, incident notification, backup integrity, and recovery communication. Informative references should be selected with the CSF 2.0 Reference Tool (NIST SP 1347); the sheet quotes references only where SP 1305 shows them.

## Limitations
- Simulated data; ratings are judgment, not measurements.
- Four outcomes were not assessed and are not counted as gaps.
- Tier selection and priorities would need leadership agreement.
- This is a CSF self-assessment aid. It is not a certification and not a statement of compliance with any law.
