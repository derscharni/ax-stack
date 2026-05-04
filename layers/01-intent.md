# Layer 1: Intent

**Definition:** What the human actually wants — and whether that matches what they expressed.

Intent is not input parsing. It is the validation process that happens before any agent acts.

## Elements

| Element | Description |
|---|---|
| Context recognition | Situation awareness: time, environment, state |
| Intent validation | Does expressed request match actual need? |
| World alignment | Relevant external information (company, events, changes) |
| Ambiguity resolution | What needs clarification before acting? |
| Delegation detection | Is intent from a human or another agent? |
| Intent drift | Is the original intent still valid mid-task? |

## Common gaps

- **Treating input as intent.** A prompt is a request, not necessarily a need. The Intent layer is the difference.
- **No delegation source check.** When Agent A asks Agent B for something, B treats it like a human request. The validation should be different.
- **Ignoring intent drift.** Long-running tasks (research, refactor, batch operations) need a re-validation point. Original intent may be obsolete.

## Design checklist

- [ ] Where does the agent confirm understanding before acting?
- [ ] How are ambiguous requests surfaced (not silently guessed)?
- [ ] When does the agent re-check intent during long-running work?
- [ ] Is the request source (human vs. agent) part of the validation logic?

## Connects to

- **Authority** — intent without authority bounds is unsafe.
- **Context** — intent is interpreted through context.
- **Inter-Stack Protocol** — when intent crosses stack boundaries, declaration is required (see `concepts/intention-disclosure.md`).
