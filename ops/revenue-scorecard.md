# OPC Clinic Revenue Sprint — Auditable Scorecard

Last checked: **2026-09-09 23:34 CST**  
Experiment window: **2026-09-09 → 2026-09-15**

This file is the canonical operational count for the 7-day revenue sprint. Counts only move on observable evidence; directory presence is not treated as a lead, and a lead is not treated as revenue.

| Metric | Current | Evidence rule |
|---|---:|---|
| Confirmed external listings / referral surfaces | **3** | Public listing or directory API confirms the product exists |
| Pending external directory / registry reviews | **1** | Submission accepted but not yet confirmed as a default public listing |
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
2. **Agent Directory API** — public no-auth directory now rejects `opc-clinic` as an existing handle, confirming directory presence.
3. **agents-launch** — public no-auth directory now returns the existing OPC Clinic record (`slug: opc-clinic`, created 2026-09-09T15:28:06Z).
4. **OpenAgentSkill** — its public no-auth submission API accepted `skill/SKILL.md` with HTTP 202 and submission status `submitted`. Automated review is still pending, so this is tracked separately and is **not** counted as a confirmed listing yet.

The zero-cost agent-directory submission audit is recorded in [`ops/agent-directory-submissions.md`](./agent-directory-submissions.md). Submission receipts are sanitized before being committed; private status tokens are not written to the public repository.

## Intake check

GitHub Issues check at 2026-09-09 23:34 CST: **0 issues total**, therefore there are no free-triage submissions, paid orders, or transaction hashes to process in this run.

## Operating rule

Acquisition is still the bottleneck. Do not spend sprint cycles polishing the landing page, copy, or SEO without new observed user behavior identifying a specific funnel defect. Prioritize legitimate distribution and high-fit public demand surfaces; never post unsolicited promotional comments into unrelated communities or issues.
