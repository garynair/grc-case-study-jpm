**MODEL ANSWER — TASK 8: Create KRIs, KPIs and an Ongoing Monitoring Dashboard**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 8's required outputs. Multiple good answers are possible — what matters is that the required elements are present and the reasoning is supported by the case.*

## Model Metric Catalog

| **Type** | **Metric** | **Calculation** | **Target** | **Threshold** | **Owner** | **Frequency** |
|---|---|---|---|---|---|---|
| KPI | Asset inventory reconciliation completion | % of monthly reconciliations completed by due date | 100% | <100% | Asset Management | Monthly |
| KPI | MFA coverage | % of in-scope systems/users enrolled in MFA | 100% internet-facing; ≥99% overall | <100% internet-facing | IAM | Weekly |
| KPI | Internet-facing security review | % of registered web properties with a current annual review | 100% | <95% | Security Architecture | Monthly |
| KPI | Corrective actions closed on time | % of actions closed by agreed date | ≥95% | <90% | GRC | Monthly |
| KRI | Unmanaged assets | Count of discovered assets not in the managed inventory | 0 | >0 | CIO / Asset Management | Weekly |
| KRI | Overdue critical exceptions | Count of critical exceptions past due | 0 | >0 | CISO | Daily / Weekly |
| KRI | Internet-facing systems without MFA | Count of internet-facing systems not protected by MFA | 0 | >0 | IAM | Daily |
| KRI | Unapproved cross-zone firewall rules | Count of rules without current owner/business justification | 0 | >0 | Network Security | Monthly |

## Model One-Page Dashboard

| **Measure** | **Status** | **Result** | **Action** |
|---|---|---|---|
| Asset inventory coverage | Amber | Discovery found three unregistered assets; owners assigned. | Track to closure at next monthly cycle. |
| Internet-facing MFA coverage | Red | One critical exception remains open. | Restrict access until compensating control approved; notify CISO. |
| Critical exceptions past due | Red | One item exceeded its target date. | Executive escalation within 1 business day; track weekly. |
| Firewall review completion | Amber | 92% reviewed; target is 100%. | Assign owner and date; review at monthly control forum. |
| High-severity detection time | Green | Median 2.5 hours after new alert rules. | Continue monitoring; report trend. |
| Corrective actions on time | Green | 96% closed by due date. | Continue monitoring; report trend. |

## Escalation Rules

- Internet-facing system without MFA: notify CISO and risk owner immediately; restrict access until an approved compensating control is in place.
- Critical exception past due: executive escalation within one business day, with weekly tracking until closure.
- Unmanaged asset discovered: classify, assign an owner, and place it into the applicable control programs within two business days.
- Repeated threshold breach for two consecutive reporting periods: present to the Technology Risk Committee with a funded corrective plan.
