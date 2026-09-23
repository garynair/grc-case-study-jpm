**MODEL ANSWER — TASK 1: Understand the Case and Learn the Basic Terms**

*JPMorgan Chase 2014 GRC Case Study*
*This model answer shows one strong way to meet Task 1's required outputs. Multiple good answers are possible — what matters is that the required elements are present and the reasoning is supported by the case.*

**Case Fact Sheet**

| **Question** | **Response** | **Basis** |
|---|---|---|
| Who was affected? | 76M households + 7M small businesses | Verified fact — Incident & Business Impact |
| What information was accessed? | Names, addresses, phone numbers, email addresses | Verified fact |
| What was NOT confirmed stolen? | Account data, passwords, SSNs, financial information | Verified fact |
| Initial entry point? | JPMC Corporate Challenge microsite (unprotected) | Verified fact |
| What control was missing? | 2FA/MFA — server excluded from the enterprise rollout | Root-cause finding |
| Why governance, not just tech? | Incomplete asset inventory kept the server out of scope; no documented exception (owner, deadline, compensating control); lateral movement reached ~90 servers | Root-cause finding |
| Fact vs. assumption? | A fact is stated directly and supported by evidence; an assumption fills a gap the source doesn't confirm and needs further evidence | Definitional |

**150-Word Summary**

June 2014: JPMorgan's Corporate Challenge microsite (a charitable running-event site) was breached using compromised login credentials. The server had not been upgraded to 2FA during JPMorgan's enterprise rollout because it was missing from the asset inventory that drove that project. From that single foothold, attackers moved laterally across roughly 90 servers and reached a customer database. JPMorgan's security team detected the activity in late July, after about 6–8 weeks of dwell time. By August the breach was contained: approximately 76 million households and 7 million small businesses had contact data accessed (names, addresses, phone numbers, emails) — no SSNs, passwords, or financial data were confirmed stolen. Public disclosure followed via an SEC filing in October. Regulatory outcome details remain an open evidence item.

**Five Investigation Questions**

- Who owned the Corporate Challenge microsite, and who approved its connection to JPMorgan's internal network? — establishes the accountability gap that let an unmanaged asset reach the internal network.
- Why was the server excluded from the asset inventory? — the root cause: this exclusion is why it missed the 2FA rollout entirely.
- Was a formal MFA exception ever recorded, approved and assigned to an owner? — tests whether a real exception process existed or the gap was simply unmanaged.
- What segmentation or firewall gaps let attackers reach the customer database? — identifies whether network design amplified a low-risk asset into a high-impact breach.
- What logs or alerts eventually detected the activity, and why did detection take 6–8 weeks? — assesses whether monitoring tools worked but response was slow, or detection itself was delayed.
