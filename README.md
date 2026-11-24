# BrightCart GRC Assessment (Educational Portfolio Project)

> **Disclaimer:** BrightCart is a **fictional** company. All people, vendors, data, scores, test results and evidence in this repository are **invented for learning**. Nothing here is a real assessment, and nothing here shows that any real organisation is compliant or non-compliant. Framework references are illustrative; verify them against the official publications.

## What this project is

A beginner-level Governance, Risk and Compliance (GRC) project that walks through a simulated Q3 2026 (1 Jul to 30 Sep) information-security assessment of a fictional online shop. It practises the core workflow of a GRC Analyst:

1. Understand the business and scope
2. Identify and score risks
3. Define and assess controls (design vs. operating effectiveness)
4. Request and evaluate evidence
5. Test a sample and record exceptions
6. Write factual findings
7. Track remediation to validated closure
8. Assess vendor risk
9. Report to management

## Scenario

BrightCart sells products online, has about 150 staff (office and remote), and holds customer contact details, order data, employee records and business documents. It uses a payroll provider, cloud storage, a payment processor and an email-marketing tool. Management wants a clearer view of its cybersecurity risks.

## Repository contents

| Folder / file | What it contains |
|---|---|
| `workbook/BrightCart_GRC_Workbook.xlsx` | Main deliverable: 15 sheets (risk register, control matrix, evidence log, sampling test, findings, remediation tracker, vendor risk, framework mapping, NIST CSF 2.0 profile, tier selection, supplier target profile, dashboard). Scores, ratings, overdue flags and dashboard counts are formulas. |
| `csv_exports/` | CSV copies of the key sheets so they preview on GitHub |
| `docs/01_scope_and_business_overview.md` | Business context, scope, stakeholders, assumptions, approach |
| `docs/02_risk_methodology.md` | 5x5 scoring method, thresholds, treatment options |
| `docs/03_nist_csf_gap_analysis.md` | NIST CSF 2.0 gap analysis: method, results, prioritized plan, tier proposal, supplier requirements |
| `policies/access_control_policy.md` | Sample policy (owner, scope, statements, exceptions, review) |
| `policies/offboarding_procedure.md` | Sample procedure linked to the policy |
| `policies/acceptable_use_policy.md` | Sample one-page acceptable-use policy |
| `reports/assessment_report.md` | Scope, results, six findings, limitations |
| `reports/management_summary.md` | One-page summary for leadership |
| `reports/evidence_request_example.md` | Sample evidence request message |

## Headline results (simulated)

| Metric | Value |
|---|---|
| Risks registered | 10 (2 Critical, 6 High, 1 Medium, 1 Low, inherent) |
| Controls in matrix | 13 (3 effective, 7 need improvement, 1 design only, 2 not assessed) |
| Findings | 6 (2 High, 3 Medium, 1 Low) |
| Offboarding sample test | 3 exceptions in 10 sampled leavers |
| Remediation actions | 10 (1 closed and validated, 1 overdue as of 2026-11-02) |
| NIST CSF 2.0 profile | 27 outcomes: 23 rated, 4 not assessed, 9 large gaps |
| CSF Tier proposal | Current Tier 1 to 2 (Detect not assessed); proposed target Tier 3 for five Functions |

## Skills demonstrated

- Qualitative risk assessment (likelihood x impact), inherent vs. residual risk, risk treatment
- Control design vs. operating effectiveness; preventive, detective, corrective controls
- Evidence evaluation: what each item proves and does not prove
- Sampling and exception testing with Excel formulas (`NETWORKDAYS`, `COUNTIF`, `INDEX/MATCH`)
- Finding writing (condition, criteria, impact, root cause, recommendation)
- Remediation tracking with validation before closure
- Third-party risk tiering and questionnaire validation
- Mapping controls to NIST CSF 2.0, ISO/IEC 27001:2022, CIS Controls v8, SOC 2 and PCI DSS (illustrative)
- NIST CSF 2.0 Current vs Target Profile, gap analysis and prioritized action plan (SP 1301)
- CSF Tier selection and justification (SP 1302)
- Supplier requirements by criticality using a CSF Target Profile (SP 1305)
- Policy and procedure drafting; management reporting

## How to use the workbook

1. Open `workbook/BrightCart_GRC_Workbook.xlsx` and start with the **About** and **Methodology** sheets.
2. Yellow cells are inputs (for example the as-of date and rating thresholds). Change them and watch ratings and overdue flags update.
3. Read the **Findings** sheet, then follow each finding back to its control, evidence and risk using the IDs (R-, C-, EV-, F-, A-).
4. Open **CSF Profile** to see the same findings expressed as NIST CSF 2.0 outcomes with current and target ratings.

## Honest limitations

- All data and results are simulated; the sample is small and judgmental.
- No real systems were tested and no legal advice is given.
- Framework mappings are for organisation only, not proof that any requirement is met.
- Rating thresholds and scales are illustrative; a real organisation defines its own.

## Author

[SHIVANI VELUMANI] | [https://www.linkedin.com/in/shivanivelumani/] | Built as a learning exercise.
