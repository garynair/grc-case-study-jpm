**MODEL ANSWER — TASK 9: Conduct the Incident Tabletop and Present to Executives**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 9's required outputs. Multiple good answers are possible — what matters is that decisions are time-bound, escalation is clear, and communication reflects only verified facts.*

## Tabletop Decision Log

| **Inject** | **Decision** | **Owner** | **Deadline** | **Rationale** | **Evidence** |
|---|---|---|---|---|---|
| 1 — SOC confirms unusual login to an internet-facing microsite using a valid employee account. | Disable/reset the account; isolate the server; preserve logs; declare a high-severity incident; assign an incident commander. | SOC / Incident Commander | Immediate (within the hour) | Contain confirmed unauthorized access before scope is known, and preserve evidence before it degrades. | Account-disable ticket, isolation confirmation, incident declaration record, SOC log extract. |
| 2 — Forensics finds connections from the microsite to multiple internal servers. | Block unnecessary cross-zone paths; segment affected systems; review privileged credentials; notify CISO, Legal, and executive leadership. | Network Security / IAM; CISO notified | Within 4 hours of the finding | Lateral movement signals enterprise-scale exposure; further reach must be limited before data scope is known. | Firewall change record, segmentation confirmation, privileged-access review log, executive notification timestamp. |
| 3 — Evidence shows access to a customer contact database and ~90 servers. | Engage Privacy, regulators, and law enforcement; assess data scope and materiality; preserve evidence; determine customer-protection actions. | Legal / Privacy / Incident Commander | Same day — materiality assessment opened | Scale of access likely triggers regulatory notification and disclosure clocks that must be assessed before any external statement. | Data-scoping report, regulator/FBI engagement log, decision-log entry, preserved forensic image. |
| 4 — No account numbers, passwords, or SSNs are confirmed stolen. | Communicate accurately: state confirmed data, unknowns, actions taken, and ongoing monitoring; do not claim zero risk. | Corporate Communications / Legal; approved by CISO / executives | Before any public or customer statement is released | Overstating certainty is a reputational and legal liability if new facts emerge; understating is a disclosure risk. | Approved message draft, legal sign-off, distribution log. |

## Communication Matrix

| **Audience** | **Information** | **Timing** | **Owner** | **Approval** |
|---|---|---|---|---|
| Executive leadership / Board | Scope, customer impact, business disruption, regulatory exposure, decisions and resources needed. | Every 2–4 hours initially | CISO / Incident Commander | Not required for internal briefing; Board informed, not asked to approve. |
| Legal / Compliance / Privacy | Data involved, jurisdictions, materiality, notification deadlines, evidence status. | Continuous during scoping | Incident Commander | General Counsel |
| Regulators / SEC | Material verified facts, timing, impact, remediation. | Per applicable regulatory deadline | Legal / Corporate Secretary | Disclosure Committee / General Counsel |
| FBI / Law enforcement | Indicators, evidence, suspected criminal activity. | Promptly after confirmation | Legal / CISO | General Counsel / CISO |
| Employees | Required credential resets, phishing awareness, operational instructions. | As actions are approved | Internal Communications | CISO |
| Customers | Confirmed data affected, protective steps, contact channels. | After facts and obligations are validated | Corporate Communications / Legal | General Counsel, Corporate Communications, CEO sign-off |

## One-Page Executive Report

| **Section** | **Content** |
|---|---|
| Situation | Attackers gained access through an internet-facing Corporate Challenge server omitted from the enterprise MFA upgrade, and used that foothold to reach approximately 90 servers. |
| Impact | Names, addresses, phone numbers, and email addresses for 76 million households and 7 million small businesses were accessed. No financial account data, passwords, or Social Security numbers were confirmed stolen. |
| Root Cause | Incomplete asset inventory, ineffective control-exception management, and inadequate segmentation between a low-criticality web property and internal customer systems. |
| Actions Taken | Containment, credential resets, forensic investigation, law-enforcement coordination, vulnerability closure, data scoping, and executive/regulatory communication. |
| Decisions Needed | Approve enterprise internet-facing asset review, mandatory MFA exception closure, segmentation remediation, formal exception governance, and independent assurance testing. |
| Lesson | Security capability does not create assurance unless governance confirms complete control coverage across every in-scope asset. |

## Five-Minute Risk Committee Presentation — Outline

- Opening (30 sec): One sentence framing — what happened, and that it is contained. Lead with control, not alarm.
- Situation and impact (90 sec): Entry point, what was accessed, what was not confirmed stolen, and current containment status.
- Root cause (60 sec): Frame as governance completeness — inventory, exception management, and segmentation — not a technology failure.
- Actions taken and in progress (60 sec): Containment steps completed; forensic, legal, and regulatory engagement underway.
- Decisions needed from the Committee (60 sec): Name each approval explicitly — asset review scope, exception-closure mandate, segmentation funding, disclosure timing.
- Close (10–15 sec): Confirm next update cadence and who owns the next decision point.

## Question Answers

| **Question** | **Model Answer** |
|---|---|
| When should operations be interrupted to contain risk? | When continued operation materially increases data loss, attacker access, safety risk, or regulatory exposure — use the least disruptive containment that is still effective. |
| What facts must be verified before public communication? | Affected systems, data categories, population size, timeline, containment status, any known fraud, applicable legal obligations, and what remains uncertain. |
| What decisions require executive or Risk Committee approval? | Major shutdowns, public disclosure, material risk acceptance, funding, vendor or service termination, and overdue critical exceptions. |
| What is the single most important governance lesson? | Governance completeness and exception management are what make security controls actually apply everywhere they are required — capability without coverage is not assurance. |
