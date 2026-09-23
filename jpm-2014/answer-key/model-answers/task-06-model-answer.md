**MODEL ANSWER — TASK 6: Map the Gaps to GRC Frameworks and Requirements**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 6's required outputs. Multiple good answers are possible — what matters is that the required elements are present and the reasoning is supported by the case.*

**NIST CSF Function-Level Assessment**

| **Function** | **Rating** | **Rationale** |
|---|---|---|
| Identify | Partial / Gap | The asset inventory was incomplete and did not include the microsite or its connectivity path. |
| Protect | Partial / Gap | MFA was broadly deployed but not applied to the breached server; segmentation and compensating controls were inadequate. |
| Detect | Adequate, needs improvement | Internal monitoring detected the breach in six to eight weeks — better than the historical industry average, but too late to prevent broad access. |
| Respond | Effective | The bank investigated, engaged forensics and law enforcement, contained the breach, and closed the vulnerability. |
| Recover | Effective | No financial credentials were confirmed stolen; the bank restored control and increased security investment. |

**Regulatory Mapping (4 requirements)**

| **Requirement** | **Case Implication** |
|---|---|
| FFIEC cyber risk management | Requires comprehensive asset and risk management; the omitted internet-facing server shows incomplete scope. |
| FFIEC authentication guidance | Supports MFA for high-risk and remote access; a single-factor internet-facing server was inconsistent with the expected control. |
| GLBA Safeguards Rule | Requires a comprehensive information-security program covering customer information systems; the access path to customer records showed a coverage gap. |
| OCC Heightened Standards | Large banks are expected to maintain strong front-line risk governance; the missed system and unmanaged exception indicate weak execution. |

**Evidence an Auditor Would Request**

- Asset inventory and asset-owner certification records; network discovery and inventory-reconciliation reports.
- MFA enrollment report and exception register; vulnerability scan and patch-compliance reports.
- Firewall diagrams, rules and approval records; SIEM log-source coverage and alert-use-case documentation.
- Incident tickets, forensic report and containment records; risk committee minutes and executive approvals; SEC filing and regulatory communication records.

**Compliance Conclusion**

The organization had mature capabilities and policies, but evidence shows material gaps in control coverage and exception governance. Identify and Protect were not fully effective because the inventory, MFA scope and segmentation controls did not cover every relevant system. Detect, Respond and Recover functioned more effectively, limiting the incident after discovery. The compliance concern is therefore not absence of a program, but incomplete implementation and insufficient assurance that mandatory controls applied to all in-scope assets.
