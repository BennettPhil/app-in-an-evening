# Claude Build Prompt

```
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


# Build Prompt

```
# Mode: Build

Keep using the communication style from the project instructions file. I'm still non-technical.

# What I want

A desktop app that helps me prioritise tasks using the Eisenhower matrix.

# How it works

1. **Add tasks.** I type a short to-do list.
2. **Prioritise.** I drag each task onto one of four quadrants of an Eisenhower matrix : Urgent + Important, Important / Not Urgent, Urgent / Not Important, Neither.  
3. **Plan.** I click "Plan" and see my tasks grouped: Do first, Schedule, Delegate, Drop.
4. **Execute.** Each task has a state: todo, in progress, paused, done. I can change states. From here, I can add more tasks or re-prioritise.

# Acceptance criteria

- Tasks (and their states and quadrants) survive closing and reopening the app.
- Menu bar/system tray icon to open the app. Closing the window doesn't quit it.
- The matrix shouldn't get cluttered if I add lots of tasks.
- Drag-and-drop works on Mac, Windows, and Linux.
- The labels should be shown on the axis of the matrix 
- The plan should be presented as a list showing the highest priority tasks at the top. 

# Build it in steps

Build one piece at a time. After each piece, tell me what to click to test it, and wait for me to confirm before moving on. Suggested order: add tasks → prioritise → plan → states → menu bar.

For small choices I haven't mentioned (colours, layout details), pick something sensible and tell me what you picked in one line. Don't ask me to choose.
```