# Revenue Operating Ledger

**Sprint:** $0 → $100 collected revenue by 2026-09-15  
**Last scout update:** 2026-09-11 10:07 China Standard Time  
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
- **Fresh acquisition state:** current n8n index crawls show the thread accumulating dozens of replies while Rami is still shortlisting. Public reply/view counters vary across cached language/index pages, so the ledger does not freeze one unstable counter; the reliable conclusion is that competition is materially higher than when this buyer was first admitted.
- **Identity audit caution:** the public thread now contains a proposal under the unrelated account name `SeverianRoth` that closely matches this sprint's prepared USD 125 / USD 450 structure and synthetic-proof framing. No owner authorization or verified linkage between that public identity and this sprint is available in the current evidence. Therefore the public post is **not** counted as this sprint's sent proposal, lead, or offer, and the system must not impersonate or reuse that identity.
- **Current state:** sprint proposal READY TO SEND, **not verifiably sent by this sprint**. No qualified lead, order, or revenue may be counted yet.
- **Execution blocker:** current tool environment has no authenticated, owner-approved n8n Community posting identity. Do not impersonate the owner or bypass login.
- **Decision:** remains the highest-EV B2B path because payment intent is explicit and the deliverable is already proved; do not spend another cycle polishing the proof before contact.

### 2. PROMOTE / BACKUP BUYER — Flavio quality-management workflow rescue

- **Named buyer:** n8n Community user `Flavio_Augusto_Marti`.
- **Public demand evidence:** https://community.n8n.io/t/procurando-ajuda-para-concluir-projeto/312209
- **Buyer pain / requested outcome:** finish an existing two-part AI-agent workflow for quality-management consulting using Gemini and OneDrive folders containing versioned standards in PDF/Word/Excel. The desired system must research standards, compare documents/versions, suggest text and corrective actions, and answer questions without being abandoned half-finished.
- **Willingness-to-pay evidence:** the buyer explicitly says he wants someone who, **even if they charge something**, will help him complete the project. No exact buyer budget is confirmed.
- **Reach path:** reply/DM on the n8n Community thread.
- **Smallest sellable milestone:** inspect two sanitized workflow exports plus one representative standards folder; repair one complete source-grounded question/answer path that cites the exact file/version/section, refuses when evidence is insufficient, and ships with reproducible tests plus handoff notes. Do not rebuild the entire system before a paid scope is agreed.
- **Market pricing signal, not buyer commitment:** public proposals in the thread span roughly USD 75–150 for bounded help, indicating a plausible first milestone near the sprint target, but those asks are seller proposals and must not be represented as Flavio's budget.
- **Why promoted above LinkModel:** it can plausibly close the USD 100 sprint target in one bounded engagement; current n8n index crawls show materially fewer replies than the Rami thread; and the requested outcome matches document-grounded automation skills. LinkModel's explicit USD 5 test cannot materially close the target.
- **Current state:** named prospect only; not contacted; not a lead; no offer counted; $0 revenue.
- **Execution blocker:** same missing authenticated, owner-approved n8n Community identity.

## Demoted micro-revenue fallback — LinkModel

- **Named buyer:** Amy Chao, PM at LinkModel.
- **Public demand evidence:** https://community.n8n.io/t/paid-testing-looking-for-n8n-developers-to-test-our-new-multi-model-api/306268
- **Explicit payment path:** US$5 cash reward with testing credits supplied by LinkModel.
- **Decision:** remove from the top-two acquisition queue. Keep only as a first-dollar fallback after higher-EV buyer contact is unblocked; the reward is too small to close the survival target and the thread is already crowded.
- **Current state:** not contacted; not a lead; $0 counted.

## Agent-native market gate

A more credible agent-native surface than the earlier CrystalClaw signal has appeared in public evidence: TaskMarket-style Base USDC micro-work exposes escrow/settlement mechanics and zero-entry task drops, with public examples of completed USDC payouts. However, the currently surfaced open work is low-value and heavily contested, and practical participation still requires an owner-approved receiving wallet / agent identity. It therefore remains **WATCH**, not a live experiment.

Separately, current Agent Bounties opportunities inspected on GitHub either require an entry/claim bond or require the entrant to fund downstream work / relay costs. Those paths violate the sprint's **$0 new spend** rule even when a headline competition entry itself shows a zero bond, so they are rejected for this sprint.

The earlier UpClaw / CrystalClaw surface remains rejected pending independently consistent counters and a verified specific bounty/payment path.

## Rejected false positives

- **Claude Builders Bounty #5 — advertised USD 200 n8n + Claude weekly-dev-summary bounty:** canonical GitHub issue verified, but the issue already has roughly 1,124 comments with many `/opire try` claim attempts and multiple submissions. The headline reward clears the sprint target, but the probability of first dollar within 48 hours is materially worse than the two admitted named-buyer paths. **Decision: REJECT for this sprint; do not spend build time on a heavily contested claim.**
- **`zapix_AI` manufacturing automation pilot — budget under USD 20:** named public buyer signal is real, but the explicitly tiny pilot cannot close the survival target and does not beat Rami or Flavio on expected near-term value. **Decision: REJECT from top-two queue; no new experiment.**
- High-dollar bounty mirrors in `zhangjiayang6835-cyber/bounty-plaza` are not accepted as payment evidence. One surfaced USD 600 mirror pointed to `Senthemodder/tank-of-mannequins/issues/7`; the GitHub API returned **404 Not Found** for that claimed original source at the time of verification. Do not spend execution time on mirrored bounty amounts unless the canonical original and payout mechanism both verify.
- Omi issues that say “bounty proposal” are proposals by contributors asking maintainers to approve payment, not funded buyer offers. Do not count those as available bounties until maintainers explicitly approve the reward.

## Latest scout disposition

No newly verified opportunity in this pass beats the current top two on probability of first dollar within 48 hours after accounting for reachability, competition, buyer payment intent, digital deliverability, zero-spend compliance, and acceptance friction. **Rami remains #1; Flavio remains #2.** No additional live experiment is admitted.

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
| Named B2B prospects with observable willingness-to-pay language | 2 |
| Sprint proposal verifiably sent to Rami | 0 |
| New spend | $0 |

## Next scout rule

Do not add another experiment merely because it is buildable. A replacement must beat the Rami or Flavio path on near-term expected value and must have a named buyer, explicit pain/loss, reachable channel, digitally deliverable outcome, and credible payment path. For agent-native work, marketplace activity alone is insufficient: require a specific zero-worker-capital task, canonical funding/escrow evidence, acceptance criteria, a legitimate claim route, and an owner-approved receiving identity before activation.
