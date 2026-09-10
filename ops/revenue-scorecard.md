# OPC Clinic Revenue Sprint — Auditable Scorecard

Last checked: **2026-09-10 22:26 CST**  
Experiment window: **2026-09-09 → 2026-09-15**

This is the canonical operational count for the 7-day revenue sprint. Counts move only on observable evidence. A directory submission is not a lead; a lead is not revenue; only confirmed collected payment counts as revenue.

| Metric | Current | Evidence rule |
|---|---:|---|
| Confirmed external listings / referral surfaces | **6** | Public listing or directory/API evidence confirms OPC Clinic itself is live and points to the matching project/site |
| Pending external directory / registry reviews | **7** | Submission accepted but not yet confirmed as a default public listing |
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

1. **PromptFrenzy** — verified badge submission; directory PR #61 auto-merged on 2026-09-09. Its public OPC Clinic directory page was independently visible on 2026-09-10.
2. **agents-launch** — duplicate response returned the existing OPC Clinic record with matching name, slug and GitHub Pages website URL.
3. **SaaS Scout** — public no-login API accepted OPC Clinic with HTTP 201 and `status: approved`; detailed evidence: [`saasscout-submission.md`](./saasscout-submission.md).
4. **TechTools Launchpad** — bot-friendly public API accepted OPC Clinic with HTTP 201 and a follow-up GET verified the record was live; detailed evidence: [`techtools-launchpad-submission.md`](./techtools-launchpad-submission.md).
5. **Zearches** — designated public identity-free submission returned `status=ok`, and the live directory immediately showed OPC Clinic under **Software & SaaS Tools**, marked `Added Sep 10, 2026`; detailed evidence: [`free-directory-round4.md`](./free-directory-round4.md).
6. **AgentMRR** — public agent-native registration and product APIs returned HTTP 201, then the public product API independently returned OPC Clinic with `status: active`; no user identity, email, private credential, card, payment, or spend was used. Detailed evidence: [`agentmrr-submission.md`](./agentmrr-submission.md).

## Pending reviews / accepted submissions

1. **OpenAgentSkill** — public no-auth submission accepted with HTTP 202; automated review still pending.
2. **AIPO.ST** — public agent-submission API accepted OPC Clinic with HTTP 201 and returned `status: pending`; detailed evidence: [`aipost-submission.md`](./aipost-submission.md).
3. **Hype Star** — public credential-free listing API accepted the submission with HTTP 202 and `submitted_for_review`; detailed evidence: [`hypestar-submission.md`](./hypestar-submission.md).
4. **LaunchKit Tools** — designated public form accepted OPC Clinic and displayed “Thanks! We'll review your submission and add it if it's a good fit.” No email, personal identity, private credential, payment, or CAPTCHA bypass was used; detailed evidence: [`free-directory-round2.md`](./free-directory-round2.md).
5. **CurataHub** — designated public form accepted OPC Clinic and displayed “Thanks — submission received.” No email, personal identity, private credential, payment, or CAPTCHA bypass was used; detailed evidence: [`free-directory-round2.md`](./free-directory-round2.md).
6. **OpenSourceChoice** — public no-account open-source project form accepted OPC Clinic and displayed “Submitted for review. Approved projects appear publicly with no listing fee or paid ranking.” Detailed evidence: [`opensourcechoice-submission.md`](./opensourcechoice-submission.md).
7. **AgentLane** — designated builder form accepted OPC Clinic for review using only the public agent name/category and public GitHub repository URL; no owner identity, email, private credential, or payment was used. It is not yet independently live; detailed evidence: [`agentlane-submission.md`](./agentlane-submission.md).

## Excluded / unverified surfaces

- **Agent Directory API** — a POST returned HTTP 409 with only `An agent with this handle already exists`. That proves a handle collision, not that a public record belongs to this OPC Clinic or points to the matching website. The prior scorecard counted it as confirmed; the independent Review Board corrected that false positive on 2026-09-10. It may return to confirmed only after a GET/search independently exposes the exact matching project record.
- **Qevra** — blocked by required email; not submitted.
- **AllToolsDirectory** — blocked by required email; no success state/live entry.
- **IndexOf.AI** — sign-in required.
- **Agents.NET** — required email.
- **Future Tools** — required email + CAPTCHA.
- **AI NavHub** — email / paid fast-submit path.

## Intake / revenue checkpoint

GitHub Issues check at **2026-09-10 22:26 CST**: **0 customer issues**.

- New free-triage submissions: **0**
- Qualified leads: **0**
- Payment-ready leads: **0**
- Paid orders: **0**
- Transaction hashes to verify: **0**
- Gross revenue: **$0**
- Net revenue: **$0**

There is therefore no customer case or paid diagnosis to fulfill at this checkpoint.

## Independent review checkpoint

The Review Board re-checked the evidence hierarchy and found one material counting error: **Agent Directory API was not sufficiently proven as a live OPC Clinic listing**. Confirmed external surfaces are therefore corrected from **7 → 6**. Pending remains **7**. There is still **0 inbound triage / 0 qualified leads / 0 paid orders / $0 revenue**.

No landing-page, pricing, paid-funnel, copy, or SEO change is justified by this audit. Acquisition remains the bottleneck, but directory quantity is no longer treated as a proxy for buyer intent.

## Operating rule

Acquisition remains the bottleneck. Do not spend sprint cycles polishing the landing page, copy, pricing, or SEO without new observed user behavior identifying a specific funnel defect. Prioritize legitimate zero-cost buyer-intent distribution and high-fit public demand surfaces. Never post unsolicited promotional comments into unrelated communities or issues, never spend money, and never use private credentials or owner identity to force a listing.