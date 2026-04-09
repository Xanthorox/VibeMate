<div align="center">

<img src="https://img.shields.io/badge/VibeMate-AI%20Coding%20Agent-7C3AED?style=for-the-badge" />

# VibeMate

### An autonomous AI coding agent that lives in your Telegram.

*Send a prompt. Get working code. No IDE. No terminal. No setup.*

## 👉 [**Try it free → @Xanthorox_bot**](https://t.me/Xanthorox_bot)

> **Free to use.** Just open the bot and send `/start` — no account, no payment, no setup required.

---

[![Live](https://img.shields.io/badge/Bot-Live%20Now-22c55e?style=flat-square&logo=telegram)](https://t.me/Xanthorox_bot)
[![Free](https://img.shields.io/badge/Access-Free-22c55e?style=flat-square)](#)
[![Agent](https://img.shields.io/badge/Agent-Autonomous-7C3AED?style=flat-square)](#)
[![Model](https://img.shields.io/badge/Model-Xanthorox%20AI-FF6B35?style=flat-square)](#)

</div>

---

VibeMate is an **autonomous coding agent on Telegram**. It doesn't just answer questions about code — it writes it, runs it, fixes it, and delivers the result as a working project. You talk to it like a developer, and it works like one.

---

## What It Does

```
You:        "Build a FastAPI backend with JWT auth and a SQLite user database"

VibeMate:   ✏️  Writing project structure...
            📦  Installing dependencies...
            ✏️  Writing main.py, auth.py, models.py...
            🔧  Running tests...
            ✅  Done — 9 files changed

            [📁 project.zip — 14.2 KB]
```

That's one message. One prompt. A real, runnable project delivered back to you in under a minute.

---

## Agentic Core

VibeMate runs a full **autonomous agent loop** — not a code generator, not a chatbot wrapper.

### 🔁 The Agent Loop

The agent thinks, acts, observes, and adapts — continuously, until the task is done:

```
Think → Call tool → Read output → Adapt → Think → ...
```

It decides which tools to use, in what order, how many times. You just say what you want.

### 🛠️ Native Agent Tools

**Surgical file editing** — Files are edited using precise unified diffs. Only changed lines are written. No full-file replacements, no data loss, no regressions from unrelated edits.

**Shell execution** — The agent runs real shell commands: `pip install`, `npm ci`, `cargo build`, `pytest`, `make`, `docker`, `git` — anything. It reads the full output and reacts to errors in real time.

**Structured planning** — The agent maintains an internal task plan, updates it as it works, and stays on scope across multi-step jobs.

**Image understanding** — Send a screenshot, UI mockup, or diagram. The agent reads it and incorporates it into the task.

### 🧠 Autonomous Behaviors

- **Self-correcting** — A failed command is an input, not a stop. The agent reads the error and retries with a different approach
- **Multi-step reasoning** — Complex tasks are broken into steps automatically; the agent sequences them without you needing to
- **Context memory** — Project state persists between sessions. The agent knows what it built last time and picks up where it left off
- **Full output visibility** — The agent receives complete command output — full stack traces, install logs, test results — so nothing is hidden from its reasoning
- **Live transparency** — Every action is streamed to Telegram as it happens: what it's doing, which files it's touching, what it's thinking

---

## What You Can Build

**Web & APIs** — React, Next.js, Vue, FastAPI, Express, Django, Flask, REST, GraphQL  
**Backends** — Auth systems, databases, queues, webhooks, cron jobs  
**CLI tools** — Automation scripts, data pipelines, file processors  
**DevOps** — Dockerfiles, CI/CD pipelines, GitHub Actions, nginx configs  
**Tests** — Unit, integration, and e2e tests for any codebase  
**Docs** — README files, API references, changelogs, inline docs  

---

## What You Can Fix

Drop in any broken code — as a ZIP, a file, or a paste. VibeMate will:

- Read the error and trace it to the root cause
- Fix the bug without breaking unrelated code
- Run the tests to confirm the fix works
- Deliver only the changed files back to you

---

## The Interface

VibeMate runs entirely through Telegram. No web dashboard, no browser, no local install.

**Send a ZIP** → Agent works on your full project  
**Send a file** → Agent reads and edits it  
**Send a prompt** → Agent continues working on your existing project  
**Hit Continue** → Agent picks up exactly where it left off  

Every run ends with a ZIP of changed files delivered directly to the chat.

---

## Commands

| Command | What it does |
|---|---|
| `/start` | Register and get your first prompts |
| `/quota` | See how many prompts you have left |
| `/status` | View your current project |
| `/diff` | Show exactly what changed in the last run |
| `/tree` | Browse your project file structure |
| `/projects` | Switch between projects |
| `/reset` | Clear context, start fresh |
| `/delete` | Remove a project permanently |
| `/cancel` | Stop a running job and get your prompt back |
| `/help` | Full reference |

---

## Production Design

VibeMate is built for reliability under real usage, not just demos.

**Concurrency** — Up to 4 agents run simultaneously. Users who submit while slots are full are queued automatically and notified of their position. Jobs time out cleanly after 30 minutes.

**Isolation** — Every user's project lives in a fully isolated directory. No cross-contamination between users, projects, or runs.

**Safety** — Uploaded ZIPs are scanned for path traversal, symlink bombs, and oversized payloads before extraction. Agent output is scrubbed of internal references before delivery.

**Context control** — Project context is byte-capped to prevent bloat from accumulating across long sessions. Prompts are truncated before they can overflow the model window.

**Idle detection** — Agents that go silent for 90 seconds are killed automatically. The prompt is refunded. No hanging jobs, no wasted quota.

**Empty run detection** — If the agent runs but produces zero file changes, no ZIP is delivered. Users get a clear status message instead.

---

## Admin

Built-in admin layer for managing access, quota, and system health.

```
/benchmark   →  Full system health check: API, model, config, agent queue
/admin       →  Live dashboard: users, quota usage, storage, top users
/grant       →  Add prompts to any user
/broadcast   →  Send a message to all registered users
/ban /unban  →  Access control
```

`/benchmark` runs four live checks against the real system — proxy reachability, model response time, config integrity, queue state — and reports results in seconds. Zero prompts consumed.

---

<div align="center">

**VibeMate** — *The coding agent that fits in your pocket.*

**[→ Start for free at @Xanthorox_bot](https://t.me/Xanthorox_bot)**

</div>
