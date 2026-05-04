# Layer 4: Orchestration

**Definition:** What gets automated, what requires human input, and how visible is all of it.

## Elements

| Element | Description |
|---|---|
| Automation scope | What is autonomous vs. requires approval vs. never delegated |
| Agent-to-agent handoffs | What can agents pass without involving the human? |
| Human-in-the-loop | Practical oversight, not theoretical |
| Zero friction vs. control | HITL without forms: notifications, progressive disclosure |
| UX heuristics | Nielsen's 10 heuristics apply directly |
| Temporal UX | When must the human know something changed mid-task? |

## Architecture is a governance choice

The choice between hub-and-spoke and swarm is not a technical decision. It determines where accountability lands.

- **Hub-and-spoke:** clear accountability, central coordination, scalability ceiling.
- **Swarm:** scales horizontally, but accountability becomes a distributed failure mode.

This choice belongs in product strategy, not just engineering.

## Common gaps

- **Forms-as-HITL.** Approval modals interrupt without informing. Progressive disclosure is the design pattern; modal blocking is the anti-pattern.
- **Invisible handoffs.** Agent A passes to Agent B without the human knowing the conversation now has a new participant.
- **Temporal blindness.** A 20-minute task changes the world; the human is not re-engaged at the moments of change.

## Design checklist

- [ ] What is autonomous, what is approved, what is never delegated — written down?
- [ ] Are agent-to-agent handoffs visible to the human in real time?
- [ ] Does the orchestration surface state at the right moments, not constantly?
- [ ] Which Nielsen heuristic is being violated when oversight feels heavy?

## Connects to

- **Accountability** — orchestration architecture determines accountability surface.
- **Intent** — orchestration without intent re-validation drifts.
- **Inter-Stack Protocol** — multi-stack orchestration is the unsolved frontier.
