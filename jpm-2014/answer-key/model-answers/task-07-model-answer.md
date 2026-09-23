**MODEL ANSWER — TASK 7: Design the Corrective Action and Exception Management Plan**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 7's required outputs. Multiple good answers are possible — what matters is that the required elements are present and the reasoning is supported by the case.*

## Model 30-60-90 Day Corrective-Action Plan

| **Window** | **Action** | **Owner** | **Evidence** |
|---|---|---|---|
| 0–30d | Disable/restrict the compromised access path; enforce MFA on the microsite; reset credentials; isolate the server; review all internet-facing MFA exceptions. | CISO, IAM, Network Security | MFA coverage report, firewall change, incident ticket, exception list |
| 0–30d | Run discovery of all internet-facing assets and reconcile against the asset inventory. | Infrastructure Asset Mgmt | Discovery report, unmatched-asset log |
| 31–60d | Register every web property; assign a business and a technical owner; classify data and connectivity. | Business Technology Governance | Approved inventory, owner certifications |
| 31–60d | Review cross-zone firewall rules; remove unjustified paths from internet-facing systems to customer-data zones. | Network Security | Approved rule review, updated diagram |
| 31–60d | Implement SIEM alerts for unusual authentication, lateral movement, and bulk data access. | SOC Engineering | Use-case test results, alert tickets |
| 61–90d | Establish monthly inventory reconciliation and quarterly business certification. | CIO / GRC | Operating procedure, dashboard, first completed review |
| 61–90d | Implement formal exception governance with aging thresholds and executive escalation. | CISO / Technology Risk | Exception policy, register, committee minutes |
| 61–90d | Independent test of MFA, asset coverage, and segmentation actions — by a function separate from the implementer. | Internal Audit / 2nd-Line Risk | Validation report, closure recommendation |

## Model Exception-Register Entry

| **Field** | **Response** |
|---|---|
| ID | EX-2014-001 |
| Control / Asset | MFA required for internet-facing corporate systems  —  Corporate Challenge microsite server |
| Reason | Legacy application not integrated with the enterprise MFA rollout |
| Owner | Corporate Events Technology Owner |
| Risk | A stolen password could permit unauthorized entry and lateral movement |
| Compensating Controls | Restrict access by source IP; monitor every login; disable unnecessary accounts; isolate the network segment; daily log review |
| Due Date / Status | Within 30 days  —  Open, Critical |
| Approvers | Business Executive, CISO, and Technology Risk |
| Escalation | Immediate CISO notification; executive approval required if not closed by the due date |
| Closure Evidence | MFA test result, updated inventory entry, access review, and independent validation sign-off |

## Model RACI Matrix

| **Activity** | **Responsible** | **Accountable** | **Consulted** | **Informed** |
|---|---|---|---|---|
| Register new asset | Business owner | Business executive | Asset Mgmt, Security | GRC, Internal Audit |
| Assess required controls | Security Architecture | CISO delegate | Business owner, Privacy | GRC |
| Approve exception | GRC (prepares) | CISO / Business exec. | Legal, Risk owner | Internal Audit |
| Implement remediation | Technical control owner | Risk owner | GRC, Vendor | Executive management |
| Validate closure | 2nd-Line Risk / Internal Audit | Chief Risk / Audit authority | Control owner | Risk Committee |

## Residual-Risk Statement

After MFA enforcement, segmentation, inventory reconciliation, and monitoring improvements, the unmanaged-exception risk (R-02) may reduce from Critical (inherent 20) to Moderate (target residual 8: likelihood 2, impact 4). The business risk owner may accept the remaining exposure only after independent validation by Internal Audit or second-line Risk, and documented approval by the CISO or, where the residual sits outside the stated tolerance threshold, the Board Risk Committee on a time-limited, non-renewable acceptance.
