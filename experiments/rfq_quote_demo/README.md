# RFQ → Excel quotation draft — synthetic proof

This is a **new synthetic-data proof**, not a client case study and not a claim of prior electrical-parts delivery. It was built after a current buyer requested evidence for a narrowly scoped RFQ-to-quote prototype.

## What this proof actually demonstrates

A generated text-based PDF is processed into line items, checked against a supplied catalogue, priced only from a separately supplied approved price list, and exported as an Excel draft. Unknown codes, unit mismatches, missing approved prices, ambiguous catalogue rows, and other blocked cases are routed to review. If any row needs review, the total is withheld. Every output remains a draft requiring human approval.

The executable test currently covers an end-to-end synthetic PDF → extraction → catalogue/price control → `.xlsx` path. It verifies a correct exact-code match, an unknown code, a unit mismatch, a known item with no approved price, exception-sheet generation, total withholding, and the human-approval marker.

## What is deliberately NOT claimed

- This is not a production client deployment.
- It does not yet orchestrate the steps in an n8n workflow; the proof isolates the deterministic document/matching/Excel core that can sit behind n8n.
- It does not handle scanned PDFs/OCR, multiple PDF layouts, ERP integration, automatic email, dashboards, catalogue cleansing, substitutions, tax, discounts, currency conversion, or production hosting.
- It never invents a price or silently substitutes a product.

## Run

```bash
python -m pip install -r requirements.txt
python -m unittest -v test_rfq_quote.py
```

The test generates its own synthetic PDF and temporary catalogue/price files, so no customer data or credentials are required.

## Buyer-fit hypothesis

For one agreed text-PDF layout and clean catalogue/price inputs, this core can be wrapped in a manually triggered n8n flow for a paid test. Final limits, acceptance criteria, delivery price, and timing must be agreed only after reviewing redacted representative samples. Any paid service or hosting cost requires separate approval.
