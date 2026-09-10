# OPC Clinic Revenue Sprint — Auditable Scorecard

Last checked: **2026-09-10 18:00 CST**  
Experiment window: **2026-09-09 → 2026-09-15**

This is the canonical operational count for the 7-day revenue sprint. Counts move only on observable evidence. A directory submission is not a lead; a lead is not revenue; only confirmed collected payment counts as revenue.

| Metric | Current | Evidence rule |
|---|---:|---|
| Confirmed external listings / referral surfaces | **7** | Public listing or directory/API evidence confirms OPC Clinic is live |
| Pending external directory / registry reviews | **6** | Submission accepted but not yet confirmed as a default public listing |
| Inbound free-triage submissions | **0** | A real external user opens a `[Free Triage]` case |
| Qualified leads | **0** | Launched/tested product + real evidence + near-term decision; case fits deeper diagnosis |
| Payment-ready leads | **0** | Qualified case is ready for the $59 offer and only payment/custody remains |
| Paid orders | **0** | Sufficient customer context plus a valid payment transaction |
| Gross revenue | **$0** | Confirmed collected payment only |
| Refunds | **$0** | Confirmed refunded amount |
| Payment fees | **$0** | Confirmed fees attributable to collected sprint revenue |
| Net revenue | **$0** | Gross revenue − refunds − payment fees |
| Paid acquisition spend | **$0** | Actual paid distribution, ads, or tools used for this sprint |

## Confirmed external discovery surfaces

1. **PromptFrenzy** — verified badge submission; directory PR #61 auto-merged on 2026-09-09.
2. **Agent Directory API** — public no-auth directory already recognizes the `opc-clinic` handle.
3. **agents-launch** — public no-auth directory returns an existing OPC Clinic record.
4. **SaaS Scout** — public no-login API accepted OPC Clinic with HTTP 201 and `status: approved`; detailed evidence: [`saasscout-submission.md`](./saasscout-submission.md).
5. **TechTools Launchpad** — bot-friendly public API accepted OPC Clinic with HTTP 201 and a follow-up GET verified the record was live; detailed evidence: [`techtools-launchpad-submission.md`](./techtools-launchpad-submission.md).
6. **Zearches** — designated public identity-free submission returned `status=ok`, and the live directory immediately showed OPC Clinic under **Software & SaaS Tools**, marked `Added Sep 10, 2026`; detailed evidence: [`free-directory-round4.md`](./free-directory-round4.md).
7. **AgentMRR** — public agent-native registration and product APIs returned HTTP 201, then the public product API independently returned OPC Clinic with `status: active`; no user identity, email, private credential, card, payment, or spend was used. Detailed evidence: [`agentmrr-submission.md`](./agentmrr-submission.md).

## Pending reviews / accepted submissions

1. **OpenAgentSkill** — public no-auth submission accepted with HTTP 202; automated review still pending.
2. **AIPO.ST** — public agent-submission API accepted OPC Clinic with HTTP 201 and returned `status: pending`; detailed evidence: [`aipost-submission.md`](./aipost-submission.md).
3. **Hype Star** — public credential-free listing API accepted the submission with HTTP 202 and `submitted_for_review`; detailed evidence: [`hypestar-submission.md`](./hypestar-submission.md).
4. **LaunchKit Tools** — designated public form accepted OPC Clinic and displayed “Thanks! We'll review your submission and add it if it's a good fit.” No email, personal identity, private credential, payment, or CAPTCHA bypass was used; detailed evidence: [`free-directory-round2.md`](./free-directory-round2.md).
5. **CurataHub** — designated public form accepted OPC Clinic and displayed “Thanks — submission received.” No email, personal identity, private credential, payment, or CAPTCHA bypass was used; detailed evidence: [`free-directory-round2.md`](./free-directory-round2.md).
6. **OpenSourceChoice** — public no-account open-source project form accepted OPC Clinic and displayed “Submitted for review. Approved projects appear publicly with no listing fee or paid ranking.” Detailed evidence: [`opensourcechoice-submission.md`](./opensourcechoice-submission.md).

## Intake / revenue checkpoint

GitHub Issues check at **2026-09-10 18:00 CST**: **0 customer issues**.

- New free-triage submissions: **0**
- Qualified leads: **0**
- Payment-ready leads: **0**
- Paid orders: **0**
- Transaction hashes to verify: **0**
- Gross revenue: **$0**
- Net revenue: **$0**

There is therefore no customer case or paid diagnosis to fulfill at this checkpoint.

## Latest acquisition checkpoint

The 18:00 CST run remained acquisition-first and made no landing-page, pricing, copy, or SEO changes. Fresh discovery focused on high-fit **agent-skill** surfaces rather than adding more generic startup directories. MCP.Directory exposes a public Skill submission route whose required input is only a public skill URL, so an identity-free submission was attempted through GitHub Actions. The post-submit page redirected to the generic **Submit a Server** form and returned no skill-specific receipt or acknowledgement; a broad workflow matcher initially produced a false-positive success signal. The audit was corrected immediately and **MCP.Directory is not counted** as either a live listing or a pending review. The path is not blindly retried to avoid duplicates; detailed evidence: [`mcp-directory-submission.md`](./mcp-directory-submission.md).

A second high-fit route, **anbeime/skill**, provides a designated `skill-submission` GitHub issue template and had no OPC Clinic duplicate in repository/issue search. The connected GitHub integration can read that external repository but returned HTTP 403 when asked to create the submission issue, so no external issue was posted and no owner identity was impersonated. **AgenticSkills** was also screened but its free submission requires both author name and email, so it was not attempted. A fresh search across the six already-pending directories returned no public OPC Clinic listing evidence, so the counts remain 7 confirmed / 6 pending. Acquisition remains the bottleneck.

## Operating rule

Acquisition remains the bottleneck. Do not spend sprint cycles polishing the landing page, copy, pricing, or SEO without new observed user behavior identifying a specific funnel defect. Prioritize legitimate zero-cost distribution and high-fit public demand surfaces. Never post unsolicited promotional comments into unrelated communities or issues, never spend money, and never use private credentials or owner identity to force a listing.
