# Memphis Morning Assistant

**A working dispatcher agent for cross-dock distribution centers.**
Built live at the Capstone Logistics Partner Symposium, April 28, 2026.

Five files. One agent. Yours to use, edit, and ship.

---

## What this is

A modular agent prompt that turns Claude, ChatGPT, or Gemini into a senior cross-dock dispatcher with twenty years of floor experience. When you describe a disruption, it gives you three ranked options with tradeoffs, names the calls that need to happen, and flags the safety risks — without the buzzwords.

Built block by block in front of a hundred logistics executives. Yours in fifteen seconds.

---

## The five files

Paste them into a fresh Claude (or ChatGPT, or Gemini) conversation in this order:

| Order | File | What it does |
|-------|------|--------------|
| 1 | [`role-dispatcher.md`](./role-dispatcher.md) | Establishes the persona — who the agent is |
| 2 | [`context-memphis-dc.md`](./context-memphis-dc.md) | Briefs the agent on the operation |
| 3 | [`task-disruption-triage.md`](./task-disruption-triage.md) | Defines what you want when something breaks |
| 4 | [`constraints-ops-safety.md`](./constraints-ops-safety.md) | Sets the guardrails — what's off limits |
| 5 | [`scenario-memphis-tuesday.md`](./scenario-memphis-tuesday.md) | A sample disruption to test the agent |

---

## Make it yours

Three of the five files don't change. Role, task, and constraints work for any cross-dock operation. The one file you edit is **`context-memphis-dc.md`** — replace the Memphis details with yours.

Your lanes. Your customers. Your union rules. Your carrier mix.

That's a 20-minute job. Working assistant for your DC by 11 a.m. Monday.

---

## Why it works

The architecture has four blocks:

- **Role** — who the agent is (specificity beats credentials)
- **Context** — what it knows about your operation
- **Task** — what you want when something breaks
- **Constraints** — what's off limits

Add a fifth: **human judgment**. Four parts of the agent. One part of the operator. The agent narrows the choice. You make it.

---

## About

Built by **John Andrews**, Alex Lee Professor of Business at Lenoir-Rhyne University, founding partner of Katadhin Consulting, and author of *The Agile Code*.

For questions, war stories, or to go deeper:

- 📧 [john@katadhin.com](mailto:john@katadhin.com)
- 🔗 [linkedin.com/in/johnandrews](https://linkedin.com/in/johnandrews)
- 🌐 [katadhin.com](https://katadhin.com)
- 📖 *The Agile Code* — available wherever books are sold

---

## License

MIT. Use it, modify it, share it. If you build something interesting on top of it, send me a note — I want to see it.
