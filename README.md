# Field Guide — Claude

A short, guided set on what Claude is, how to set it up, and how to build with it — for both **teams** (Claude CoWork) and **developers** (Claude Code). Static HTML, served via GitHub Pages.

**Built by [loganmatson.com](https://loganmatson.github.io/loganmatson.com/).**

## Live links

**▶ Start here — [The Pitch](https://loganmatson.github.io/field-guide/)**

| Page | What it is | Link |
|------|------------|------|
| ⭐ The Pitch (start here) | Why Claude Code — the scroll-driven case, served at the root | https://loganmatson.github.io/field-guide/ |
| 🏠 Hub | The card index — pick your path | https://loganmatson.github.io/field-guide/home.html |
| 🎬 Session 1 | 30-min live talk + first skill exercise | https://loganmatson.github.io/field-guide/session.html |
| 02 · Find Your Setup | A 60-second quiz that routes you to the right guide | https://loganmatson.github.io/field-guide/quiz.html |
| → Set Up CoWork | Interactive team-admin setup (7 phases, tips, FAQ, checklist) | https://loganmatson.github.io/field-guide/cowork.html |
| → Set Up Claude Code | Interactive developer setup (CLI, VS Code, GitHub, team) | https://loganmatson.github.io/field-guide/claude-code.html |
| 03 · Build an Agentic Workforce | Skills, memory, pipelines, agent teams (Session 2) | https://loganmatson.github.io/field-guide/business.html |
| 📄 Cheat Sheet (one-pager) | Dense, scannable command + pattern reference | https://loganmatson.github.io/field-guide/cheatsheet.html |
| 🛠 Build Menu (live session) | Ten things to build together, with steps | https://loganmatson.github.io/field-guide/build-menu.html |

## The Pitch — the root landing page

[index.html](https://loganmatson.github.io/field-guide/) is the front door, served at the root URL. A scroll-driven, GSAP-animated case for Claude Code that works for technical and non-technical readers alike:

- **One mechanism, any domain** — five real skills shown by what they do (write in your voice, find your next move, settle a decision with data, run your client work, plan your money), each running the same read → carry memory → run workflow → produce artifact loop
- **One command, a whole week** — a pinned, scroll-scrubbed walkthrough of a six-agent pipeline handing work down the chain
- **The leverage curve, the compounding math, the ROI** — the thesis in numbers
- **The fair questions** — a skeptic's objections answered (Copilot, control, rot)
- **Build your first skill** — the close is an on-ramp, not a sales pitch: get set up → pick one weekly repeat → run the skill-creator → run it and build the next

## Session 1 — the live talk page

[session.html](https://loganmatson.github.io/field-guide/session.html) is a cinematic, presentation-grade page built to drive a 30–35 minute live session:

- **TL;DR popup** — a dismissible 30-second summary card that docks on the right edge (bottom-center on smaller screens) with a jump-to-the-exercise CTA, for cold scanners who want the gist before scrolling
- **Act 1** — 30-second mental model (sous-chef two-panel), then concept ladder: Workflows → Skills → Agents → Pipelines → Empire, one pinned frame per rung
- **Act 2** — Three proofs: the research pipeline maze (animated SVG, opens with a real-world "understand something new by Monday" anchor), the writing skill before/after, and the agent run log
- **Act 3** — Why it matters, the widening gap, two paths (CoWork / Claude Code)
- **Skeptic scoreboard** — the "just a better Copilot" myth is answered with a side-by-side comparison (Copilot: *you drive* every line vs. Claude Code: *it drives* the whole task), not just a claim
- **The exercise** — introduces `skill-creator` with a robot analogy (if you were building 1,000 robots, the first you'd build is the one that builds robots), then walks through a two-part exercise: watch it explain itself, then use it to commission your first real skill saved to `~/.claude/skills/`. Includes a copy-paste rescue `SKILL.md` so a live build never dies on a misfire
- **Close** — CTA to Session 2 (business.html)

Scroll acts as the clicker. Dual-purpose: skimmable for live pacing, readable solo afterward.

## How Part 02 works

Part 02 is a **scored quiz** ([quiz.html](https://loganmatson.github.io/field-guide/quiz.html)) that asks five use-case questions and routes you to one of three places:

- **Claude CoWork** ([cowork.html](https://loganmatson.github.io/field-guide/cowork.html)) — set Claude up for a whole team: shared skills, shared knowledge, admin guardrails. No terminal required.
- **Claude Code** ([claude-code.html](https://loganmatson.github.io/field-guide/claude-code.html)) — the developer setup: Claude in your terminal, VS Code, and GitHub, writing and running real code.
- **Claude.ai** — if you just need a personal account, the quiz points you there.

If your answers point both ways, the quiz shows both guides with the stronger match highlighted. You can also jump straight to either guide from the Hub.

Both setup guides are fully interactive: collapsible sections, copy-to-clipboard commands, tip pills, and a launch checklist. **Every step carries its own FAQ** — 2–3 likely questions per step, each with a direct answer and a "what to do next" line that points to the following step — on top of the global FAQ at the bottom of each guide.

## Structure

```
index.html         The Pitch — root landing, scroll-driven case for Claude Code
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

- **2026-06-20** — Re-added `index.html` (The Pitch) as the root landing page and made it the "start here" entry, ahead of `home.html` and `session.html`. Redid the Act 3 "One mechanism, any domain" examples as five real skills described by what they do (no names), ordered simple → complex, each with parallel mechanism bullets and a "You get ·" outcome line. Reworked the ending from a business pitch into a "build your first skill" on-ramp (four numbered steps; dropped the "Why me" block and the mailto CTA).
- **2026-06-17** — Added per-step FAQ blocks to both setup guides. Each step in `claude-code.html` (Install, VS Code, First project, Memory, GitHub, Team) and each phase in `cowork.html` (Admin, Invite, Skills, Shared project, Guardrails, Memory, Connectors) now ends with 2–3 likely questions — each answered, with a "what to do next" line pointing to the following step. Reuses the existing accordion FAQ pattern in a scoped `.step-faq` variant.
- **2026-06-17** — Refined both session pages from a review pass. `session.html`: added a dismissible 30-second TL;DR popup docked on the right edge (bottom-center on narrow screens, with a re-open handle); reframed Proof 1 to open with a real-world "understand something new by Monday" anchor before the diagram; rebuilt the "just a better Copilot" answer as a balanced *you drive / it drives* side-by-side; added a readability scrim behind the pinned Act scenes so copy stays legible over the drifting particle field; added a copy-paste rescue `SKILL.md` to the exercise. `business.html`: added an inbound "from Session 1" bridge under the hero (you built `/interview`, here's where it lives), and reframed the six-building-blocks lede to call out **hooks** and **MCP** as the two capabilities Copilot has no answer for, with a per-card badge.
- **2026-06-12** — Added 30-second mental model scene (sous-chef two-panel) to `session.html` between hook and concept ladder. Removed `index.html` (Why Claude) from the live site; stored locally. Added `skill-creator` robot analogy section above the exercise.
- **2026-06-12** — Added `skill-creator` robot analogy section to `session.html`: if you were building 1,000 robots and each did one thing well, the first you'd build is the one that builds robots. Tightened CoWork exercise step to save skills to `~/.claude/skills/` globally rather than paste into project instructions.
- **2026-06-11** — Headers locked, proof order swapped (maze → writing → run log), stats row added, exercise rebuilt as instructive two-parter, two-paths visual added.
- **2026-06-10** — New `session.html`: cinematic Session 1 page with Three.js background, concept ladder, three proof sections, skeptic scoreboard, and timed exercise. Repositioned `business.html` as Session 2. Journey-reordered `home.html`. Full de-brand sweep.
- **2026-06-06** — Replaced `how.html` with a routing quiz (`quiz.html`) plus two interactive setup guides (`cowork.html`, `claude-code.html`). Retired `how.html` and `team-setup.html`. Broadened the Hub to a two-audience scope (teams + developers) and added direct CoWork / Claude Code cards.

> Unlisted link (noindex) — please share directly, not publicly.
