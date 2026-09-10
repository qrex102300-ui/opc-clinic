# Acquisition run — 2026-09-10 21:56 CST

Objective: revenue-first acquisition. No landing-page, pricing, copy, SEO-page, or paid-funnel changes were made.

## Intake and revenue

A fresh GitHub issue search returned `total_count: 0` for `repo:qrex102300-ui/opc-clinic is:issue`.

- New free-triage submissions: **0**
- Qualified leads: **0**
- Payment-ready leads: **0**
- Paid orders: **0**
- Transaction hashes to verify: **0**
- Gross revenue: **$0**
- Net revenue: **$0**

There is no customer case to fulfill at this checkpoint.

## Acquisition actions

### Qevra — guarded API attempt

Fresh public research found Qevra advertising a free public listing with a documented no-key `POST /api/submit` path. The sprint authorized legitimate zero-cost external distribution, so a one-shot workflow attempted the public API using only OPC Clinic's public URL/name/tagline/category and `board_notes: false`; no owner email, identity, private credential, payment, ad purchase, or human-verification bypass was supplied.

Observed response:

```json
{
  "http": 400,
  "body": {
    "ok": false,
    "error": "A valid email is required."
  }
}
```

Classification: **BLOCKED BY REQUIRED EMAIL / DO NOT COUNT**. Detailed receipt: [`qevra-submission.md`](./qevra-submission.md).

### AllToolsDirectory — guarded designated-form attempt

The public submission page advertises free submission and no login. A guarded browser attempt supplied only public OPC Clinic project information and left contact email/social fields blank.

The designated submit action did not produce a success state. Instead, the form displayed **“Please enter a valid email address”** and stayed on the submission page. No public OPC Clinic entry was found.

Classification: **BLOCKED BY REQUIRED EMAIL / DO NOT COUNT**. The initial automation heuristic falsely treated static “review” language as acceptance; the audit was corrected so the scorecard cannot over-count it. Detailed receipt: [`alltoolsdirectory-submission.md`](./alltoolsdirectory-submission.md).

## Fresh surface screening — no forced submissions

The following high-fit public surfaces were re-checked and rejected for this run because their current submission path requires identity/contact/payment or sign-in:

- **IndexOf.AI** — free basic listing exists, but the submit page requires sign-in.
- **Agents.NET** — free agent listing, but `Your Email *` is required.
- **Future Tools** — tool submission requires owner email and loads CAPTCHA; no bypass attempted.
- **AI NavHub** — current submission path exposes an email field and promotes a paid fast-submit route; no paid/identity action attempted.

Open-source PR directories such as **aifindr.org** remain legitimate zero-cost targets, but the connected GitHub identity has read-only permission on the upstream repository and no safe fork action is available in the current connector. No unauthorized upstream write was attempted.

## Discovery status

PromptFrenzy's public directory page for OPC Clinic was independently visible during this run, so the existing confirmed listing remains valid. No fresh evidence justified changing the status of the seven pending directory reviews.

Canonical counts therefore remain:

- Confirmed external listings / referral surfaces: **7**
- Pending external directory / registry reviews: **7**
- Inbound free-triage submissions: **0**
- Qualified leads: **0**
- Payment-ready leads: **0**
- Paid orders: **0**
- Gross revenue: **$0**
- Net revenue: **$0**
- Paid acquisition spend: **$0**

## Next-run rule

Keep acquisition-first. Do not retry Qevra or AllToolsDirectory without explicit owner authorization for an email identity. Prefer newly discovered no-login/no-email/no-payment APIs, designated public forms, public registries, and independent verification of pending listings. Do not post unsolicited promotional comments.