# FLOW

**A solo creator operating system for building software with AI agents.**

One person. Massive scope. No dropped threads.

---

## Install

1. Download `flow.plugin` from the [latest release](https://github.com/binkybink1/FLOW/releases/latest)
2. Open Claude Code → Settings → Plugins → Install from file
3. Select `flow.plugin` — install at **user scope** so it's available in every project

That's it. FLOW is ready.

---

## Start a project

Open your project folder in Claude Code, then pick the path that matches what you actually have.

### You have chaos
Ideas in your head, scattered notes, half-formed thoughts.

```
/spinup
```
Dump everything — text, links, attachments. No questions asked. Repeat as many times as you need across as many sessions as you want. When you're ready:

```
/crystallize
```
FLOW reads the inbox, asks for anything blocking (usually just the project name), and scaffolds everything: brief, hub, dashboard, folder structure.

### You have an idea but it's unstructured
You can describe it, just not in bullet points.

```
/project-strategy
```
Brain-dump in one shot. FLOW distills it into `docs/product-brief.md` and sets up the hub.

### You know the shape
You have a name, a stack, a deadline.

```
/new-project
```
FLOW asks a few structured questions and scaffolds immediately.

---

## The daily loop

**Morning** — say: `morning kickoff`

FLOW reads your hub, surfaces your active milestone, flags blockers, and gives you a focused top-3 plan for the session.

**During work** — capture as you go:

| Say | Goes to |
|---|---|
| `"note: never use X"` | Rules |
| `"bug: login crashes on empty submit"` | Known bugs |
| `"decision: using Supabase not Firebase"` | Decisions |
| `"add to backlog: dark mode"` | Backlog |

**End of session** — say: `session close`

FLOW updates the hub, logs completed tasks, syncs the dashboard, and asks if you want evening research.

---

## Serve the dashboard

```bash
cd your-project-folder
npx serve . -l 3000
```

Open `http://localhost:3000` — the dashboard reads `PROJECT_HUB.json` live.

---

## What's in the box

| | |
|---|---|
| `/spinup` + `/crystallize` | Chaos-first kickoff |
| `/new-project` | Structured kickoff |
| `/project-strategy` | Idea-to-brief kickoff |
| Morning kickoff | Daily briefing |
| Session closeout | Hub sync + history |
| Note capture | Routes notes mid-session |
| Doc sync | Keeps docs in sync as decisions are made |
| Gantt | Generates visual timeline from your docs |
| Evening research | Briefs you before the next session |

---

FLOW v2.1.0 — built for solo creators running high-volume agent sessions.
