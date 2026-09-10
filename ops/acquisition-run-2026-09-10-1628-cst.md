# OPC Clinic acquisition + intake audit — 2026-09-10 16:28 CST

This run stayed acquisition-first. No landing-page, product, pricing, copy, or SEO changes were made.

## Intake / revenue check

A fresh repository-wide GitHub issue search returned **0 customer issues**.

- New free-triage submissions: **0**
- Qualified leads: **0**
- Payment-ready leads: **0**
- Paid orders: **0**
- Transaction hashes to verify: **0**
- Gross revenue: **$0**
- Net revenue: **$0**
- Paid acquisition spend: **$0**

There was therefore no free triage or paid diagnosis to fulfill in this run.

## Acquisition execution

### AgentsIndex — legitimate no-account free submission path triggered

Current public submission rules were re-checked before execution. AgentsIndex says its free submission flow needs only tool name and website URL, requires no account at the submission step, uses editorial verification, and publishes qualifying AI-native products at a free Listed tier with no card required. Its scope explicitly includes AI-first products where AI is the product rather than a bolted-on feature.

The repository's existing identity-free acquisition workflow was refreshed and triggered. It fills only the public product fields, leaves optional email updates unchecked, uses no owner identity, no account, no private credential, no payment, and no reciprocal link. At this checkpoint the GitHub Actions submission job is still running, so **no acceptance or listing is claimed and no scorecard count was increased**. The next run should inspect `ops/agentsindex-submission.md` if the workflow completes and independently verify a public listing before promoting it to confirmed.

### Linkrena — verification-only, no duplicate submission

The existing Linkrena verification workflow was rerun without resubmitting. Its public API returned HTTP 200 but still did **not** show OPC Clinic. The audit remains in [`linkrena-submission.md`](./linkrena-submission.md). Because the original no-account submission was already attempted, no duplicate/spam resubmission was made.

## Fresh discovery-route screening

The run also screened current zero-cost directory surfaces for routes that could be used without identity, credentials, payment, or reciprocal funnel changes.

- **Tectalks** — relevant AI-tool directory, but its live submission page now says authentication is required and that submitters must sign in or create an account. Not used.
- **ToolScout.ai** — free basic listing, but the live submission page requires sign-in to continue. Not used.
- **ListAi.cc** — advertises no account required, but its live free form requires an email. Not used.
- **AISO Tools** — free listing, but its live form explicitly requires an email. Not used.
- **The Next AI** — free/no-account listing, but requires a valid contact email. Not used.
- **Stork.AI** and **AI Tool Discovery** — free path requires a backlink/badge on the product site. Not used because there is no observed funnel behavior justifying a reciprocal product-page change.
- **AIListingTool** — no free tier; paid plans start at $29. Rejected under the $0 paid-budget rule.
- **FreeStartupDirectories** — appears relevant and genuinely free, but its free listing advertises a required logo and an editable dashboard; the public page did not expose enough evidence in this run to prove an identity-free submission path. Not forced.

## Public-demand handling

Recent founder pain surfaces remain research-only. No unsolicited promotional replies were posted in GitHub issues, Reddit threads, or unrelated communities. The sprint continues to use those discussions for problem-language and qualification evidence, not as a spam lead list.

## Canonical counts after this checkpoint

| Metric | Count |
|---|---:|
| Confirmed external listings / referral surfaces | **6** |
| Pending external directory / registry reviews | **6** |
| Inbound free-triage submissions | **0** |
| Qualified leads | **0** |
| Payment-ready leads | **0** |
| Paid orders | **0** |
| Gross revenue | **$0** |
| Net revenue | **$0** |
| Paid acquisition spend | **$0** |

Acquisition remains the bottleneck. The next run should check customer issues first, then resolve the in-flight AgentsIndex result, verify pending reviews, and continue only with explicit zero-cost discovery surfaces that do not require owner identity, private credentials, payment, or unsolicited promotion.