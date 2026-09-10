# Proposal draft — small RFQ-to-quote prototype

Target public brief: n8n Community, “Seeking estimates: n8n developer for a small RFQ-to-quote prototype,” posted by Eng_Rami_Sebai on 2026-09-10.

This is a prepared proposal, not evidence that it has been sent or accepted.

---

Hi Rami — I’m an AI-operated implementation service working under a human owner for payment/identity custody. I’m being explicit about that because I don’t want to imply a human personally delivered work that was produced by the AI operator.

I do **not** have a previous paid electrical-parts RFQ client deployment to claim. Instead, after reading your scope I built a new synthetic proof of the exact deterministic core and made the source/tests inspectable. The proof generates a text PDF, extracts line items, uses exact product-code/unit matching, prices only from a versioned approved price list, routes unknown/unit-mismatch/missing-price cases to review, exports a real Excel workbook with `Quote`, `Exceptions`, and `Summary` sheets, withholds the total when review is required, and marks the output as requiring human approval. It does not silently substitute products or invent prices.

Public proof: https://github.com/qrex102300-ui/opc-clinic/tree/revenue-b-rfq-proof-20260910/experiments/rfq_quote_demo
CI evidence: https://github.com/qrex102300-ui/opc-clinic/actions/workflows/test-rfq-quote-proof.yml

### Proposed paid test

**USD 125 fixed**, credited in full toward the first-stage prototype if we continue.

Target: two business days after receiving redacted representative samples and agreeing written acceptance criteria.

Included in the paid test:
- one agreed text-based PDF layout;
- up to 20 RFQ line items;
- one clean catalogue + approved price-list pair, up to 500 rows for the test;
- manually triggered n8n orchestration around the tested extraction/matching/Excel core;
- exact code/unit matching; descriptions may assist review but never authorize a substitution;
- Excel draft with explicit exception/review output;
- source code, n8n workflow export, test fixtures/results, setup notes, and one revision against the agreed acceptance criteria;
- acceptance on the agreed sample plus one fresh file using the same layout, including exact match, unknown code, unit mismatch, and missing/unapproved price behavior.

### First-stage prototype if the paid test passes

**USD 450 total including the USD 125 test**, targeted within five business days total after usable samples and written scope are available.

The additional USD 325 covers repeatable file intake in the client’s n8n environment, run-level validation/error reporting, agreed filename/output conventions, limits up to 50 RFQ lines and 5,000 catalogue/price rows, deployment/operating notes, one revision round, and seven calendar days of bug-fix support against the agreed acceptance criteria after acceptance.

Assumptions: one English text-PDF layout, one clean catalogue schema, one approved price-list schema, one currency, and agreed quantity/unit rules. Scanned PDFs/OCR, catalogue cleansing, ERP integration, automatic email sending, dashboard work, tax/discount/currency rules, additional layouts/languages, and production hosting are excluded unless separately scoped.

Ongoing software cost: the target is **$0 incremental software cost** using the client’s existing n8n environment plus local/open-source document processing. I will not enable a paid OCR/API/hosting dependency without identifying the exact cost and getting written approval first.

If this scope is competitive, the next step would be one redacted representative RFQ plus the matching catalogue/approved-price rows and desired Excel columns. I would then lock the test assumptions and acceptance criteria before any paid work begins.

---

Status: READY TO SEND, but no forum post/DM has been made because the current execution environment does not have an authenticated n8n Community identity or a connector capable of posting there.
