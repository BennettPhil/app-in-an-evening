---
theme: default
title: Don't Be Afraid Of The Terminal
favicon: ''
fonts:
  sans: Inter
  serif: Space Grotesk
  mono: JetBrains Mono
  weights: '400,500,600,700'
  provider: google
class: text-center
highlighter: shiki
transition: slide-left
mdc: false
---

# Build your first App with AI in one evening

Impact Hub Berlin

Wifi: Delta Campus

Password: Campu$2024!?

---
layout: center
class: text-center
---

<div class="wifi-badge" aria-label="Workshop Wi-Fi credentials">
  <span class="wifi-badge__label">Workshop Wi-Fi</span>
  <span><strong>Delta Campus</strong></span>
  <span>Password: <code>Campu$2024!?</code></span>
</div>

# ⚠️ Windows Users ⚠️

### If WSL is not already installed, start it now.

Open PowerShell or Command Prompt and run:

```text
wsl --install
```

Then after reboot

```text
wsl --install Ubuntu
```

---

# How This Will Work

- You'll install and configure an AI coding agent on your laptop.
- You'll build a fully functioning productivity app that you get to take away with you.
- You'll receive the slides and course material, so you do not need to take notes.
- Things will break; raise your hand and someone will come help.
- If you see `green text` in the slides, it is code you can copy.
- Please wait for the group
- Toilets
- Invoice

---

# What You'll Walk Away With

<div class="promise">

<div class="prow">
  <div class="pnum">1</div>
  <div class="ptext">
    <div class="pclaim">Build a <b>real desktop app</b> — a productivity tool you take home with you</div>
    <div class="pquote">It's yours, running on your laptop. No subscription.</div>
  </div>
</div>

<div class="prow">
  <div class="pnum">2</div>
  <div class="ptext">
    <div class="pclaim">Understand <b>how building with AI works</b> — what coding agents do and how to direct them</div>
    <div class="pquote">No need to pay for Lovable or other platforms — go to the source.</div>
  </div>
</div>

<div class="prow">
  <div class="pnum">3</div>
  <div class="ptext">
    <div class="pclaim">Be able to <b>build for yourself</b> — independently, after you leave</div>
    <div class="pquote">Ask AI, not Phil or Igor.</div>
  </div>
</div>

</div>

<style scoped>
.slidev-layout h1 { margin-bottom: 2.4rem; }
.promise {
  display: flex;
  flex-direction: column;
  gap: 1.9rem;
  max-width: 60rem;
}
.prow {
  display: flex;
  align-items: flex-start;
  gap: 1.5rem;
}
.pnum {
  flex: none;
  width: 3.3rem;
  height: 3.3rem;
  border-radius: 50%;
  background: var(--accent);
  color: var(--term-bg);
  font-family: 'JetBrains Mono', monospace;
  font-weight: 700;
  font-size: 1.65rem;
  display: flex;
  align-items: center;
  justify-content: center;
}
.ptext { padding-top: 0.15rem; }
.pclaim {
  font-family: 'Space Grotesk', 'Inter', sans-serif;
  font-size: 1.72rem;
  line-height: 1.22;
  letter-spacing: -0.01em;
  color: var(--ink);
}
.pclaim b { font-weight: 700; }
.pquote {
  margin-top: 0.55rem;
  padding-left: 0.95rem;
  border-left: 3px solid var(--accent);
  font-size: 1.18rem;
  line-height: 1.4;
  font-style: italic;
  color: var(--accent-ink);
}
</style>

---
layout: two-cols
---

# Who Are You And Why Are You Here?

::right::

<img src="/media/why-here.png" class="h-100" />

---

# Agenda

| Duration | |
|---|---|
| ~~5 min~~ | ~~Sit down and get comfortable~~ |
| 15 min | Intro & Context 👈🏾 |
| 70 min | Hands-on & Build |
| 20 min | Advanced Topics |
| 10 min | Wrap Up & Next Steps |
| 60 min | Hangout & Chat |

---
layout: two-cols
hide: true
---

# Everyday AI Club: product designers

## Tuesday, 7 July 2026

### A casual meetup for AI-curious non-technical people. Bring your curiosity, leave with ideas you can use.

