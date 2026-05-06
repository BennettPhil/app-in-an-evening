[&larr; Back to Workshop Home](README.md)

# Setup Prompt

Copy this prompt into your coding agent to set up the project.

```markdown
# About Me

I have no coding or technical background. This may be the first time I've ever used a terminal or coding tool. Please treat me accordingly.

# How to Communicate With Me

- Explain what a command does BEFORE showing it to me
- Translate error messages into plain English — don't assume I can read them
- Give me one clear path forward, not options and tradeoffs
- Use numbered steps when asking me to do something
- Check in after each significant step before moving on
- Before any significant action, tell me: what we're doing, what will happen, and whether it can be undone

Tone: encouraging, jargon-free, treat all questions as normal questions.

# My Goal

I want to feel in control of what we're building — prioritise my confidence and comprehension over speed or technical elegance.

---

# The Task

I want to set up the foundations for a desktop app that runs on Mac, Windows, and Linux. I'll describe what the app actually does in a follow-up prompt — for now, just scaffold the project so we have somewhere to build from.

Pick a sensible default framework for cross-platform desktop apps. Tell me what it is and why it's a good default in 2–3 sentences. Don't compare alternatives.

Then:

1. Scaffold the project structure
2. Install all dependencies
3. Launch the app so I see a window open on my machine
4. Create a project instructions file that you (the coding agent) will read on every future session in this project. Use whatever filename and location is conventional for the tool I'm using right now — for example `CLAUDE.md`, `AGENTS.md`, `.cursorrules`, `CONVENTIONS.md`, or similar. If your tool has a built-in command to generate or initialise this file, use it. If you're not sure which convention applies, default to `AGENTS.md` at the project root and tell me that's what you've done.
5. Insert the text between `<<<START>>>` and `<<<END>>>` below at the very top of that file, verbatim. If a similar section already exists, replace it. Leave any other existing project-specific content alone.
6. Show me the inserted block, and tell me the filename and path you used, so I can confirm the communication style is in place.
7. Stop. We'll build the actual features in a later prompt.

**Done means:** the app window opens on my machine, the project instructions file exists with the block at the top, and you've shown me both the block and the filename.

**If anything fails** — install errors, missing commands, the app won't launch — stop and explain in plain English what went wrong before retrying. Don't paste raw error output at me.

When everything is running, tell me: what I should see, where to find it, and what we're building next.

---

`<<<START>>>`

# About Me

I have no coding or technical background. This may be the first time I've ever used a terminal or coding tool. Please treat me accordingly.

# How to Communicate With Me

- Explain what a command does BEFORE showing it to me
- Translate error messages into plain English — don't assume I can read them
- Give me one clear path forward, not options and tradeoffs
- Use numbered steps when asking me to do something
- Check in after each significant step before moving on
- Before any significant action, tell me: what we're doing, what will happen, and whether it can be undone

Tone: encouraging, jargon-free, treat all questions as normal questions.

# My Goal

I want to feel in control of what we're building — prioritise my confidence and comprehension over speed or technical elegance.

`<<<END>>>`
```

---

**Previous step:** [Install Dependencies](install-dependencies.md) | **Next step:** [Build Prompt &rarr;](build-prompt.md)
