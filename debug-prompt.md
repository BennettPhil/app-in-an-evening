[&larr; Back to Workshop Home](README.md)

# Debug Prompt

Use this template when something is broken and you want your coding agent to investigate it. Copy the template, fill in the parts in square brackets `[like this]`, and paste it into your coding agent.

```markdown
## Mode
Debug

## Expected Behaviour
A few short sentences about what you expected the software to do.
Include what you were doing when the problem happened.

## Current Behaviour
A few short sentences about what is happening instead.

## Context
- Relevant files/paths: [list them or say "see src/auth/"]
- Any error messages that you see when the problem occurs
- Any log files that exist and can be checked
- Related issue/ticket: [link or description]

## What I've Already Tried
A list of everything you've tried

## Acceptance Criteria
- [ ] [Specific, testable outcome]
- [ ] [Another outcome]

## Notes
[Any edge cases, preferences, or things to watch out for]
```

---

## Optional Next Step

Want to add a reviewer after the bug is fixed? Pick the guide for your agent:

- [Claude Code Sub-Agent](claude-sub-agent.md)
- [Codex Sub-Agent](codex-sub-agent.md)

---

**Previous step:** [Build Prompt](build-prompt.md) | **Next step:** [Workshop Home &rarr;](README.md)