[luma.com/everyday-ai-club-designers](https://luma.com/everyday-ai-club-designers)

::right::

<img src="/media/everyday-ai-club.jpg" class="h-100 object-cover bg-white" />

---
layout: center
class: text-center
---

# Intro & Context

---
layout: two-cols
---

# Phil

- Engineering Leadership Consultant & Fractional CTO
- Brit "stuck" in Berlin
- 25+ years in software engineering & leadership
- Author of "Punk Leadership"
- Fixer of unfixable engineering teams

::right::

<img src="/media/phil.jpeg" class="h-100 object-cover" />

---
layout: two-cols
---

# Igor

- Founder of Handpicked Berlin
- Previously in NGOs, corporate, and scale-up environments
- Focused on events, projects, data, and product
- Basic Python knowledge
- The "ideas" guy, enabled by AI

::right::

<img src="/media/igor.jpg" class="h-100" />

---

# What We Built

<div class="grid grid-cols-2 gap-8">
<div>

### Phil

- **Personal Outreach Agent**
- CMS Replacement
- All of Brainfork
- This Presentation
- Agentic Primordial Soup Experiment
- Loads more..

</div>
<div>

### Igor

- Email extractor / newsroom
- Personal task manager
- AI-powered content calendar
- Firefox extension
- **New handpickedberlin.com page**
- Salary Trends reports (v2)
- Luma calendar manager

</div>
</div>

---
layout: center
class: text-center
---

# The Terminal

---

# The Problem

### Computers think like this 👇

```asm
; Register usage
; R1 -- input data pointer
; R2 -- most recent value
;
x3000 LD R1, x006        ; load data pointer
x3001 LDR R2, R1, #0     ; load data value
x3002 BRz x005           ; branch to end if zero
;
; repeating statements go here
;
x3003 ADD R1, R1, #1     ; increment data pointer
x3004 BRnzp x001         ; branch back to top
x3005 HALT
;
; data section
;
x3006 x4000  ; address of data
```

---
layout: two-cols
---

# Humans think like this 👉

::right::

<img src="/media/humans-think.png" class="h-110 object-cover" />

---
layout: image
image: /media/magic-1.png
---

---
layout: image
image: /media/magic-2.png
---

---
layout: image
image: /media/magic-3.png
---

---
layout: center
class: text-center
---

# Then "Magic Happened"

---
layout: image
image: /media/frame1.png
---
layout: two-cols
---

<br/><br/>

> "..the notion that business applications exist, that's probably where they'll all collapse, right in the agent era."
>
> — Satya Nadella, CEO of Microsoft

::right::

<img src="/media/satya.png" class="w-full h-auto object-contain" />

---
layout: center
class: text-center
---

# Agent

### (noun) /ˈeɪdʒ(ə)nt/

A person or thing that takes an active role or produces a specified effect.

---
layout: center
class: text-center
---

# Proven Power of Agentic Coding

---
layout: center
class: text-center
---

### The majority of Claude Code is code now written with Claude Code.

— Boris Cherny, Creator of Claude Code

---
layout: center
class: text-center
---

<img src="/media/chart.webp" class="max-h-110 mx-auto" />

---

# Coding Agents

<div class="grid grid-cols-2 gap-12">
<div>

## Claude Code

- Anthropic, launched in Feb 2025
- CLI and IDE plugin
- Reads your codebase, edits files, runs commands, and works well from the terminal or an IDE.

</div>
<div>

## Codex

- OpenAI, launched in May 2025
- CLI, IDE plugin, and app
- OpenAI's coding agent for reading code, making edits, and running software tasks.

</div>
</div>

### Others worth knowing

<div class="grid grid-cols-2 gap-12">
<div>

- Google Gemini CLI
- Kimi Code CLI
- iFlow CLI
- Pi

</div>
<div>

- Github Copilot CLI
- Kiro CLI
- Aider
- Goose

</div>
</div>

---

# Why Use The Terminal?

- **Works on your real files**, not a sandboxed copy.
- **Does the task end-to-end**, not just describes it.
- **Every step is visible and reversible.**
- **Avoids vendor lock-in** because the work stays in files, commands, and tools you control.

---

# Agenda

| Duration | |
|---|---|
| ~~5 min~~ | ~~Sit down and get comfortable~~ |
| ~~15 min~~ | ~~Intro & Context~~ |
| 70 min | Hands-on & Build 👈🏾 |
| 20 min | Advanced Topics |
| 10 min | Wrap Up & Next Steps |
| 60 min | Hangout & Chat |

---
layout: two-cols
---

# Join the Slack Group

### If you haven't received an invite

### Join here 👉

::right::

<div class="flex flex-col items-center">
<img src="/media/everyday-ai-club-slack-qr.png" class="h-80 bg-white p-5 border-3 border-black" />

[https://is.gd/pGiP5o](https://is.gd/pGiP5o)

</div>

---
layout: two-cols
---

# Hands-on

### Open a Terminal

### Get The Docs 👉

::right::

<div class="flex flex-col items-center">
<img src="/media/qr.png" class="h-80 bg-white p-5 border-3 border-black" />

[https://bit.ly/app-in-day](https://bit.ly/app-in-day)

</div>

---
layout: center
class: text-center
---

# Eisenhower Matrix

<img src="/media/eisenhower-matrix.png" class="max-h-105 object-contain mx-auto mt-6" />

---
layout: two-cols
---

# All applications are *just* folders.

::right::

<img src="/media/folder-of-files.png" class="max-h-110" />

---

# Step 1: Open The Terminal

<div class="grid grid-cols-2 gap-16 pt-8">
<div>

## macOS

1. Press `⌘ + Space` to open Spotlight
2. Type **Terminal**
3. Press `Return`

Or: Applications → Utilities → Terminal

</div>
<div>

## Windows (WSL)

1. Open **Command Prompt** or **PowerShell**
2. Run `wsl`

First-time setup asks for a username & password.

🚨 **When you type a password, nothing shows up.** No dots, no stars. That's normal. Just type it and press Return.

</div>
</div>

<Progress phase="setup" :active="1" />

---

# Before we start: Terminal Basics

### The few commands we'll use today

| Command | What it does | When to use it |
|---|---|---|
| `pwd` | Shows where you are right now | When you feel lost |
| `ls` | Lists the files and folders here | Before moving around |
| `cd workshop` | Moves into the `workshop` folder | To step into your project |
| `cd ..` | Moves back up one folder | To go back |
| `mkdir workshop` | Creates a new folder | To make a place for the project |
| `clear` | Clears the terminal screen | When things feel cluttered |
| `Ctrl + C` | Stops the command currently running | When something seems stuck |

<div style="white-space: nowrap">You do not need to memorise these. The full cheat sheet is on the course website.</div>

<Progress phase="setup" :active="1" />

---

# Step 2: Prepare the Project Tools

<div class="grid grid-cols-2 gap-16 pt-8">
<div>

## 1. Install Homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

*Once the install has completed it will ask you to copy, paste and run some commands. Copy each one separately and run them in the terminal.*

</div>
<div>

## 2. Install Node.js

```bash
brew install node
```

*Node.js includes npm. Our app project needs them; the coding agent itself does not.*

</div>
</div>

<Progress phase="setup" :active="2" />

---

# Step 3: Install an Agent

<p class="pt-8">Install one of these in your terminal. You only need to do this once.</p>

<div class="border-2 border-red-700 bg-red-50 text-red-900 px-5 py-3 mt-4 mb-6 font-bold">
Install only. Do not start the agent yet — we'll do that together in Step 5.
</div>

<div style="display: grid; grid-template-columns: 1fr 2fr; column-gap: 3rem; row-gap: 1.25rem; margin-top: 2rem; align-items: center;">
<div class="text-2xl font-bold">Claude Code</div>
<div><code style="font-size: 18px;">brew install --cask claude-code</code></div>

<div class="text-2xl font-bold">Codex</div>
<div><code style="font-size: 18px;">brew install --cask codex</code></div>

<div class="text-2xl font-bold">Gemini</div>
<div><code style="font-size: 18px;">brew install gemini-cli</code></div>
</div>

<Progress phase="setup" :active="3" />

---

# Step 4: Make A Workshop Folder

<p class="pt-8">A clean place to keep everything we make today. Run these one at a time.</p>


<div class="grid grid-cols-2 gap-16 pt-8">
<div>

### 1. Create the folder

```bash
mkdir workshop
```

*<b>mkdir</b> = "make directory". Nothing will show on screen, that's normal. The folder now exists in your home folder.*

</div>
<div>

### 2. Step into it

```bash
cd workshop
```

*<b>cd</b> = "change directory". Your prompt will now show you're inside `workshop`.*

</div>
</div>

<Progress phase="setup" :active="4" />

---

# Three Views of the Same Thing

### Terminal, Finder and Explorer all walk the same folders.

<img src="/media/three-views.png" class="max-h-90 mx-auto" />

<Progress phase="setup" :active="4" />

---

# Step 5: Start an Agent


<div class="pt-8">

1. Make sure you are in your workshop folder. Your terminal line should mention `workshop`, something like:

```text
jane@laptop:~/workshop$
```

<span class="text-sm opacity-70">The exact look differs per computer.</span>

2. Launch the agent.

<div class="grid grid-cols-3 gap-12 mt-8">
<div>

## Claude Code

`claude`

</div>
<div>

## Codex

`codex`

</div>
<div>

## Gemini

`gemini`

</div>
</div>

</div>

<Progress phase="setup" :active="5" />

---
layout: two-cols
---

# Prompting

### The "Enthusiastic Intern" model

::right::

<img src="/media/intern.png" class="h-100" />

---

# Project Memory
### A note your agent reads every time you start a chat (=session)

<div class="grid grid-cols-2 gap-12 pt-6">
<div>

## `CLAUDE.md`

What Claude Code reads at the top of every session — your project's standing instructions.

</div>
<div>

## `AGENT.md`

The same idea, shared across other tools (Codex, Cursor, etc.) — one file, many agents.

</div>
</div>

- Who you are, how you like to work, what tone to use.
- Project conventions: stack, folder layout, commands to run.
- Things *not* to touch — secrets, generated files, prod data.
- Lives in your project folder and grows as the project does.

---
layout: center
class: text-center
---

# Setup

### We will start by building the structure of our application.

<Progress phase="build" :active="1" />

---

# Step 6: Configuring the Agent

Before we build anything, we'll teach the agent how to talk to us — non-technical, jargon-free, one step at a time. This sets the tone for the whole project.

<div class="border-2 border-black rounded-lg p-8 mt-8 flex gap-12 items-center">
<div class="flex-1">

#### WHAT TO DO

## Grab the *Setup Prompt* from the course website.

Copy it, paste it into your agent, and let it run. We'll walk through what's actually inside it on the next slide.

`bennettphil.github.io/app-in-an-evening/setup-prompt.html`

</div>
<div class="flex flex-col items-center gap-2">
<img src="https://api.qrserver.com/v1/create-qr-code/?size=280x280&margin=0&data=https%3A%2F%2Fbennettphil.github.io%2Fapp-in-an-evening%2Fsetup-prompt.html" class="w-52 border-2 border-black rounded p-2 bg-white" />
<div class="text-xs uppercase tracking-widest opacity-60">Scan to open</div>
</div>
</div>

<Progress phase="build" :active="1" />

---
class: prompt prompt-xl
---

# App Setup Prompt

<div class="grid grid-cols-2 gap-8 text-xs">
<div>

<pre v-pre class="!text-xs !leading-snug overflow-auto max-h-105"># About Me

I have no coding or technical background. This may be the
first time I've ever used a terminal or coding tool. Please
treat me accordingly.

# How to Communicate With Me

- Explain what a command does BEFORE showing it to me
- Translate error messages into plain English — don't
  assume I can read them
- Give me one clear path forward, not options and tradeoffs
- Use numbered steps when asking me to do something
- Check in after each significant step before moving on
- Before any significant action, tell me: what we're doing,
  what will happen, and whether it can be undone

Tone: encouraging, jargon-free, treat all questions as
normal questions.

# My Goal

I want to feel in control of what we're building —
prioritise my confidence and comprehension over speed or
technical elegance.

&#45;&#45;&#45;

# The Task

I want to set up the foundations for a desktop app that
runs on Mac, Windows, and Linux. I'll describe what the app
actually does in a follow-up prompt — for now, just
scaffold the project so we have somewhere to build from.

Pick a sensible default framework for cross-platform
desktop apps. Tell me what it is and why it's a good
default in 2–3 sentences. Don't compare alternatives.

Then:

1. Scaffold the project structure
2. Install all dependencies
3. Launch the app so I see a window open on my machine
4. Create a project instructions file that you (the coding
   agent) will read on every future session in this
   project. Use whatever filename and location is
   conventional for the tool I'm using right now — for
   example `CLAUDE.md`, `AGENTS.md`, `.cursorrules`,
   `CONVENTIONS.md`, or similar. If your tool has a
   built-in command to generate or initialise this file,
   use it. If you're not sure which convention applies,
   default to `AGENTS.md` at the project root and tell me
   that's what you've done.
5. Insert the text between &lt;&lt;&lt;START&gt;&gt;&gt; and &lt;&lt;&lt;END&gt;&gt;&gt; below
   at the very top of that file, verbatim. If a similar
   section already exists, replace it. Leave any other
   existing project-specific content alone.
6. Show me the inserted block, and tell me the filename and
   path you used, so I can confirm the communication style
   is in place.
7. Stop. We'll build the actual features in a later prompt.

**Done means:** the app window opens on my machine, the
project instructions file exists with the block at the top,
and you've shown me both the block and the filename.

**If anything fails** — install errors, missing commands,
the app won't launch — stop and explain in plain English
what went wrong before retrying. Don't paste raw error
output at me.

When everything is running, tell me: what I should see,
where to find it, and what we're building next.

&#45;&#45;&#45;

&lt;&lt;&lt;START&gt;&gt;&gt;

# About Me

I have no coding or technical background. This may be the
first time I've ever used a terminal or coding tool. Please
treat me accordingly.

# How to Communicate With Me

- Explain what a command does BEFORE showing it to me
- Translate error messages into plain English — don't
  assume I can read them
- Give me one clear path forward, not options and tradeoffs
- Use numbered steps when asking me to do something
- Check in after each significant step before moving on
- Before any significant action, tell me: what we're doing,
  what will happen, and whether it can be undone

Tone: encouraging, jargon-free, treat all questions as
normal questions.

# My Goal

I want to feel in control of what we're building —
prioritise my confidence and comprehension over speed or
technical elegance.

&lt;&lt;&lt;END&gt;&gt;&gt;
</pre>

</div>
<div class="pnotes">

<div class="pnote"><span class="pn">1</span>

**Tell it who you are.** Set the communication style up front — non-technical, plain English, encouraging.

</div>

<div class="pnote"><span class="pn">2</span>

**Pick the framework for me.** Don't ask the user to choose a stack — pick a sensible default and explain it briefly.

</div>

<div class="pnote"><span class="pn">3</span>

**What to do, in order.** Numbered steps so the agent works incrementally and you can confirm as it goes.

</div>

<div class="pnote"><span class="pn">4</span>

**Save the rules for next time.** Write the comms preferences to `CLAUDE.md / AGENTS.md` so every future session inherits them.

</div>

<div class="pnote"><span class="pn">5</span>

**Define done & failure.** "Done means…" and "If anything fails…" — give the agent a clear stop condition and a fallback.

</div>

</div>
</div>

---
layout: center
class: text-center
---

# Build

### Now we build

<Progress phase="build" :active="2" />

---

# Step 7: Now We Build the Application

The scaffolding is in place. Now we tell the agent *what* we're actually building — the features, the look, the behaviour.

<div class="border-2 border-black rounded-lg p-8 mt-8 flex gap-12 items-center">
<div class="flex-1">

#### WHAT TO DO

## Grab the *Build Prompt* from the course website.

Paste it into the same session. We'll walk through how it's structured on the next slide.

`bennettphil.github.io/app-in-an-evening/build-prompt.html`

</div>
<div class="flex flex-col items-center gap-2">
<img src="https://api.qrserver.com/v1/create-qr-code/?size=280x280&margin=0&data=https%3A%2F%2Fbennettphil.github.io%2Fapp-in-an-evening%2Fbuild-prompt.html" class="w-52 border-2 border-black rounded p-2 bg-white" />
<div class="text-xs uppercase tracking-widest opacity-60">Scan to open</div>
</div>
</div>

<Progress phase="build" :active="2" />

---
class: prompt prompt-md
---

# Build Prompt

<div class="grid grid-cols-2 gap-8 text-xs">
<div>

```md
# Mode: Build

Keep using the communication style from the project
instructions file. I'm still non-technical.

# What I want

A desktop app that helps me prioritise tasks using the
Eisenhower matrix.

# How it works

1. **Add tasks.** I type a short to-do list.
2. **Prioritise.** I drag each task onto one of four
   quadrants of an Eisenhower matrix : Urgent + Important,
   Important / Not Urgent, Urgent / Not Important, Neither.
3. **Plan.** I click "Plan" and see my tasks grouped: Do
   first, Schedule, Delegate, Drop.
4. **Execute.** Each task has a state: todo, in progress,
   paused, done. I can change states. From here, I can add
   more tasks or re-prioritise.

# Acceptance criteria

- Tasks (and their states and quadrants) survive closing
  and reopening the app.
- Menu bar/system tray icon to open the app. Closing the
  window doesn't quit it.
- The matrix shouldn't get cluttered if I add lots of tasks.
- Drag-and-drop works on Mac, Windows, and Linux.
- The labels should be shown on the axis of the matrix
- The plan should be presented as a list showing the
  highest priority tasks at the top.

# Build it in steps

Build one piece at a time. After each piece, tell me what
to click to test it, and wait for me to confirm before
moving on. Suggested order: add tasks → prioritise → plan →
states → menu bar.

For small choices I haven't mentioned (colours, layout
details), pick something sensible and tell me what you
picked in one line. Don't ask me to choose.
```

</div>
<div class="pnotes">

<div class="pnote"><span class="pn">1</span>

**Set the mode.** "Mode: Build" tells the agent which job it's doing — and to keep using your saved communication style.

</div>

<div class="pnote"><span class="pn">2</span>

**One-line goal.** Say what you want in a single sentence. The whole prompt hangs off this.

</div>

<div class="pnote"><span class="pn">3</span>

**How a user uses it.** Walk through the user flow as numbered steps — concrete, in order, with the words you'd say out loud.

</div>

<div class="pnote"><span class="pn">4</span>

**Definition of done.** Acceptance criteria: the things that *must* be true before you'd call it shipped.

</div>

<div class="pnote"><span class="pn">5</span>

**Build in steps, not in one shot.** Tell it to deliver in pieces and pause for confirmation — small choices, it makes for you.

</div>

</div>
</div>

---

# What if something doesn't work?

Something *will* break — no software is perfect. The trick is telling the agent what you saw, what you expected, and letting it translate the error back into plain English.

<div class="border-2 border-black rounded-lg p-8 mt-8 flex gap-12 items-center">
<div class="flex-1">

#### WHAT TO DO

## Grab the *Debug Prompt* from the course website.

Fill in what you expected, what you saw, and what you'd already tried. Paste it in. We'll walk through the structure next.

`bennettphil.github.io/app-in-an-evening/debug-prompt.html`

</div>
<div class="flex flex-col items-center gap-2">
<img src="https://api.qrserver.com/v1/create-qr-code/?size=280x280&margin=0&data=https%3A%2F%2Fbennettphil.github.io%2Fapp-in-an-evening%2Fdebug-prompt.html" class="w-52 border-2 border-black rounded p-2 bg-white" />
<div class="text-xs uppercase tracking-widest opacity-60">Scan to open</div>
</div>
</div>

<Progress phase="build" :active="3" />

---
class: prompt prompt-lg
---

# Debug Prompt

<div class="grid grid-cols-2 gap-8 text-xs">
<div>

```md
# Mode: Debug

Keep using the communication style from the project
instructions file. I'm still non-technical. Don't paste raw
error output at me — translate it.

# Expected behaviour

What I expected the app to do, and what I was doing when
the problem happened.

- I clicked "Plan" after dragging three tasks into the
  Urgent + Important quadrant.
- I expected to see those three tasks at the top of the
  "Do first" list.

# Current behaviour

What's actually happening instead.

- The Plan screen opens but it's empty.
- The tasks are still there on the matrix when I go back —
  they didn't get deleted.
- It happens every time, not just once.

# Context

- Relevant files/paths: see `src/plan/` and wherever the
  matrix state lives.
- Any error message I can see (in the app, in a popup, or
  in the dev console if you tell me how to open it).
- Any log files you know about — tell me where to look and
  I'll paste what's there.
- This started after we added the "Schedule / Delegate /
  Drop" grouping.

# What I've already tried

- Quit the app and reopened it — same result.
- Added a fresh task and dragged it in — still empty Plan
  screen.
- I have NOT touched any code or settings myself.

# How I want you to work

1. Form a hypothesis in plain English before changing
   anything.
2. Tell me the smallest test we can run to confirm it — one
   step at a time.
3. Only change code once we agree on the cause.
4. After the fix, tell me what you changed and why, in one
   paragraph.

# Acceptance criteria

- Clicking "Plan" shows my prioritised tasks, highest
  priority first.
- Existing tasks and quadrants are not lost.
- Closing and reopening the app still works.

# Notes

If you discover the real bug is somewhere else, stop and
tell me before fixing it — don't quietly expand the scope.
```

</div>
<div class="pnotes">

<div class="pnote"><span class="pn">1</span>

**Switch the mode.** "Mode: Debug" — same comms style, different job. No raw error dumps.

</div>

<div class="pnote"><span class="pn">2</span>

**Expected vs. actual.** Two short stories: what you thought would happen, and what's happening instead. Concrete actions, not vibes.

</div>

<div class="pnote"><span class="pn">3</span>

**Where to look & what changed.** Point at files, errors, logs — and mention what changed just before things broke.

</div>

<div class="pnote"><span class="pn">4</span>

**Hypothesis before fix.** Make the agent reason out loud and propose the smallest test before touching code.

</div>

<div class="pnote"><span class="pn">5</span>

**Don't expand the scope.** If the real bug is somewhere else, stop and tell you — don't quietly fix five things at once.

</div>

</div>
</div>

---

# Agenda

| Duration | |
|---|---|
| ~~5 min~~ | ~~Sit down and get comfortable~~ |
| ~~15 min~~ | ~~Intro & Context~~ |
| ~~70 min~~ | ~~Hands-on & Build~~ |
| 20 min | Advanced Topics 👈🏾 |
| 10 min | Wrap Up & Next Steps |
| 60 min | Hangout & Chat |

---
layout: two-cols
---

# Advanced Topics

## <span class="topic-line">Model Choice</span>

## <span class="topic-line">Sub-agents</span>

## <span class="topic-line">Skills</span>

::right::

<img src="/media/advanced.png" class="h-100" />


---

# FYI: Models and "Thinking Level"

### More "Power" = More Cost

<div class="grid grid-cols-2 gap-12">
<div>

## Claude

`/model`

- **Opus:** more powerful, use for more complicated tasks
- **Sonnet:** cheaper, use for simpler everyday tasks

<hr class="my-3"/>

`/effort auto`

Good default — you can change it anytime.

</div>
<div>

## Codex

`/model`

- Strongest / default coding model: use for harder tasks
- Mini / smaller model: cheaper, use for simpler everyday tasks

<hr class="my-3"/>

"Medium" is a good default — turn it up only if a task is genuinely hard.

</div>
</div>


---
layout: two-cols
---

<img src="/media/subagent.png" class="h-100" />

::right::

# Sub-agents

## Add *me* to your project!

---

# Sub-agents

<div class="grid grid-cols-2 gap-12">
<div>

## Claude

### Easy

`/agents`

Paste in the sub-agent prompt

</div>
<div>

## Codex

### Less Easy

Follow the guide on the course site.

</div>
</div>

---
layout: two-cols
---

# Skills

## Add *anyone* to your project

::right::

<img src="/media/skills.png" class="h-100" />

---
layout: center
class: text-center
---

# Skills

## Via skills.sh

Add a frontend design skill to your project:

`npx skills add https://github.com/anthropics/skills --skill frontend-design`

---

# Agenda

| Duration | |
|---|---|
| ~~5 min~~ | ~~Sit down and get comfortable~~ |
| ~~15 min~~ | ~~Intro & Context~~ |
| ~~70 min~~ | ~~Hands-on & Build~~ |
| ~~20 min~~ | ~~Advanced Topics~~ |
| 10 min | Wrap Up & Next Steps 👈🏾 |
| 60 min | Hangout & Chat |

---
layout: two-cols
---

# Homework

> "Move Fast, Break Things"
>
> Work on your project for a few hours and see what you can achieve.

::right::

<img src="/media/homework.png" class="h-100" />

---

# Follow Up Session

<div class="grid grid-cols-2 gap-16 mt-8">
<div>

#### WHAT WE'LL COVER

- "Open Office": review issues and provide hands-on support
- Show & Tell: show us what you made
- What next: distribution, what agents aren't good at

</div>
<div>

#### WHEN

<div class="border-2 border-black rounded-lg p-6">

### Thursday, 6 August

18:00 – 20:00

</div>

</div>
</div>

---
layout: two-cols
---

#### YOUR SUPPORT CONTINUES AFTER TONIGHT

# Keep Building in Slack

## Your private workshop channel

- Ask follow-up questions when you get stuck
- Share your builds and get feedback
- Keep learning with this workshop group

::right::

## The wider Everyday AI community

- **Show-and-tell** — share projects and ask for feedback
- **Ask-anything** — bring questions beyond the workshop
- **Meetups & announcements** — stay connected to what's next

<div class="mt-8 border-t-2 border-black pt-4 text-xl font-bold">
You're already invited — look for your private workshop channel in Slack.
</div>

---
layout: center
class: text-center
---

# Igor, Selfie!

---
layout: center
class: text-center
---

## Good Luck

---
layout: two-cols
---

#### SESSION TWO

# Build Your First App With AI In One Evening

Online

::right::

<img src="/media/monster-1.png" class="h-110 object-contain" />

---

#### SESSION TWO

# Agenda

| Duration | |
|---|---|
| 30 min | Advanced Topics & Distribution |
| 30 min | Show and Tell |
| 55 min | Questions |
| 5 min | Wrap Up |

---
class: dense
---

#### WHICH ONE SHOULD I USE?

# AI Coding Surfaces

<div class="text-xs">

| | **TERMINAL**<br/>Claude Code, Codex CLI | **CODE EDITOR**<br/>VS Code, Cursor | **BROWSER**<br/>Claude web, ChatGPT web, Codex web | **DESKTOP APP**<br/>Claude Desktop, ChatGPT app, Codex app |
|---|---|---|---|---|
| **Best for** | Quick build-test-fix work, scripts, repeat jobs | Everyday coding with help inside the editor | Research, planning, questions, longer tasks | Cross-app help, less tab switching |
| **Biggest plus** | Closest to your real project and tools | Best mix of speed and easy review | Good for bigger tasks you can hand off | Can work with local apps and files |
| **Watch out for** | Harder to learn, less visual | Depends on your editor and plugins | May be less connected to live local files | What it can do varies by product |
| **What it can see** | Project files, commands, scripts | Open files, your project, selected code | Chats, uploaded files, saved project info, connected tools | Local files, apps, and chat history |
| **How you review** | Read the output, tests, and file changes | See changes in the editor and accept or reject them | Review summaries, results, and produced files | Review the chat and any actions it takes |
| **Use this when…** | You want the fastest path from idea to working code | You want AI inside your normal coding flow | You want help thinking, exploring, or delegating | You want a general assistant with local awareness |

</div>

<div class="mt-4 p-3 border border-gray-500 text-center font-medium text-sm">Different workspaces for different jobs — not one winner.</div>

---
layout: two-cols
---

#### REALITY CHECK

# What LLMs Can't Do Well

### Powerful. Also confidently wrong, often.

::right::

<img src="/media/monster-4.png" class="h-110 object-cover" />

---

#### REALITY CHECK

# What LLMs Can't Do Well

<div class="grid grid-cols-2 gap-x-16 gap-y-6 mt-8 text-2xl">

<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">01</span>It doesn't know when it's wrong</div>
<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">02</span>It doesn't read your codebase the way you do</div>
<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">03</span>More context isn't better context</div>
<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">04</span>If it has to be right, verify it</div>
<div class="border-t-2 border-black pt-4 col-span-2"><span class="text-red-700 text-4xl mr-4">05</span>The model is a mirror for your prompt</div>

</div>

---

#### ALSO GOOD TO KNOW

# More Things It Gets Wrong

<div class="grid grid-cols-2 gap-x-16 gap-y-6 mt-8 text-2xl">

<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">06</span>It can't do math reliably</div>
<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">07</span>It is extremely suggestible</div>
<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">08</span>Same prompt, different answer</div>
<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">09</span>The model behind the name keeps changing</div>
<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">10</span>It won't write like you</div>
<div class="border-t-2 border-black pt-4"><span class="text-red-700 text-4xl mr-4">11</span>The "pink elephant" effect — don't tell it what <em>not</em> to do</div>

</div>

---
layout: two-cols
---

#### SHIP IT

# Distribution

### How do I get my thing into people's hands?

::right::

<img src="/media/monster-distribution.png" class="h-110 object-contain" />

---
class: dense
---

#### SHIP IT

# Next Steps by Target

<div class="text-sm">

| Target | Where It Lives | Cost / Gotchas | Source Control |
|---|---|---|---|
| **Web App** | Vercel, Netlify, Cloudflare Pages — free tiers | Domain ~€10/yr. Add analytics early. | Connect GitHub — every push auto-deploys. Use branches for previews. |
| **Browser Ext.** | Chrome Web Store, Firefox Add-ons | Chrome: $5 dev fee, ~1 week review. Firefox: free, faster. | GitHub + tagged releases. Zip the build from a clean checkout. |
| **Desktop App** | Electron or Tauri. Installers on GitHub Releases. | macOS signing: $99/yr Apple Developer. Auto-update via electron/tauri-updater. | GitHub Releases as your distribution channel. Tag = version. |
| **Mobile App** | TestFlight (iOS) / Play Internal Testing | Store listing = its own project. Hardest path — be sure you need native. | GitHub + Fastlane or EAS to automate builds per branch. |

</div>

<div class="text-sm mt-4 opacity-80"><b>First, a word on Git.</b> Git is a "save button" for your whole project — every change is a snapshot you can roll back to. Start with `git init`, push to a private GitHub repo, and let the agent commit as you work. → <b>Idiots Guide to Git</b> on the docs site.</div>

---
layout: two-cols
---

#### YOUR TURN

# Show & Tell

### 3 minutes. What did you build?

::right::

<img src="/media/monster-showtell.png" class="h-110 object-contain" />

---
layout: center
class: text-center
---

# Questions?

### Anything stuck? Anything weird? Anything amazing?

---

#### STAY IN TOUCH

# Follow Us on LinkedIn

<div class="grid grid-cols-2 gap-16 mt-8">
<div class="flex flex-col items-start">

## Phil

<img src="/media/qr-phil.png" class="w-72 h-72 object-contain" />

</div>
<div class="flex flex-col items-start">

## Igor

<img src="/media/qr-igor.png" class="w-72 h-72 object-contain" />

</div>
</div>

---
layout: two-cols
---

#### THAT'S A WRAP

# Thanks.

### Now tell us how we did — 2 minutes, honest.

`tally.so/r/BzLabK`

::right::

<img src="/media/feedback-qr.png" class="w-80 mx-auto" />
