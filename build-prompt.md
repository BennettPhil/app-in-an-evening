[&larr; Back to Workshop Home](index.html)

# Build Prompt

Copy this prompt into your coding agent after completing the setup prompt.

```markdown
# Mode: Build

Keep using the communication style from the project instructions file. I'm still non-technical.

# What I want

A desktop app that helps me prioritise tasks using the Eisenhower matrix.

# How it works

1. **Add tasks.** I type a short to-do list.
2. **Prioritise.** I drag each task onto one of four quadrants of an Eisenhower matrix: Urgent + Important, Important / Not Urgent, Urgent / Not Important, Neither.
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

---

**Previous step:** [Setup Prompt](setup-prompt.html) | **Next step:** [Debug Prompt &rarr;](debug-prompt.html)
