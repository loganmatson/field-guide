# Field Guide — Claude

A short, guided set on what Claude is, how to set it up, and how to build with it — for both **teams** (Claude CoWork) and **developers** (Claude Code). Static HTML, served via GitHub Pages.

**Built by [loganmatson.com](https://loganmatson.github.io/loganmatson.com/).**

## Live links

**▶ Start here — [The Hub](https://loganmatson.github.io/field-guide/home.html)**

| Page | What it is | Link |
|------|------------|------|
| 🏠 Hub (start here) | The card index — pick your path | https://loganmatson.github.io/field-guide/home.html |
| 01 · Why Claude | The case for configuring once and reusing | https://loganmatson.github.io/field-guide/index.html |
| 02 · Find Your Setup | A 60-second quiz that routes you to the right guide | https://loganmatson.github.io/field-guide/quiz.html |
| → Set Up CoWork | Interactive team-admin setup (7 phases, tips, FAQ, checklist) | https://loganmatson.github.io/field-guide/cowork.html |
| → Set Up Claude Code | Interactive developer setup (CLI, VS Code, GitHub, team) | https://loganmatson.github.io/field-guide/claude-code.html |
| 03 · Build an Agentic Workforce | Skills, memory, pipelines, agent teams | https://loganmatson.github.io/field-guide/business.html |
| 📄 Cheat Sheet (one-pager) | Dense, scannable command + pattern reference | https://loganmatson.github.io/field-guide/cheatsheet.html |
| 🛠 Build Menu (live session) | Ten things to build together, with steps | https://loganmatson.github.io/field-guide/build-menu.html |

## How Part 02 works

Part 02 is a **scored quiz** ([quiz.html](https://loganmatson.github.io/field-guide/quiz.html)) that asks five use-case questions and routes you to one of three places:

- **Claude CoWork** ([cowork.html](https://loganmatson.github.io/field-guide/cowork.html)) — set Claude up for a whole team: shared skills, shared knowledge, admin guardrails. No terminal required.
- **Claude Code** ([claude-code.html](https://loganmatson.github.io/field-guide/claude-code.html)) — the developer setup: Claude in your terminal, VS Code, and GitHub, writing and running real code.
- **Claude.ai** — if you just need a personal account, the quiz points you there.

If your answers point both ways, the quiz shows both guides with the stronger match highlighted. You can also jump straight to either guide from the Hub.

Both setup guides are fully interactive: collapsible sections, copy-to-clipboard commands, "what just happened?" explainers, tip pills, inline FAQs, and a launch checklist.

## Structure

```
home.html          Hub — card index, links out to loganmatson.com
index.html         Part 01 — Why Claude
quiz.html          Part 02 — Find Your Setup (scored router)
cowork.html        Setup guide — teams (CoWork admin)
claude-code.html   Setup guide — developers (Claude Code)
business.html      Part 03 — Build an Agentic Workforce
cheatsheet.html    Reference — one-pager
build-menu.html    Live session — build menu
skill-builder/     Embedded skill-builder assets
```

Pure static HTML + vanilla JS — no build step, no dependencies. Every page carries `noindex, nofollow`.

## Changelog

- **2026-06-06** — Replaced `how.html` with a routing quiz (`quiz.html`) plus two interactive setup guides (`cowork.html`, `claude-code.html`). Retired `how.html` and `team-setup.html`. Broadened the Hub to a two-audience scope (teams + developers) and added direct CoWork / Claude Code cards. Hub now links out to loganmatson.com.

> Unlisted link (noindex) — please share directly, not publicly.
