[&larr; Back to Workshop Home](index.html)

# Debug Prompt

Use this template when something is broken and you want your coding agent to investigate it. Copy the template, fill in the details from your situation, and paste it into your coding agent.

```markdown
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

---

## Optional Next Step

Want to add a reviewer after the bug is fixed? Pick the guide for your agent:

- [Claude Code Sub-Agent](claude-sub-agent.html)
- [Codex Sub-Agent](codex-sub-agent.html)

---

**Previous step:** [Build Prompt](build-prompt.html) | **Next step:** [Workshop Home &rarr;](index.html)
