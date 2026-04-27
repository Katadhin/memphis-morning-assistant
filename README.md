<div align="center">

<br>

# 🚛 Memphis Morning Assistant

### *A working dispatcher agent for cross-dock distribution centers.*

**Five files. One agent. Yours to use, edit, and ship.**

<br>

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Built at Capstone 2026](https://img.shields.io/badge/Built%20at-Capstone%202026-1A2942?style=for-the-badge)](https://katadhin.com)
[![The Agile Code](https://img.shields.io/badge/Read%20the%20book-The%20Agile%20Code-C89152?style=for-the-badge)](https://katadhin.com)
[![Made by Katadhin](https://img.shields.io/badge/Made%20by-Katadhin-1A2942?style=for-the-badge)](https://katadhin.com)

<br>

[**🚀 Try it in Claude**](https://claude.ai) · [**🤖 Try it in ChatGPT**](https://chatgpt.com) · [**✨ Try it in Gemini**](https://gemini.google.com)

<br>

*Built live in front of 100 logistics executives at the Capstone Logistics Partner Symposium · April 28, 2026*

<br>

---

</div>

<br>

## 📋 Table of Contents

- [What this is](#what-this-is)
- [Why it works](#why-it-works)
- [Quick start](#-quick-start)
- [Make it yours](#-make-it-yours)
- [What's in this repo](#-whats-in-this-repo)
- [Going deeper](#-going-deeper)
- [About](#-about)
- [Connect](#-connect)

<br>

## What this is

A modular agent prompt that turns Claude, ChatGPT, or Gemini into a senior cross-dock dispatcher with twenty years of floor experience.

When you describe a disruption, it gives you **three ranked options** with tradeoffs called out, **names the calls** that need to happen, and **flags the safety risks** — all in operator language. No buzzwords. No frameworks. No fluff.

> *"Built block by block in front of a hundred logistics executives. Yours in fifteen seconds."*

<br>

## Why it works

The architecture has four blocks. Add a fifth — your judgment — and you have a working system.

| | Block | What it does | Where it lives |
|---|---|---|---|
| 1️⃣ | **Role** | Establishes who the agent is. Specificity beats credentials. | [`role-dispatcher.md`](./role-dispatcher.md) |
| 2️⃣ | **Context** | Briefs the agent on your operation. Lanes, customers, crew, rules. | [`context-memphis-dc.md`](./context-memphis-dc.md) |
| 3️⃣ | **Task** | Defines what you want when something breaks. Three options, ranked. | [`task-disruption-triage.md`](./task-disruption-triage.md) |
| 4️⃣ | **Constraints** | Sets the guardrails. SLA flagging, OT rules, escalation triggers. | [`constraints-ops-safety.md`](./constraints-ops-safety.md) |
| ✋ | **Judgment** | The fifth block. *Yours.* The agent narrows the choice. **You make it.** | — |

<br>

## 🚀 Quick start

Open a fresh chat in your AI tool of choice. Paste the five files **in this order** — one at a time, waiting for the agent to acknowledge each before moving on.

```bash
1. role-dispatcher.md           →  who the agent is
2. context-memphis-dc.md        →  what your operation looks like
3. task-disruption-triage.md    →  what you want when something breaks
4. constraints-ops-safety.md    →  what's off limits
5. scenario-memphis-tuesday.md  →  a sample disruption to test
```

By the fifth paste, you'll have a working dispatcher giving you three ranked options with tradeoffs, calls to make, and safety flags.

<details>
<summary><b>📺 What you'll see when it works</b></summary>

<br>

After pasting all five blocks, ask the agent a real disruption — *"It's 6:12 a.m. Tuesday. Atlanta inbound is two hours behind. What are my options?"* — and you'll get back something like this:

> **Option 1: Hold and run lean** *(low cost, moderate SLA risk)*
> **Option 2: Pull from Retailer B trailer** *(moderate cost, low SLA risk)*
> **Option 3: Spot market truck** *(ALERT: high cost, high SLA risk)*
>
> Each option includes the call to make, who makes it, and the most likely failure mode.

The agent will also flag safety concerns, identify the customer call that needs to happen, and ask one clarifying question if it doesn't have enough information.

</details>

<br>

## 🛠 Make it yours

> ⚡ **Three of the five files don't change.** Role, task, and constraints work for any cross-dock operation.

The one file you edit is **[`context-memphis-dc.md`](./context-memphis-dc.md)**. Replace the Memphis details with yours:

- ✅ Your inbound lanes
- ✅ Your outbound customers and SLA windows
- ✅ Your crew composition and union rules
- ✅ Your carrier mix
- ✅ Your visibility gaps and tooling realities

**Twenty minutes of editing. Working assistant for your DC by 11 a.m. Monday.**

<br>

## 📁 What's in this repo

```
memphis-morning-assistant/
│
├── 📄 README.md                     ← you are here
│
├── 🎭 role-dispatcher.md            ← block 1 — the persona
├── 📍 context-memphis-dc.md         ← block 2 — the operation
├── 🎯 task-disruption-triage.md     ← block 3 — the request
├── 🛡  constraints-ops-safety.md    ← block 4 — the guardrails
│
└── 🧪 scenario-memphis-tuesday.md   ← test scenario — feed this last
```

<br>

## 🔬 Going deeper

Each file is heavily commented and short enough to read in under two minutes.

<details>
<summary><b>🎭 Start with the role file</b></summary>

The role file establishes the agent's persona — twenty years of floor experience, calm under pressure, thinks in tradeoffs. The trick: specificity beats credentials. *"Senior dispatcher at a Memphis cross-dock"* outperforms *"supply chain expert"* every time.

</details>

<details>
<summary><b>🛡 Then read the constraints file</b></summary>

The constraints file is where the magic happens. Ten rules that turn the agent from a confident bullshitter into a thoughtful collaborator. The most important one: *"If you don't have enough information, ask one clarifying question first."*

</details>

<details>
<summary><b>🚀 Want to extend it?</b></summary>

A few directions worth exploring:

- **Domain-specific context blocks** — `context-yard-management.md`, `context-driver-relations.md`, etc. The role and constraints stay constant.
- **Scenario libraries** — build a folder of `scenario-*.md` files for the disruptions you face most. Run them as a regression test when you change the prompt.
- **Compose with other agents** — the dispatcher is one role. The same architecture works for procurement, account management, fleet maintenance, even customer success.

</details>

<br>

## 👤 About

Built by **John Andrews**

🎓 Alex Lee Professor of Business at Lenoir-Rhyne University
🤝 Founding partner at Katadhin Consulting
📖 Author of *The Agile Code*

The framework behind this prompt — **Knowledge, Instructions, Tools, Triggers, and Human Judgment** — is the operating model from *The Agile Code*. This repo is one applied example. There are many more.

<br>

## 💬 Connect

<div align="center">

[![Email](https://img.shields.io/badge/Email-john@katadhin.com-1A2942?style=for-the-badge&logo=gmail&logoColor=white)](mailto:john@katadhin.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-katadhin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/katadhin)
[![Website](https://img.shields.io/badge/Website-katadhin.com-C89152?style=for-the-badge&logo=safari&logoColor=white)](https://katadhin.com)
[![Book](https://img.shields.io/badge/Read-The_Agile_Code-1A2942?style=for-the-badge&logo=bookstack&logoColor=white)](https://katadhin.com)

</div>

<br>

## 📜 License

**MIT.** Use it. Modify it. Ship it.

If you build something interesting on top of it, send me a note. I want to see what you do with it.

<br>

---

<div align="center">

### ⚡ *Built for operators, by an operator.*

<br>

⭐ **If this saved you a Monday morning, star the repo.**

<br>

</div>
