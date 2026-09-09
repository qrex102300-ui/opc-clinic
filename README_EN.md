# OPC Clinic

![License](https://img.shields.io/badge/license-MIT-blue)
![Version](https://img.shields.io/badge/version-v0.1-lightgrey)
![Models](https://img.shields.io/badge/models-Claude%20%7C%20ChatGPT%20%7C%20Gemini%20%7C%20DeepSeek-green)

> An AI diagnostician that **interrogates** your one-person-company. It refuses generic advice and digs until it finds the real cause you've been avoiding.

**Who it's for**: Solo founders, indie developers, and micro-team founders (at the 0→1 or 1→100 stage) who've been building for a while and are stuck somewhere they can't quite articulate. You've already started — you're not still picking ideas.

**How it's different from just asking ChatGPT / Claude**: General-purpose LLMs default to telling you what you want to hear. This diagnostician is bound by a strict discipline — symptoms must be traced to root causes, every conclusion must be anchored to a specific fact you've stated, and multi-turn conversations are not allowed to drift into comfort. It's uncomfortable. That's the point.

---

## Founding Beta · Post-launch Founder Debugging

**Built it. People try it. Nobody pays?**

The open-source OPC Clinic stays free under MIT. The founding beta adds a different layer for founders who already have reality to inspect: bring actual visits, signups, trials, calls, rejections, usage, or revenue, and the diagnosis is cross-checked against current competitors, customer complaints, pricing, and substitutes before turning into a 7-day test.

**$0 bottleneck triage → $59 USDC accepted diagnosis · 3 founding-beta slots.**

No sales call. No subscription. No 40-page generic report. Start with the free triage; payment is requested only after the case is accepted. The paid diagnosis targets delivery within 24 hours after payment and complete context.

[Open the live free bottleneck triage →](https://qrex102300-ui.github.io/opc-clinic/paid-diagnosis.html) · [See the exact paid sample →](./SAMPLE_PAID_DIAGNOSIS.md) · [Follow the public $0 → $100 self-funding sprint →](./SELF_FUNDING_SPRINT.md)

---

## What This Is (and Isn't)

- ✅ A **carefully crafted prompt / skill** that codifies the ability to "interrogate on the spot and see through bullshit at a glance"
- ✅ **Fully local**: You load it into your own Claude / ChatGPT / any LLM. Your data stays with you end-to-end, never passes through any third party
- ✅ Open source, free, forkable, and improvable
- ❌ Not a SaaS — collects none of your data
- ❌ Not a replacement for real market validation — it helps you figure out what to validate, but you still have to do the validation yourself

---

## 60-Second Quick Start

The diagnostic power is a prompt inside [`prompt/diagnostician.md`](prompt/diagnostician.md) — **it's model-agnostic and platform-independent**. Claude / ChatGPT / DeepSeek / Gemini / Kimi / Qwen and more can all run it.

**Method A · Copy & Paste (Any LLM, Simplest)**

1. Copy the entire contents of [`prompt/diagnostician.md`](prompt/diagnostician.md)
2. Open any LLM you use (Claude / ChatGPT / DeepSeek / Gemini / Kimi / Qwen, etc.) and start a new conversation
3. Paste it in as the first message and send
4. It'll reply with "The clinic is open — tell me your situation" — then, act like a real case owner: **don't go along with it, push back when you disagree**, and go with it

**Method B · Claude Code Skill (One-Click Reuse)**

Drop the `skill/` directory into your Claude Code skills folder. After that, saying "diagnose my project" automatically triggers it. See [Installation Guide](README-skill.md) for details.

**Method C · Claude Project Custom Instructions**

Create a new Claude Project, paste `diagnostician.md` into custom instructions. One-click access from then on.

> 🌐 **Works with any model**: It's just a prompt, not tied to any platform. That said, its soul is "multi-turn interrogation that holds firm against your pushback" — and this is precisely what stresses a model's reasoning and multi-turn ability most. **The stronger the model, the sharper the diagnosis**; use the strongest tier each provider offers, not the lite / fast versions.

**Advanced (technical users)**

- Use `prompt/diagnostician.md` as a system prompt in your own API calls
- Or wrap it as a Cursor / other AI coding tool rule and invoke it anytime in your dev workflow

---

## How Brutal Is It · A Real Diagnosis (Excerpt)

> Below is a real excerpt from when it diagnosed **my own startup project**. I'm its author, and it gave me no mercy.
> *(Full conversation in [`examples/founder-self-diagnosis.md`](examples/founder-self-diagnosis.md))*

```
Founder: I built an AI startup diagnostic tool. It's been over three months.
   People come and ask questions, some say it's good, but no one pays.
   What makes me doubt myself more is — my own product, run through its
   own diagnostic flow, produces worse conclusions than just chatting with
   Claude for half an hour. If it can't even beat 30 minutes with an LLM,
   have I already failed?

Diagnostician: Stop right there. "If it can't beat 30 minutes with an LLM,
   it's a failure" — I'm not going to engage with that yet, because I suspect
   your benchmark was crooked from the start.
   That person who "chatted with Claude for half an hour and got a great
   conclusion" — was that you, or a real small-business owner who can't even
   articulate where they're stuck? You're in this field. You know what to ask.
   Take that same blank prompt and hand it to your target customer — can they
   get the same conclusions you got?
   If they can't, what you're comparing is not "product vs. LLM," it's
   "you the expert vs. your product" — and that contest was never fair.

   ...(It endured every counter-argument from its author, interrogating for
   over a dozen rounds, then delivered this diagnosis)

   Real cause: You bet your product's value on two things LLMs already do
   better than you — "diagnostic conclusions" and a "case library." And the
   one truly scarce asset you have — your own ability to interrogate on the
   spot and see through bullshit at a glance — you not only failed to
   productize, you actively replaced it with a static form. For weeks, you've
   been meticulously building a shoddy knockoff of your only moat.
```

> This diagnosis single-handedly made me scrap 5 weeks of engineering direction. **If a tool can convince its own author, it probably has something for you too.**

---

## Why "Asking Better Questions" Beats "Giving Better Answers"

LLMs can generate questions and conclusions. The one thing they **cannot** do reliably is embody this stance:

- **No pandering** — What you want to hear ≠ the right answer. If the direction is wrong, it says so.
- **No accepting vagueness** — "No traffic" and "low conversion" are symptoms, not causes. Dig until you can't dig further.
- **Every conclusion pinned to a fact** — No universally-true-for-everyone platitudes. If the sentence still holds when you swap in a different founder, delete and rewrite.
- **No multi-turn drift** — The longer a conversation goes, the stronger the pull to make you comfortable — that's the most dangerous drift. This diagnostician is nailed to "only finding the cause."

That stance is the entire value of this prompt.

---

## Repository Structure

```
opc-clinic/
├── README.md                          # Chinese + beta entry point
├── README_EN.md                       # English version
├── PAID_DIAGNOSIS.md                  # Paid beta scope
├── SAMPLE_PAID_DIAGNOSIS.md           # Transparent sample deliverable
├── SELF_FUNDING_SPRINT.md              # Public revenue experiment scorecard
├── prompt/
│   └── diagnostician.md               # Core: the diagnostician prompt (copy this to use)
├── examples/
│   ├── founder-self-diagnosis.md      # Real demo: full conversation of it diagnosing its author
│   ├── saas-founder-diagnosis.md      # SaaS founder: free users, zero paid conversion
│   ├── content-creator-diagnosis.md   # Content creator: stuck at 5K followers
│   └── ecommerce-diagnosis.md         # E-commerce: products sell once, then die
├── CONTRIBUTING.md                    # How to contribute
└── LICENSE                            # MIT
```

---

## Help Me Sharpen It Further · I Want Your Feedback

This is v0.1. For now it only validates one thing: **does this interrogation-style diagnosis actually work for a real person like you?**

After running a diagnosis on your project, **come to [Issues](../../issues) and tell me** (even just one line):

- **Which cut hit home?** — What question did it ask that you'd never asked yourself?
- **Which cut missed?** — Where did it chase the wrong lead or give you a platitude?
- **What stage and industry are you in?** — Helps me know where it lands better

> Every piece of real feedback goes directly into the next iteration. This project's moat isn't in code — it's in how many real founders have used it, cursed at it, and improved it.
> If you build something better on top of it, **fork away — and also come back and tell me what you changed. I'll probably learn from you.**

---

## Roadmap (Depends on Feedback)

- [ ] Multi-language versions (English first, to reach the broader indie hacker world)
- [ ] Diagnostic branches tailored to different stages (0→1 / 1→100)
- [ ] Auto-generate "actionable next steps + exit criteria" at the end of each diagnosis
- [ ] (Maybe) a web version that works out of the box without configuring your own API — if enough people ask

---

## License

MIT — Use it freely, modify it freely, use it commercially. One request: if it helps you, drop a line in the Issues section. Let me know it's actually useful, not just another repo that gets starred and forgotten.

---

*The author is publicly documenting this project's 0→1 journey. If you're also building a one-person company and stuck at the "built it but no one's buying" halfway point, welcome aboard.*
