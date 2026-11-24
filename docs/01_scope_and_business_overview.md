# 01. Scope and Business Overview

*Fictional company. Educational use only.*

## Company profile
| Item | Detail |
|---|---|
| Company | BrightCart (fictional) |
| Business | Online shopping platform |
| Staff | About 150, office and remote |
| Growth | Rapid; documentation is inconsistent |
| Management goal | Clearer understanding of cybersecurity risks |

## Key systems and information
| Asset | Information | Classification |
|---|---|---|
| E-commerce platform | Orders, customer contact details | Confidential |
| Order and finance databases | Order history, financial records | Confidential |
| HR system | Employee records | Highly restricted |
| Cloud storage (CloudStore) | Business documents, order exports | Confidential |
| Email and collaboration | Internal and customer communication | Internal / Confidential |

## Critical business processes
Order placement and payment; order fulfilment; payroll; customer support.

## External providers
PayrollPro (payroll), CloudStore (cloud storage), PayGate (payment processing), MailBlast (email marketing). All fictional.

## Stakeholders
| Role | Interest |
|---|---|
| CFO | Financial risk, payment obligations |
| HR Director | Employee data, offboarding, payroll vendor |
| Head of Security | Access control, incidents, training |
| IT Manager | Accounts, patching, cloud configuration |
| Head of Infrastructure | Backups and recovery |
| Legal / Procurement | Contracts, privacy questions |
| GRC Analyst (author) | Coordinates assessment, documents risks, tracks actions |

## Scope
**In scope (1 Jul to 30 Sep 2026):** access management (offboarding, privileged access), backups, vendor risk, incident reporting, security awareness training, selected policies.
**Out of scope or not assessed:** patching (C-12), vendor contract clauses (C-09), cloud configuration operation (C-13), penetration testing, legal compliance conclusions.

## Applicable obligations (to be confirmed with Legal)
The analyst does not conclude that BrightCart is compliant with any law. Obligations may arise from customer contracts, payment-card requirements (PCI DSS, via payment processor), privacy laws in the places where customers and staff are located, and internal policies. Legal and privacy advisors should confirm which apply.

## Approach
1. Held scoping discussions with control owners (simulated).
2. Built an initial risk list as **hypotheses**, then scored with owners.
3. Listed controls and the evidence needed for each.
4. Requested evidence (see `reports/evidence_request_example.md`) and logged it.
5. Tested one control (offboarding) using a judgmental sample of 10 from 34 leavers.
6. Recorded findings with facts, criteria and impact, without assuming misuse.
7. Agreed actions with owners and tracked them; closed items only after validation.

## Assumptions
- Evidence provided is genuine; authenticity was not independently verified.
- Leaver population list from HR is complete (not independently verified).
- Dates, owners and ratings are illustrative and would be agreed with real stakeholders.
