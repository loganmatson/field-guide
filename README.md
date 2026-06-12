# Field Guide — Claude

A short, guided set on what Claude is, how to set it up, and how to build with it — for both **teams** (Claude CoWork) and **developers** (Claude Code). Static HTML, served via GitHub Pages.

**Built by [loganmatson.com](https://loganmatson.github.io/loganmatson.com/).**

## Live links

**▶ Start here — [The Hub](https://loganmatson.github.io/field-guide/home.html)**

| Page | What it is | Link |
|------|------------|------|
| 🏠 Hub (start here) | The card index — pick your path | https://loganmatson.github.io/field-guide/home.html |
| 🎬 Session 1 | 30-min live talk + first skill exercise | https://loganmatson.github.io/field-guide/session.html |
| 02 · Find Your Setup | A 60-second quiz that routes you to the right guide | https://loganmatson.github.io/field-guide/quiz.html |
| → Set Up CoWork | Interactive team-admin setup (7 phases, tips, FAQ, checklist) | https://loganmatson.github.io/field-guide/cowork.html |
| → Set Up Claude Code | Interactive developer setup (CLI, VS Code, GitHub, team) | https://loganmatson.github.io/field-guide/claude-code.html |
| 03 · Build an Agentic Workforce | Skills, memory, pipelines, agent teams (Session 2) | https://loganmatson.github.io/field-guide/business.html |
| 📄 Cheat Sheet (one-pager) | Dense, scannable command + pattern reference | https://loganmatson.github.io/field-guide/cheatsheet.html |
| 🛠 Build Menu (live session) | Ten things to build together, with steps | https://loganmatson.github.io/field-guide/build-menu.html |

## Session 1 — the live talk page

[session.html](https://loganmatson.github.io/field-guide/session.html) is a cinematic, presentation-grade page built to drive a 30–35 minute live session:

- **Act 1** — 30-second mental model (sous-chef two-panel), then concept ladder: Workflows → Skills → Agents → Pipelines → Empire, one pinned frame per rung
- **Act 2** — Three proofs: the health pipeline maze (animated SVG), the writing skill before/after, and the agent run log
- **Act 3** — Why it matters, the widening gap, two paths (CoWork / Claude Code)
- **The exercise** — introduces `skill-creator` with a robot analogy (if you were building 1,000 robots, the first you'd build is the one that builds robots), then walks through a two-part exercise: watch it explain itself, then use it to commission your first real skill saved to `~/.claude/skills/`
- **Close** — CTA to Session 2 (business.html)

Scroll acts as the clicker. Dual-purpose: skimmable for live pacing, readable solo afterward.

## How Part 02 works

Part 02 is a **scored quiz** ([quiz.html](https://loganmatson.github.io/field-guide/quiz.html)) that asks five use-case questions and routes you to one of three places:

- **Claude CoWork** ([cowork.html](https://loganmatson.github.io/field-guide/cowork.html)) — set Claude up for a whole team: shared skills, shared knowledge, admin guardrails. No terminal required.
- **Claude Code** ([claude-code.html](https://loganmatson.github.io/field-guide/claude-code.html)) — the developer setup: Claude in your terminal, VS Code, and GitHub, writing and running real code.
- **Claude.ai** — if you just need a personal account, the quiz points you there.

If your answers point both ways, the quiz shows both guides with the stronger match highlighted. You can also jump straight to either guide from the Hub.

Both setup guides are fully interactive: collapsible sections, copy-to-clipboard commands, tip pills, inline FAQs, and a launch checklist.

## Structure

```
home.html          Hub — card index, links out to loganmatson.com
session.html       Session 1 — cinematic 30-min talk + skill exercise
quiz.html          Part 02 — Find Your Setup (scored router)
cowork.html        Setup guide — teams (CoWork admin)
claude-code.html   Setup guide — developers (Claude Code)
business.html      Session 2 / Part 03 — Build an Agentic Workforce
cheatsheet.html    Reference — one-pager
build-menu.html    Live session — build menu
```

Pure static HTML + vanilla JS — no build step, no dependencies. Every page carries `noindex, nofollow`.

## Changelog

- **2026-06-12** — Added 30-second mental model scene (sous-chef two-panel) to `session.html` between hook and concept ladder. Removed `index.html` (Why Claude) from the live site; stored locally. Added `skill-creator` robot analogy section above the exercise.
- **2026-06-12** — Added `skill-creator` robot analogy section to `session.html`: if you were building 1,000 robots and each did one thing well, the first you'd build is the one that builds robots. Tightened CoWork exercise step to save skills to `~/.claude/skills/` globally rather than paste into project instructions.
- **2026-06-11** — Headers locked, proof order swapped (maze → writing → run log), stats row added, exercise rebuilt as instructive two-parter, two-paths visual added.
- **2026-06-10** — New `session.html`: cinematic Session 1 page with Three.js background, concept ladder, three proof sections, skeptic scoreboard, and timed exercise. Repositioned `business.html` as Session 2. Journey-reordered `home.html`. Full de-brand sweep.
- **2026-06-06** — Replaced `how.html` with a routing quiz (`quiz.html`) plus two interactive setup guides (`cowork.html`, `claude-code.html`). Retired `how.html` and `team-setup.html`. Broadened the Hub to a two-audience scope (teams + developers) and added direct CoWork / Claude Code cards.

> Unlisted link (noindex) — please share directly, not publicly.
