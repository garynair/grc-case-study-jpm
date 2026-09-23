**MODEL ANSWER — TASK 4: Identify Risks and Write Clear Risk Statements**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 4's required outputs. Multiple good answers are possible — what matters is that the required elements are present and the reasoning is supported by the case.*

**Risk Register — Identification Stage (formula: Because of [cause], there is a possibility that [event], resulting in [impact])**

| **ID** | **Risk Statement** | **Control Gap** | **Risk Owner** | **CIA** |
|---|---|---|---|---|
| R1 | Because the asset inventory is incomplete, internet-facing systems may be omitted from mandatory security programs, resulting in unauthorized access, data exposure, regulatory criticism and reputational harm. | Asset inventory & reconciliation | CIO / Technology Risk Executive | C, I, A |
| R2 | Because MFA exceptions are not formally tracked and escalated, attackers using stolen passwords may access corporate systems, resulting in account compromise and unauthorized network entry. | MFA coverage & exception management | CISO / Head of Identity Security | C, I |
| R3 | Because business-managed microsites are commissioned outside standard security governance, vulnerable internet-facing systems may be launched or retained, resulting in an expanded attack surface and control noncompliance. | Secure onboarding & web-property registration | Business Unit Executive | C, I, A |
| R4 | Because network segmentation and cross-zone access controls are insufficient, an attacker compromising a low-criticality web server may move to customer systems, resulting in large-scale data exposure and operational disruption. | Network segmentation & firewall governance | Head of Network Security | C, I, A |
| R5 | Because monitoring rules do not identify unusual authentication, lateral movement and bulk data access quickly enough, attackers may remain undetected for weeks, resulting in greater data loss and investigation cost. | Security logging, SIEM coverage & alerting | SOC Director | C, I |
| R6 | Because security program effectiveness is measured mainly by tools and spending rather than control coverage, management may receive false assurance, resulting in unaddressed exceptions and repeated control failures. | Coverage assurance & governance reporting | CISO / Enterprise Risk Committee | All |

**Question Answers**

- Is “no MFA” a risk or a control gap? It's a control gap. The risk is what could happen because the control is missing.
- What business impacts follow from an incomplete asset inventory? Missed patching, missed MFA, missed monitoring, unknown data exposure, compliance gaps, and delayed incident response.
- Why should business owners hold cybersecurity risk ownership? The business owner creates or uses the service, understands the business need and impact, and must accept or fund risk decisions — the executive owns the business risk while technical teams operate the controls.
