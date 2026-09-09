# OPC Clinic Revenue Sprint — Auditable Scorecard

Last checked: **2026-09-10 03:20 CST**  
Experiment window: **2026-09-09 → 2026-09-15**

This file is the canonical operational count for the 7-day revenue sprint. Counts only move on observable evidence; directory presence is not treated as a lead, and a lead is not treated as revenue.

| Metric | Current | Evidence rule |
|---|---:|---|
| Confirmed external listings / referral surfaces | **5** | Public listing or directory API confirms the product exists |
| Pending external directory / registry reviews | **3** | Submission accepted but not yet confirmed as a default public listing |
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
4. **SaaS Scout** — documented public no-login product API accepted OPC Clinic with HTTP 201 and returned `status: approved`, `slug: opc-clinic`, an 85/100 relevance score, and `isRelevant: true` on 2026-09-10 CST. No account, email, payment, private credential, or personal identity was supplied. See [`ops/saasscout-submission.md`](./saasscout-submission.md).
5. **TechTools Launchpad** — its public page explicitly states no registration, no CAPTCHA, instant listing, and an AI/bot-friendly API. The API accepted OPC Clinic with HTTP 201, returned tool ID `817` plus a public share URL, and a follow-up GET verified the record was live. Optional submitter identity fields were omitted. See [`ops/techtools-launchpad-submission.md`](./techtools-launchpad-submission.md).
6. **OpenAgentSkill** — its public no-auth submission API accepted `skill/SKILL.md` with HTTP 202 and submission status `submitted`. Automated review is still pending, so it is tracked separately and is **not** counted as a confirmed listing yet.
7. **AIPO.ST** — its documented public agent-submission API accepted OPC Clinic with HTTP 201 on 2026-09-10 CST and returned `status: pending` plus the proposed product page `https://aipo.st/products/opc`. It is tracked as pending until the listing is verifiably public. See [`ops/aipost-submission.md`](./aipost-submission.md).
8. **Hype Star** — its public OpenAPI contract explicitly supports credential-free project submission for permanent basic inclusion after review. OPC Clinic was submitted once as a `service` in `services-marketplaces` with `supporterChoice: skipped`; HTTP 202 returned `submitted_for_review` / `pending`, and a post-submit public search correctly showed no public listing yet. No account, email, API key, card, payment, badge, reciprocal link, private credential, or identity was used. See [`ops/hypestar-submission.md`](./hypestar-submission.md).

The earlier zero-cost agent-directory submission receipts are recorded in [`ops/agent-directory-submissions.md`](./agent-directory-submissions.md). Public audit files exclude private submission/status tokens.

## Additional zero-cost acquisition checks this run

- **Hype Star** — successful legitimate acquisition action. Its current public OpenAPI contract documents `POST /api/v1/listings`, requires only the public URL, listing kind, and category slug, and explicitly states that no account, email, API key, card, payment, supporter badge, or renewal is required. A preflight search found no existing OPC Clinic listing; one submission then returned HTTP 202 with `publicationStatus: submitted_for_review` and `reviewStatus: pending`. It is counted as pending, not confirmed, and not as a lead. The optional supporter choice was explicitly skipped, so this created no product/funnel change or backlink obligation. See [`ops/hypestar-submission.md`](./hypestar-submission.md).
- **TechTools Launchpad** — successful legitimate acquisition action. Its documented public API is explicitly designed for bots and AI agents. A preflight listing check avoided duplicates; the submission then returned HTTP 201 with `success: true` and `Tool submitted successfully! It is now live.`, and a post-submit listing check independently found the OPC Clinic URL. It is counted as a confirmed external listing, not as a lead. No account, email, payment, private credential, or submitter identity was used.
- **SaaS Scout** — successful legitimate acquisition action. The site publicly states that no login is required to submit. A public API-contract probe showed that `POST /api/products` requires only name, tagline, description, website, and category; an actual submission was then accepted with HTTP 201 and `status: approved`. It is counted as a confirmed external listing, not as a lead. See [`ops/saasscout-submission-route.md`](./saasscout-submission-route.md) and [`ops/saasscout-submission.md`](./saasscout-submission.md).
- **AIPO.ST** — successful legitimate acquisition action from an earlier run: one no-auth/no-email/no-card submission was accepted, but the returned state remains pending and is not counted as confirmed traffic or a lead.
- **AIToolsIndex** — its live public submission page currently marks contact email optional. Because a fresh public crawl resolved the page after the earlier GitHub-runner DNS failure, one justified retry was made without identity or email. The runner still returned `DNS_PROBE_FINISHED_NXDOMAIN` before reaching the form, so no submission occurred and nothing is counted. Do not retry again without new runner/network evidence. See [`ops/aitoolsindex-submission.md`](./aitoolsindex-submission.md).
- **WebList / appli.st** — researched because it explicitly exposes `POST /api/submit` to AI agents, uses a CC0 directory, and makes contact optional. A single no-auth/no-email API submission attempt returned Cloudflare HTTP 522; therefore no acceptance is claimed and nothing is counted. See [`ops/weblist-submission.md`](./weblist-submission.md).
- **Linkrena** — one designated no-account/no-card public-form attempt was made earlier. A later public API verification returned HTTP 200 but did **not** show OPC Clinic, so it is not counted as confirmed or pending. See [`ops/linkrena-submission.md`](./linkrena-submission.md).
- **Awesome Skills** — its public submit page accepts a GitHub URL in principle, but after the OPC Clinic skill URL was entered the submit button remained disabled until browser timeout. No submission was made and nothing is counted. See [`ops/awesomeskills-submission.md`](./awesomeskills-submission.md).
- **Skills Registry / gotskills** — one first-install discovery attempt was made because the registry documents first-install discovery for public GitHub skills. A subsequent verification-only search did not return OPC Clinic, so it is not counted. No repeated installs will be used to inflate discovery/install signals. See [`ops/gotskills-registration.md`](./gotskills-registration.md).
- **MCP.Directory** — the apparent skill-submission route redirects to an MCP server submission form. It remains **NOT SUBMITTED / NOT COUNTED**; no identity, email, payment, or private credential was supplied. See [`ops/mcp-directory-submission.md`](./mcp-directory-submission.md).
- **SubmitLLMs** — researched as another legitimate free discovery surface focused on AI-ready websites. Its public directory currently indexes thousands of sites, but no no-identity submission contract was proven in this run, so no submission was made and nothing is counted.
- **Current founder-demand evidence** — recent public SaaS and indie-founder discussions continue to show launched products with zero paid users and distribution/customer acquisition as repeated bottlenecks. These surfaces are used only to guide channel selection; no unsolicited promotion is posted into ordinary help threads. See [`ops/acquisition-demand-evidence.md`](./acquisition-demand-evidence.md).

## Intake check

GitHub Issues check at 2026-09-10 03:20 CST: **0 issues**, therefore there are no free-triage submissions, paid orders, transaction hashes, qualified leads, or payment-ready leads to process in this run.

## Operating rule

Acquisition remains the bottleneck. Do not spend sprint cycles polishing the landing page, copy, or SEO without new observed user behavior identifying a specific funnel defect. Prioritize legitimate zero-cost distribution and high-fit public demand surfaces; never post unsolicited promotional comments into unrelated communities or issues.
