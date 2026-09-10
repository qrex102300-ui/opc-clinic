# Revenue Operating Ledger

**Sprint:** $0 → $100 collected revenue by 2026-09-15  
**Last scout update:** 2026-09-11 02:00 China Standard Time  
**New spend:** $0  
**Verified collected revenue:** $0

This ledger records buyer-facing evidence, not product activity. A forum post, directory listing, page view, public bounty, or proposal draft is not a lead or revenue unless the corresponding buyer action is observable.

## Ranked opportunities admitted from the latest scout

### 1. KEEP / PRIORITIZE — Rami RFQ-to-quote paid test

- **Named buyer:** Rami / n8n Community user `Eng_Rami_Sebai`.
- **Public demand evidence:** https://community.n8n.io/t/seeking-estimates-n8n-developer-for-a-small-rfq-to-quote-prototype/312281?tl=en
- **Buyer pain / requested outcome:** convert a fixed-format text-PDF RFQ into extracted codes/descriptions/quantity/units, match only against the buyer-supplied catalogue and approved price list, route uncertain matches to human review, and export an Excel quotation draft.
- **Willingness-to-pay evidence:** the buyer explicitly states that any engagement will start with a separately agreed **paid test** and milestones.
- **Reach path:** reply/DM on the n8n Community thread.
- **Delivery path:** existing synthetic executable proof in `experiments/rfq_quote_demo/`, adapted only after redacted buyer samples and written acceptance criteria are supplied.
- **Prepared paid-test offer:** USD 125 fixed, credited toward a USD 450 first-stage prototype; two-business-day target after usable samples and scope agreement.
- **Acquisition friction:** high competition (the thread accumulated many proposals on 2026-09-10), but the sprint has an already-built, tested proof matched to the requested failure modes.
- **Current state:** proposal READY TO SEND, **not sent**. No qualified lead, order, or revenue may be counted yet.
- **Execution blocker:** current tool environment has no authenticated n8n Community posting identity. Do not impersonate the owner or bypass login.
- **Decision:** keep this as the highest-EV B2B experiment. Do not spend another cycle polishing the proof before contact.

### 2. WATCH / MICRO-REVENUE FALLBACK — LinkModel paid API test

- **Named buyer:** Amy Chao, PM at LinkModel.
- **Public demand evidence:** https://community.n8n.io/t/paid-testing-looking-for-n8n-developers-to-test-our-new-multi-model-api/306268
- **Requested outcome:** connect LinkModel to n8n, complete a real AI task, share the output/workflow result, provide candid feedback, and ideally repeat a task on another day.
- **Explicit payment path:** US$5 cash reward; testing credits supplied by LinkModel.
- **Reach path:** n8n Community comment or private message.
- **Delivery path:** bounded n8n/API test plus structured feedback; no new software spend required.
- **Why it is not promoted above Rami:** US$5 cannot materially close the $100 sprint target and the thread already has many participants. It is useful only as a first-dollar / payment-loop proof if access becomes available.
- **Current state:** not contacted; not a lead; $0 counted.
- **Execution blocker:** same missing authenticated n8n Community identity.

## Agent-native market gate

Fresh scouting found an apparent USDC-paying agent bounty surface branded **UpClaw / CrystalClaw**, with public pages advertising open tasks such as website pricing extraction, data scraping, QA, and content work. Public pages also claim on-chain payouts. However, the public counters shown across its pages are internally inconsistent, and the current environment does not have a verified enrolled agent identity, claim API session, or owner-approved receiving wallet for that surface. Therefore it is **not admitted as a live revenue experiment yet**.

Evidence checked:
- https://crystalclaw.io/
- https://crystalclaw.io/bounties/
- https://crystalclaw.io/network/

Gate to activate C: verify one specific open bounty, its named/fundable poster or escrow state, exact acceptance criteria, claim endpoint, and payout terms; then obtain only the minimum agent identity / receiving-wallet permission required. Do not fund stakes, trade, speculate, or send money to activate earning.

## Benchmark implication

Anthropic's Project Deal showed that agents can execute real transactions when there is a real marketplace, defined budgets/preferences, and actual counterparties; Project Vend Phase Two showed that stronger models, better tools, customer/stock tracking, and tighter operating instructions improved a previously loss-making autonomous shop but did not eliminate robustness problems. For this sprint, the operational translation is: prefer already-funded buyer surfaces and bounded paid tests over building another product or relying on passive traffic.

Official references:
- https://www.anthropic.com/features/project-deal
- https://www.anthropic.com/research/project-vend-2

## Current scorecard

| Metric | Verified current |
|---|---:|
| Collected revenue | $0 |
| Paid orders | 0 |
| Qualified payment-ready leads | 0 |
| Named high-fit B2B prospects with explicit paid-test intent | 1 |
| Micro-paid API-test buyers identified | 1 |
| Proposal actually sent to Rami | 0 |
| New spend | $0 |

## Next scout rule

Do not add another experiment merely because it is buildable. A replacement must beat the Rami path on near-term expected value and must have a named buyer, explicit pain/loss, reachable channel, digitally deliverable outcome, and credible payment path. For agent-native work, public marketplace activity alone is insufficient; verify the specific escrow/payment path before activation.
