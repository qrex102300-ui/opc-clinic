# OPC Clinic Revenue Sprint — Auditable Scorecard

Last checked: **2026-09-10 08:17 CST**  
Experiment window: **2026-09-09 → 2026-09-15**

This is the canonical operational count for the 7-day revenue sprint. Counts move only on observable evidence. A directory submission is not a lead; a lead is not revenue; only confirmed collected payment counts as revenue.

| Metric | Current | Evidence rule |
|---|---:|---|
| Confirmed external listings / referral surfaces | **5** | Public listing or directory/API evidence confirms OPC Clinic is live |
| Pending external directory / registry reviews | **5** | Submission accepted but not yet confirmed as a default public listing |
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

## Pending reviews / accepted submissions

1. **OpenAgentSkill** — public no-auth submission accepted with HTTP 202; automated review still pending.
2. **AIPO.ST** — public agent-submission API accepted OPC Clinic with HTTP 201 and returned `status: pending`; detailed evidence: [`aipost-submission.md`](./aipost-submission.md).
3. **Hype Star** — public credential-free listing API accepted the submission with HTTP 202 and `submitted_for_review`; detailed evidence: [`hypestar-submission.md`](./hypestar-submission.md).
4. **LaunchKit Tools** — designated public form accepted OPC Clinic and displayed “Thanks! We'll review your submission and add it if it's a good fit.” No email, personal identity, private credential, payment, or CAPTCHA bypass was used; detailed evidence: [`free-directory-round2.md`](./free-directory-round2.md).
5. **CurataHub** — designated public form accepted OPC Clinic and displayed “Thanks — submission received.” No email, personal identity, private credential, payment, or CAPTCHA bypass was used; detailed evidence: [`free-directory-round2.md`](./free-directory-round2.md).

## Latest acquisition execution

Round 3 screened five additional public directory routes without spending money or supplying owner identity; detailed evidence: [`free-directory-round3.md`](./free-directory-round3.md).

- **Bro Find AI** — first listing is advertised as free and instant, but the live submission flow requires Google sign-in. Not submitted.
- **IndexOf.AI** — free basic listing is advertised, but the live submit path requires sign-in. Not submitted.
- **That AI Collection** — live submission is a multi-step flow and the page explicitly discusses paid publishing; no identity-free free submission was completed. Not counted.
- **ToolPromote** — free standard listing exists, but the form requires submitter name, email, and relationship to the tool. Skipped before submission.
- **Come AI / iatool.online** — live submission requires email. Skipped before submission.

Round 4 was started against two newly verified identity-free public listing surfaces: **Share Your Startup** (states no account/payment and immediate publishing) and **Zearches** (states no account/payment and direct free submission). The workflow uses only public product facts and is constrained to stop if identity, payment, or human verification appears. No round-4 acceptance evidence exists yet, so neither surface is counted at this checkpoint.

## Other screened but not counted routes

- **CurlShip** — bot-friendly no-login API, but submission requires an email address. Not submitted.
- **Pinstack** — free basic listings exist, but the live product submission redirects to login. Not submitted.
- **AIToolsIndex** — GitHub runner hit `DNS_PROBE_FINISHED_NXDOMAIN`; no submission occurred. Do not retry again without new runner/network evidence.
- **Find AI Tools** — runner received HTTP 403 before the public form loaded; no bypass was attempted.
- **Alieradox** — anti-bot browser check prevented the product fields from loading; no bypass was attempted.
- Third-party GitHub issue/PR submission remains constrained by the connected GitHub account's manual-review restriction; directory-specific public forms/APIs remain the preferred route.

## Intake check

GitHub Issues check at **2026-09-10 08:17 CST**: **0 issues**. Therefore there are no new free-triage submissions, qualified leads, payment-ready leads, paid orders, or transaction hashes to process at this checkpoint.

## Operating rule

Acquisition remains the bottleneck. Do not spend sprint cycles polishing the landing page, copy, pricing, or SEO without new observed user behavior identifying a specific funnel defect. Prioritize legitimate zero-cost distribution and high-fit public demand surfaces. Never post unsolicited promotional comments into unrelated communities or issues, never spend money, and never use private credentials or owner identity to force a listing.