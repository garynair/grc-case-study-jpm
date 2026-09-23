**MODEL ANSWER — TASK 3: Create an Asset Inventory and Define Control Scope**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 3's required outputs. Multiple good answers are possible — what matters is that the required elements are present and the reasoning is supported by the case.*

**Asset Inventory (6-minimum; shaded item = MFA omission)**

| **Asset** | **Business Owner** | **Technical Owner** | **Data Handled** | **Internet?** | **Applicable Controls** |
|---|---|---|---|---|---|
| Corporate Challenge Microsite | Corporate/Community Affairs | IT Web Services | Event registration info (low sensitivity) | Yes | MFA: MISSING (root cause). Patch status unconfirmed. |
| Customer Online/Mobile Banking | Retail Banking | Digital Channels IT | Customer PII, account/transaction data | Yes | MFA, encryption, continuous monitoring |
| Customer Contact Database | Consumer & Community Banking | Database/Infra Team | Names, addresses, phone, email (~76M/7M) | No | Access control, encryption at rest, segmentation |
| Active Directory / IAM System | Information Security | IAM Team | Credentials, access entitlements | No | Privileged access mgmt, admin MFA, logging |
| Enterprise Network / DMZ | IT Infrastructure | Network Engineering | N/A (infrastructure) | Partial (DMZ) | Segmentation, firewall rules, IDS/IPS |
| SIEM / Security Monitoring | CISO / Info Security | Security Operations Center | Logs, security events | No | Log retention, correlation rules, alerting |

**Control-Scope Statement — MFA**

All internet-facing systems are in scope for mandatory multi-factor authentication, without exception, based solely on internet exposure — not business criticality, asset type, or sponsoring department. Any exception requires documented, time-bound risk acceptance approved by Information Security leadership and tracked to an expiration date.

**Control-Scope Statement — Vulnerability Management**

All assets connected to the corporate network — internet-facing or internal — are in scope for recurring vulnerability scanning and timely patching, prioritized by exploitability and network exposure. Newly registered assets are enrolled at the time of network connection, not at the next scheduled review cycle.

**Four Inventory Completeness Checks**

- CMDB-to-discovery reconciliation: run automated network/DNS discovery monthly and reconcile against the CMDB; every discrepancy gets a named owner and risk decision within 5 business days.
- Control-enrollment cross-check: cross-reference the MFA enrollment list and vulnerability-scan inventory against the full CMDB — any asset in one list but not another is an open exception.
- Owner-verification sampling: periodically contact a sample of listed owners and confirm they can identify their asset — catches stale or incorrect ownership records.
- Pre-launch gate: require a security checklist (registration, MFA, vuln-scan enrollment) before any new internet-facing asset goes live — prevents a repeat of the Corporate Challenge gap at the source.
