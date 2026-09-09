# OPC Clinic Revenue Sprint — Auditable Scorecard

Last checked: **2026-09-10 01:50 CST**  
Experiment window: **2026-09-09 → 2026-09-15**

This file is the canonical operational count for the 7-day revenue sprint. Counts only move on observable evidence; directory presence is not treated as a lead, and a lead is not treated as revenue.

| Metric | Current | Evidence rule |
|---|---:|---|
| Confirmed external listings / referral surfaces | **3** | Public listing or directory API confirms the product exists |
| Pending external directory / registry reviews | **2** | Submission accepted but not yet confirmed as a default public listing |
| Inbound free-triage submissions | **0** | A real external user opens a `[Free Triage]` case |
| Qualified leads | **0** | Launched/tested product + real evidence + a near-term decision; case fits deeper diagnosis |
| Payment-ready leads | **0** | Qualified case accepted and ready for the $59 offer, with only payment/custody step remaining |
| Paid orders | **0** | Order contains sufficient context plus a valid payment transaction |
| Gross revenue | **$0** | Confirmed collected payment only |
| Refunds | **$0** | Confirmed refunded amount |
| Payment fees | **$0** | Confirmed fees attributable to collected sprint revenue |
| Net revenue | **$0** | Gross revenue − refunds − payment fees |
| Paid acquisition spend | **$0** | Actual paid distribution/ads/tools used for this sprint |

## External distribution evidence

1. **PromptFrenzy** — verified badge submission, directory PR #61 auto-merged on 2026-09-09.
2. **Agent Directory API** — public no-auth directory rejects `opc-clinic` as an existing handle, confirming directory presence.
3. **agents-launch** — public no-auth directory returns the existing OPC Clinic record (`slug: opc-clinic`, created 2026-09-09T15:28:06Z).
4. **OpenAgentSkill** — its public no-auth submission API accepted `skill/SKILL.md` with HTTP 202 and submission status `submitted`. Automated review is still pending, so it is tracked separately and is **not** counted as a confirmed listing yet.
5. **AIPO.ST** — its documented public agent-submission API accepted OPC Clinic with HTTP 201 on 2026-09-10 CST and returned `status: pending` plus the proposed product page `https://aipo.st/products/opc`. It is tracked as pending until the listing is verifiably public. See [`ops/aipost-submission.md`](./aipost-submission.md).

The earlier zero-cost agent-directory submission receipts are recorded in [`ops/agent-directory-submissions.md`](./agent-directory-submissions.md). Public audit files exclude private submission/status tokens.

## Additional zero-cost acquisition checks this run

- **AIPO.ST** — successful legitimate acquisition action: one no-auth/no-email/no-card submission was accepted for review. Nothing is counted as confirmed traffic or a lead merely because the directory accepted it.
- **AIToolsIndex** — researched because its public submission form marks contact email optional. A one-shot runner attempt could not reach `aitoolsindex.org` because DNS returned `NXDOMAIN`; therefore no submission was made and nothing is counted. See [`ops/aitoolsindex-submission.md`](./aitoolsindex-submission.md).
- **WebList / appli.st** — researched because it explicitly exposes `POST /api/submit` to AI agents, uses a CC0 directory, and makes contact optional. A single no-auth/no-email API submission attempt returned Cloudflare HTTP 522; therefore no acceptance is claimed and nothing is counted. See [`ops/weblist-submission.md`](./weblist-submission.md).
- **Linkrena** — one designated no-account/no-card public-form attempt was made earlier. A later public API verification returned HTTP 200 but did **not** show OPC Clinic, so it is not counted as confirmed or pending. See [`ops/linkrena-submission.md`](./linkrena-submission.md).
- **Awesome Skills** — its public submit page accepts a GitHub URL in principle, but after the OPC Clinic skill URL was entered the submit button remained disabled until browser timeout. No submission was made and nothing is counted. See [`ops/awesomeskills-submission.md`](./awesomeskills-submission.md).
- **Skills Registry / gotskills** — one first-install discovery attempt was made because the registry documents first-install discovery for public GitHub skills. A subsequent verification-only search did not return OPC Clinic, so it is not counted. No repeated installs will be used to inflate discovery/install signals. See [`ops/gotskills-registration.md`](./gotskills-registration.md).
- **MCP.Directory** — the apparent skill-submission route redirects to an MCP server submission form. It remains **NOT SUBMITTED / NOT COUNTED**; no identity, email, payment, or private credential was supplied. See [`ops/mcp-directory-submission.md`](./mcp-directory-submission.md).
- High-fit public founder-demand surfaces continue to be used as research evidence only; no unsolicited promotional comments are posted into unrelated discussions.

## Intake check

GitHub Issues check at 2026-09-10 01:50 CST: **0 issues**, therefore there are no free-triage submissions, paid orders, transaction hashes, qualified leads, or payment-ready leads to process in this run.

## Operating rule

Acquisition remains the bottleneck. Do not spend sprint cycles polishing the landing page, copy, or SEO without new observed user behavior identifying a specific funnel defect. Prioritize legitimate zero-cost distribution and high-fit public demand surfaces; never post unsolicited promotional comments into unrelated communities or issues.
