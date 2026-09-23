**MODEL ANSWER MASTER REFERENCE — TASKS 1–9**

**JPMorgan Chase 2014 Cyber Incident | GRC Case Study**

*Combined instructor answer key across the full nine-task simulation*

# 1. Purpose

This is the single reference version of what a strong answer looks like at every stage of the simulation, Task 1 through Task 9. Each task's model answer stands on its own and is summarized here in sequence so instructors can grade against one consistent standard, and so capstone presenters can be coached against the intended answer. Multiple good answers are possible for each task; what matters is that the required elements are present and reasoning is supported by the case.

# 2. The Governance Thread (One Story, Nine Tasks)

One sentence per task shows how the model answers build a single argument: the breach was a governance-completeness failure, not a technology failure.

| **Task** | **One-Line Thread** |
|---|---|
| T1 | Establish the facts: an unmanaged microsite, no MFA, ~90 servers, 76M/7M records, no financial data confirmed stolen. |
| T2 | Timeline + stakeholders show two missed-intervention points: the MFA/inventory gap and the segmentation gap. |
| T3 | Asset inventory + control scope prove the omission was structural, not a one-off oversight. |
| T4 | Six risk statements convert the gaps into cause-event-impact risks with named owners. |
| T5 | Scoring puts three risks at Critical (R1, R2, R4) and prioritizes MFA exception closure first. |
| T6 | Framework mapping shows Identify/Protect were Partial while Detect/Respond/Recover were Effective. |
| T7 | 30-60-90 day plan, exception register, and RACI turn findings into owned, dated actions. |
| T8 | KRIs/KPIs make the same gaps visible on an ongoing basis, not just at audit time. |
| T9 | Tabletop + executive report translate the whole chain into time-bound decisions and one 5-minute briefing. |

# 3. Task-by-Task Model Answer Summary

## Task 1 — Case Fact Sheet

150-word case summary, five investigation questions (asset ownership/approval, why excluded from inventory, whether a formal exception existed, segmentation gaps, why detection took 6-8 weeks), and a fact-vs-assumption table. Confirmed: 76M households + 7M small businesses; names/addresses/phones/emails only. Not confirmed: account data, passwords, SSNs, financial data.

## Task 2 — Incident Timeline & Stakeholders

7-event timeline (Spring 2014 recon → Nov 2015 DOJ indictments) and an 8-plus stakeholder map spanning CISO, SOC, Asset Owner, IAM, Network Engineering, CRO, Legal, FBI, SEC, and customers. Two missed-intervention points: MFA/CMDB validation before rollout closure, and DMZ isolation with least-privilege access to customer-data environments.

## Task 3 — Asset Inventory & Control Scope

Six-asset inventory (microsite shaded as the MFA omission). Control-scope statements: MFA is mandatory for all internet-facing systems based solely on exposure, not criticality; vulnerability management covers all connected assets, enrolled at connection time. Four completeness checks: CMDB-to-discovery reconciliation, control-enrollment cross-check, owner-verification sampling, and a pre-launch security gate.

## Task 4 — Risk Statements

| **ID** | **Risk Statement (abridged)** | **Owner** | **CIA** |
|---|---|---|---|
| R1 | Incomplete inventory omits internet-facing systems from security programs | CIO / Tech Risk Exec | C,I,A |
| R2 | Untracked MFA exceptions let stolen-credential attackers in | CISO / Head of Identity Security | C,I |
| R3 | Business-managed microsites launch outside security governance | Business Unit Executive | C,I,A |
| R4 | Weak segmentation lets a low-criticality server reach customer systems | Head of Network Security | C,I,A |
| R5 | Monitoring gaps let attackers stay undetected for weeks | SOC Director | C,I |
| R6 | Coverage measured by spend/tools, not actual control reach | CISO / Enterprise Risk Committee | All |

## Task 5 — Risk Assessment & Prioritization

Score = Likelihood x Impact, 1-4 Low / 5-9 Moderate / 10-16 High / 17-25 Critical.

| **ID** | **L** | **I** | **Score** | **Rating** |
|---|---|---|---|---|
| R1 Inventory | 4 | 5 | 20 | Critical |
| R2 MFA exception | 5 | 5 | 25 | Critical |
| R3 Portal governance | 4 | 4 | 16 | High |
| R4 Segmentation | 4 | 5 | 20 | Critical |
| R5 Delayed detection | 4 | 4 | 16 | High |
| R6 Coverage assurance | 4 | 4 | 16 | High |

Top 3 priorities: (1) R2 MFA exception closure, (2) R4 segmentation/isolation, (3) R1 inventory reconciliation. Two auditor challenges resolved: R1 likelihood held at 4 (not enough evidence of widespread omission yet); R5 impact held at 4 (contact data, not financial data, was exposed).

