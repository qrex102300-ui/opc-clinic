# OPC Clinic

![License](https://img.shields.io/badge/license-MIT-blue)
![Version](https://img.shields.io/badge/version-v0.1-lightgrey)
![Models](https://img.shields.io/badge/models-Claude%20%7C%20ChatGPT%20%7C%20Gemini%20%7C%20DeepSeek-green)

> An AI diagnostician that **interrogates** your one-person-company. It refuses generic advice and digs until it finds the real cause you've been avoiding.

**Who it's for**: Solo founders, indie developers, and micro-team founders (at the 0→1 or 1→100 stage) who've been building for a while and are stuck somewhere they can't quite articulate. You've already started — you're not still picking ideas.

**How it's different from just asking ChatGPT / Claude**: General-purpose LLMs default to telling you what you want to hear. This diagnostician is bound by a strict discipline — symptoms must be traced to root causes, every conclusion must be anchored to a specific fact you've stated, and multi-turn conversations are not allowed to drift into comfort. It's uncomfortable. That's the point.

---

## What This Is (and Isn't)

- ✅ A **carefully crafted prompt / skill** that codifies the ability to "interrogate on the spot and see through bullshit at a glance"
- ✅ **Fully local**: You load it into your own Claude / ChatGPT / any LLM. Your data stays with you end-to-end, never passes through any third party
- ✅ Open source, free, forkable, and improvable
- ❌ Not a SaaS — collects none of your data
- ❌ Not a replacement for real market validation — it helps you figure out what to validate, but you still have to do the validation yourself

---

## 60-Second Quick Start

**The simplest way (anyone can use it, no code required)**

1. Copy the entire contents of [`prompt/diagnostician.md`](prompt/diagnostician.md)
2. Open [Claude](https://claude.ai) (recommended) or ChatGPT and start a new conversation
3. Paste it in as the first message and send
4. It'll reply with "The clinic is open — tell me your situation" — then, act like a real case owner: **don't go along with it, push back when you disagree**, and go with it

> 💡 For stabler results: save it as a Claude [Project](https://www.anthropic.com/news/projects) custom instruction, or as a custom GPT in ChatGPT, for one-click access later.

> 🌐 **Works with any model**: Claude / ChatGPT / Gemini / DeepSeek / Kimi / Qwen and more can all run it — it's just a prompt, not tied to any specific platform.
> That said, its soul is "multi-turn interrogation that holds firm against your pushback" — and this is precisely what stresses a model's reasoning and multi-turn ability most. **The stronger the model, the sharper the diagnosis**; use the strongest tier each provider offers, not the lite / fast versions.

**Advanced (technical users)**

- Use `prompt/diagnostician.md` as a system prompt in your own API calls
- Or wrap it as a Claude Code / Cursor skill and invoke it anytime in your dev workflow

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
├── README.md                          # You're reading this (Chinese)
├── README_EN.md                       # English version
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
