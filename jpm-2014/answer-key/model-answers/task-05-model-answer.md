**MODEL ANSWER — TASK 5: Assess and Prioritize the Risks**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 5's required outputs. Multiple good answers are possible — what matters is that the required elements are present and the reasoning is supported by the case.*

**Risk Register (Score = Likelihood × Impact; 1–4 Low, 5–9 Moderate, 10–16 High, 17–25 Critical)**

| **ID** | **Risk** | **L** | **I** | **Score** | **Rating** | **Rationale** |
|---|---|---|---|---|---|---|
| R1 | Incomplete asset inventory | 4 | 5 | 20 | Critical | The missed asset demonstrates likely recurrence without systemic correction. |
| R2 | Untracked MFA exception | 5 | 5 | 25 | Critical | The event occurred and enabled initial access; customer exposure was severe. |
| R3 | Business-managed portal governance | 4 | 4 | 16 | High | Similar portals may exist and can create internet-facing gaps. |
| R4 | Insufficient network segmentation | 4 | 5 | 20 | Critical | Attackers reached ~90 servers and a large customer database. |
| R5 | Delayed detection | 4 | 4 | 16 | High | Six-to-eight week dwell time allowed broad access. |
| R6 | Coverage assurance weakness | 4 | 4 | 16 | High | Management can receive false assurance across multiple control programs. |

**Top-Three Priorities**

- Priority 1 — R2, untracked MFA exception: close all externally accessible MFA exceptions and apply compensating controls immediately.
- Priority 2 — R4, network segmentation: isolate internet-facing systems and remove unnecessary connectivity to customer-data zones.
- Priority 3 — R1, inventory completeness: establish reconciliation so other unknown assets are identified before they repeat this pattern.

**Internal Auditor Challenges (2 minimum)**

- Challenge: R1 likelihood could be 5 because one missed asset proves the process failed. Decision: kept at 4 — the number of other unknown assets is not established; raise to 5 if discovery finds widespread omissions.
- Challenge: R5 impact could be 5 given 83 million affected customer/business relationships. Decision: kept at 4 — contact data, not financial credentials, was accessed; raise to 5 if financial data or fraud is confirmed.

**Question Answers**

- Why are R2/R4 high or critical? Both directly enabled access and expansion of the breach and involved highly sensitive customer systems.
- Can two risks share a score but differ in urgency? Yes — active exploitation, regulatory deadlines, available quick fixes, and concentration risk can all change urgency independent of score.
- What evidence would change a score? New incidents, control testing results, discovery findings, data classification, financial-loss estimates, and threat intelligence.