## Task 6 — Framework Mapping

| **NIST CSF Function** | **Rating** | **Rationale (abridged)** |
|---|---|---|
| Identify | Partial / Gap | Inventory incomplete; microsite and its connectivity path excluded |
| Protect | Partial / Gap | MFA broadly deployed but not on the breached server; weak segmentation |
| Detect | Adequate | Detected in 6-8 weeks — better than industry average, still too slow |
| Respond | Effective | Forensics, law enforcement, containment all executed |
| Recover | Effective | No financial credentials confirmed stolen; controls restored |

Four regulatory mappings cited: FFIEC cyber risk management, FFIEC authentication guidance, GLBA Safeguards Rule, OCC Heightened Standards. Conclusion: the gap was incomplete implementation and insufficient assurance, not absence of a program.

## Task 7 — Corrective Action & Exception Management

30-60-90 day plan (disable/enforce MFA and reconcile inventory in 0-30d; register web properties and review firewall rules in 31-60d; institutionalize reconciliation, exception governance, and independent testing in 61-90d). Model exception-register entry (EX-2014-001, MFA gap, 30-day due date, CISO/Business Exec/Tech Risk approvers). RACI matrix across register/assess/approve/implement/validate steps. Residual risk: R-02 reduces from Critical (20) to Moderate (target 8), accepted only with Internal Audit validation and CISO or Board sign-off.

## Task 8 — KRIs, KPIs & Monitoring Dashboard

| **Type** | **Metric** | **Target** | **Owner** |
|---|---|---|---|
| KPI | Asset inventory reconciliation completion | 100% | Asset Management |
| KPI | MFA coverage | 100% internet-facing | IAM |
| KRI | Unmanaged assets discovered | 0 | CIO / Asset Mgmt |
| KRI | Overdue critical exceptions | 0 | CISO |
| KRI | Internet-facing systems without MFA | 0 | IAM |

Escalation rules: any internet-facing system without MFA notifies the CISO immediately; a critical exception past due escalates to executives within 1 business day; two consecutive threshold breaches go to the Technology Risk Committee with a funded plan.

## Task 9 — Tabletop & Executive Presentation

Four-inject decision log (unusual login → disable/isolate immediately; lateral connections found → segment and notify CISO within 4 hours; customer-DB access confirmed → engage Legal/Privacy/regulators same day; no financial data confirmed → communicate accurately, no overstatement). Communication matrix across six audiences (Board, Legal/Compliance, SEC, FBI, Employees, Customers) with timing and approval chain for each. One-page executive report and a 5-minute Risk Committee outline: opening, situation/impact, root cause, actions, decisions needed, close. Core lesson: security capability does not create assurance unless governance confirms complete control coverage across every in-scope asset.

# 4. Consolidated Scoring & Compliance Reference

| **Risk** | **Inherent Score** | **NIST CSF** | **Key Regulatory Reference** |
|---|---|---|---|
| R1 Inventory | 20 Critical | IDENTIFY — Partial | FFIEC cyber risk mgmt; OCC Heightened Standards |
| R2 MFA exception | 25 Critical | PROTECT — Partial | FFIEC authentication guidance; GLBA Safeguards |
| R3 Portal governance | 16 High | IDENTIFY / GOVERN | OCC Heightened Standards |
| R4 Segmentation | 20 Critical | PROTECT — Partial | FFIEC Information Security Booklet |
| R5 Detection latency | 16 High | DETECT — Adequate | FFIEC CAT Domain 5 |
| R6 Coverage assurance | 16 High | GOVERN | OCC Heightened Standards |

# 5. Using This Reference for Capstone Presentation Prep

Each capstone presenter's section should be checked against the matching task(s) below, since this is the standard the presentation is graded against.

| **Role** | **Model-Answer Tasks to Reconcile Against** | **What "Conformant" Looks Like** |
|---|---|---|
| S1 — GRC Coordinator | T1, T9 (executive framing) | Opinion is source-grounded; distinguishes fact from assumption |
| S2 — Asset & Control Analyst | T2, T3, T4 (R1/R3) | Inventory and control-scope checks are traceable to case evidence |
| S3 — Risk Analyst | T4, T5 | Cause-event-impact form; correct L x I scoring against the assigned thresholds |
| S4 — Compliance & Controls Analyst | T6 | Function ratings and regulatory citations match the case's actual gaps |
| S5 — Incident & Communications Analyst | T2 (stakeholders), T7 (Sec.4), T9 | Escalation timing and audience-specific messaging are time-bound |
| S6 — Internal Auditor | T5 (challenge log), T7 (residual risk) | Challenges are evidenced, not asserted; residual risk has a named acceptance authority |
