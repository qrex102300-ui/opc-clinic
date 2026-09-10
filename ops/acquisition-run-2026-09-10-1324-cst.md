# OPC Clinic acquisition + intake audit — 2026-09-10 13:24 CST

This run remained acquisition-first. No landing-page, product, pricing, copy, or SEO changes were made.

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

### SearchAITools — human-verification blocked; not counted

SearchAITools was independently screened as a potentially high-fit zero-cost AI-tool directory because its public submit surface advertised a free permanent listing and no account requirement. A one-shot browser workflow attempted only the designated public submission route and supplied no identity, email, payment, private credential, or unsolicited community comment.

The live runner was stopped by Cloudflare's **security verification / bot check** before the form became available. No bypass was attempted. The surface is not counted as submitted, pending, or confirmed. The audit record was corrected so its human-verification flag matches the observed page: [`searchaitools-submission.md`](./searchaitools-submission.md).

### Directory round 7 — three screened surfaces, zero counted submissions

- **Ship or Skip:** the designated `/submit` route returned a Vercel `DEPLOYMENT_NOT_FOUND` 404. No submission occurred.
- **FindTools Guide:** its current live page says tool submissions have moved to a community Submission Center and now require **Google sign-in**. No account or identity was used.
- **Aiverda Labs:** the live runner was stopped at a browser security-check page before the public form became available. No bypass was attempted.

Full sanitized evidence is in [`free-directory-round7.md`](./free-directory-round7.md).

Completed one-shot acquisition workflows for SearchAITools, directory round 5, DiscoverAISkills, and directory round 7 were removed after their audit records were committed, so they cannot accidentally re-submit on future pushes.

## Acquisition evidence / screening decisions

Fresh screening continues to show a recurring constraint: many nominally free directories either require person/email identity, require sign-in, place the submit route behind bot verification, or require a reciprocal backlink/site modification. Those routes are skipped rather than inventing identity, using private credentials, bypassing controls, or changing the funnel without observed user behavior.

Third-party GitHub issue/PR directory routes also remain deprioritized because the connected GitHub account previously received an account-level 403/manual-review restriction for third-party writes. No retry or workaround was attempted.

## Canonical counts after this run

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

Acquisition remains the bottleneck. The next run should continue checking pending approvals and finding legitimate identity-free, zero-cost discovery surfaces rather than polishing the product or funnel without behavioral evidence.
