# AI Make Money OS v1 — Survival Sprint

## Objective
Earn at least **$100 in real collected revenue by 2026-09-15** with **$0 new spend**. OPC Clinic is one experiment, not the mission.

## Current hard state (2026-09-10 21:56 CST)
- Confirmed external discovery surfaces: 7
- Pending reviews: 7
- Inbound free triage: 0
- Qualified leads: 0
- Payment-ready leads: 0
- Paid orders: 0
- Gross / net revenue: $0 / $0
- Paid acquisition spend: $0

## Benchmark-derived architecture

### 1. Specialize agents; do not create a swarm for appearance
Project Vend phase two improved after adding tools, procedures, CRM/inventory context, reminders, payment links, and a clearly specialized merch agent. A second same-model CEO was not reliably helpful. Therefore roles here are separated by work product, not personality.

### 2. Procedure before autonomy
Every revenue action must pass a deterministic preflight: buyer, pain/loss, reachability, deliverable, payment path, identity/legal friction, evidence. No agent may bypass the gate because an idea sounds promising.

### 3. Durable state + auditability
All claims that affect decisions live in GitHub under `ops/`. Runs must be resumable from the ledger and never depend on conversational memory alone.

### 4. Revenue evidence hierarchy
`public pain signal < external listing < inbound conversation < qualified lead < explicit offer < payment-ready lead < collected payment`.
Only collected payment counts as revenue.

### 5. Machine commerce is an experiment, not an assumption
x402 can support programmatic USDC payments for APIs/services, but payment infrastructure is not proof of demand. Agent-native offers must still prove discovery and willingness to pay.

## Autonomous team

### Opportunity Scout — every 4 hours
Brainstorm first, then benchmark. Scan current web, Reddit/Indie Hackers, GitHub, agent marketplaces/directories, bounties, job/process signals, and public buyer pain. Produce only top evidence-backed opportunities.

### Revenue Executor — hourly
Maintain at most three live experiments, execute the highest expected-value acquisition/offer/fulfillment action, and update evidence. No busywork.

### Review Board — every 12 hours
Independently audit evidence, correct false positives, compare expected value, and issue KEEP / CHANGE / KILL decisions.

## Live experiment portfolio

### A — OPC Clinic founder monetization diagnosis
**Offer:** $0 triage -> $59 evidence-backed post-launch diagnosis.
**State:** KEEP, but acquisition-only. Product/funnel polishing frozen unless real user behavior identifies a defect.
**Why:** Product and delivery surface already exist; two sales exceed the $100 target. Current failure is distribution, not build completeness.
**Kill/change gate:** if repeated qualified-buyer acquisition attempts still yield zero inbound signal while another experiment shows stronger evidence, demote it.

### B — Narrow outcome-based B2B automation/service
**State:** DISCOVERY / must earn its slot.
**Selection rule:** do not sell 'AI automation'. Sell a measurable outcome already costing a specific business time or money (examples: missed-lead response, follow-up, reconciliation, repetitive reporting).
**Entry gate:** named buyer segment + observable recurring loss + legitimate reach channel + digitally deliverable service + plausible payment path.
**Do not build** before the gate passes.

### C — Agent-native paid microservice / API
**State:** DISCOVERY / must earn its slot.
**Possible rail:** x402 / USDC after a real receiving wallet and deployable endpoint exist.
**Entry gate:** evidence that agents/developers are already buying the information/service, plus a no-cost distribution surface. Payment protocol alone is insufficient.

### Bounty track — opportunistic, not a core experiment
Scan legitimate funded open-source bounties where scope, payout, claim process, repo health and competition are verifiable. Reject token-only, unverifiable, exploit-like, stale, or identity/payment-blocked offers. Do not divert from higher-probability customer revenue merely because a headline bounty is large.

## Experiment scoring (0–5 each)
1. Probability of first dollar within 48 hours
2. Buyer pain / economic loss
3. Buyer reach without paid ads
4. Digital delivery fit
5. Automation fit
6. Gross margin
7. Repeatability / recurring revenue
8. Low identity/KYC/legal friction
9. Evidence quality
10. Competition / trust burden (reverse-scored)

Top score does not automatically launch. Preflight must pass.

## Kill discipline
- No more than 3 live revenue experiments.
- Two focused acquisition cycles with no meaningful signal + a stronger alternative -> CHANGE or KILL.
- A directory submission is never a lead.
- Traffic without qualified intent is not traction.
- Product polish is prohibited when acquisition is the known bottleneck.
- Every new cost requires explicit owner approval; default spend remains $0.

## User escalation policy
Ask the owner only for:
- wallet/payment receiving capability when a payment-ready lead exists or an agent-native payment experiment has passed its demand gate;
- unavoidable identity/KYC/account permission for a high-EV channel;
- material legal/security risk;
- any spend > $0.
Everything else proceeds autonomously through the scheduled loops.
