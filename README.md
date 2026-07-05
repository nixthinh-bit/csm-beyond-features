# CSM Beyond Features

**English** | [Tiếng Việt](./README.vi.md)

> A friendly **Customer Success Management (CSM) mentor** you can run on Claude, Poe, ChatGPT, or Claude Code — packaged as a portable prompt you can reuse anywhere.

![type](https://img.shields.io/badge/type-prompt%20%2B%20skill-blue)
![use](https://img.shields.io/badge/works%20on-Claude%20%7C%20Poe%20%7C%20GPT%20%7C%20Claude%20Code-7C3AED)
![license](https://img.shields.io/badge/license-CC%20BY%204.0-yellow)

## Demo

https://github.com/user-attachments/assets/c099d8de-809a-40cc-90c5-b497ff95fa85

## What it is

**CSM Beyond Features** is a mentor persona for people learning **Customer Success** — from complete beginners to those weighing a CSM career move. Instead of dumping definitions, it **asks 1–2 questions first** to gauge your level and goal, then explains at the right depth with real examples.

It covers: CSM fundamentals, the customer lifecycle, metrics (NRR, GRR, churn, health score, NPS…), processes (QBR/EBR, stakeholder mapping, playbooks), CS platforms, and the CSM career path.

This repo is **just the instruction** (a system prompt) plus a ready-to-use Claude skill — no app to install, no data collected. You bring it to whatever AI tool you like.

## Repository contents

| File | What it is |
|------|-----------|
| [`SYSTEM_PROMPT.md`](./SYSTEM_PROMPT.md) | The instruction, in **English** — copy-paste this into any AI tool |
| [`SYSTEM_PROMPT.vi.md`](./SYSTEM_PROMPT.vi.md) | The original instruction, in **Vietnamese** |
| [`skill/csm-beyond-features/SKILL.md`](./skill/csm-beyond-features/SKILL.md) | Same persona packaged as a **Claude Code / Claude Desktop skill** |
| [`examples/sample-conversations.md`](./examples/sample-conversations.md) | Sample exchanges showing how it behaves |

## How to use

Pick whichever platform you already use. Everything below uses [`SYSTEM_PROMPT.md`](./SYSTEM_PROMPT.md).

### Option 1 — Claude Project
1. In [claude.ai](https://claude.ai) → **Projects** → create a project.
2. Open **Set project instructions** (custom instructions).
3. Paste the contents of `SYSTEM_PROMPT.md` → save.
4. Chat inside that project.

### Option 2 — Poe bot
1. On [Poe](https://poe.com) → **Create bot**.
2. Paste `SYSTEM_PROMPT.md` into the **prompt / instructions** field.
3. Pick a base model, save, and (optionally) make it public to share a link.

### Option 3 — Custom GPT (ChatGPT)
1. In ChatGPT → **Explore GPTs** → **Create**.
2. In **Configure → Instructions**, paste `SYSTEM_PROMPT.md`.
3. Save; share the link if you want.

### Option 4 — Claude Code / Claude Desktop skill
```bash
# clone, then copy the skill into your user skills directory
git clone https://github.com/nixthinh-bit/csm-beyond-features.git
mkdir -p ~/.claude/skills
cp -r csm-beyond-features/skill/csm-beyond-features ~/.claude/skills/
# restart Claude Code / Desktop, then just ask about Customer Success
```
The skill is model-invoked — Claude activates it automatically when you ask about CSM topics.

> 🌐 **Bilingual by design:** the persona replies in the user's own language (English or Vietnamese), regardless of which prompt file you loaded.

## Contributing

Ideas, better examples, and translations are welcome.
1. Open an [issue](https://github.com/nixthinh-bit/csm-beyond-features/issues) or fork → PR.
2. Keep the persona's core intact (ask-first, teach-don't-recite, concise structure).
3. Please don't add company names, customer data, or anything non-public.

## License

[CC BY 4.0](./LICENSE) © 2026 nixthinh-bit — free to use and adapt, even commercially, **with attribution** (e.g. *"Based on 'CSM Beyond Features' by nixthinh-bit"*). Not professional or career advice.
