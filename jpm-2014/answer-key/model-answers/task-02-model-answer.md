**MODEL ANSWER — TASK 2: Build the Incident Timeline and Identify Stakeholders**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 2's required outputs. Multiple good answers are possible — what matters is that the required elements are present and the reasoning is supported by the case.*

**Incident Timeline (7-event minimum)**

| **Date/Period** | **Event** | **Category** | **Why It Matters** |
|---|---|---|---|
| Spring 2014 | Reconnaissance of internet-facing infrastructure; Corporate Challenge microsite identified | Attack activity | Shows attackers scanned for assets outside standard security coverage |
| Mid-June 2014 | Initial access via compromised credentials on the MFA-excluded server | Attack activity | Root-cause control gap: one unmanaged asset became the entry point |
| Jun–Jul 2014 | Lateral movement to ~90 servers; contact data for 76M/7M accessed | Attack activity | Reflects weak segmentation between the DMZ and customer-data zones |
| Late July 2014 | Security team detects and confirms unauthorized access | Detection | ~6–8 weeks dwell time — the key monitoring-effectiveness metric |
| August 2014 | Access revoked, systems remediated (incl. accelerated MFA); FBI and regulators notified | Response | Containment speed/completeness determines residual attacker access |
| Early Oct 2014 | SEC Form 8-K filed; affected customers notified | Disclosure | Triggered once scope and materiality were confirmed with Legal |
| Nov 2015 | DOJ unseals indictments against those responsible | Legal follow-up | Closes the incident lifecycle; external validation of root cause |

**Stakeholder Map (8-minimum, internal + external)**

| **Stakeholder** | **Role / Decision Authority** | **Information Needed** | **Timing** |
|---|---|---|---|
| CISO (internal) | Approves/denies control exceptions; authorizes IR strategy | Exception register, risk dashboard, incident status | Immediate at detection |
| SOC (internal) | Escalates alerts; triggers IR playbook | SIEM alerts, auth logs, anomaly data | Continuous; immediate |
| Asset Owner / Infra (internal) | Approves onboarding; certifies inventory completeness | CMDB, exception requests, patch status | Ongoing pre-incident; post-incident remediation |
| IAM (internal) | Approves/rejects MFA coverage exceptions | MFA coverage reports, exception log | Ongoing; validated during remediation |
| Network Engineering (internal) | Approves segmentation/access-control design | Topology maps, firewall rules | Pre-incident design; active in containment |
| CRO / Enterprise Risk (internal) | Accepts, mitigates, or escalates residual risk | Risk register, KRIs, control-effectiveness data | Escalation within 24–48 hrs |
| Legal / General Counsel (internal) | Determines disclosure timing; authorizes law-enforcement contact | Breach scope, notification-law requirements | Immediate upon confirmed breach |
| FBI / Law Enforcement (external) | Independent authority over investigation | IOCs, forensic evidence | Promptly after detection |
| SEC / Regulators (external) | Independent authority to require disclosure | 8-K content, incident scope | Per statutory disclosure deadline |
| Affected Customers (external) | Informational recipient of notice | What data was affected; protective steps | At public disclosure |

**Two Missed-Intervention Points**

- MFA/asset-inventory gap: Infrastructure & IAM should have validated 100% MFA coverage against a continuously reconciled CMDB before closing the rollout — likely blocks initial access.
- Network segmentation: Network Engineering should have enforced DMZ isolation and least-privilege access to customer-data environments — delays or blocks attacker reach to customer data.

**Additional Information Requested**

Exact reconnaissance date range; the forensic report identifying the specific detection trigger; any MFA exception record covering the affected server; the full SEC 8-K text; DOJ indictment records confirming attribution.
