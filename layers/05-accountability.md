# Layer 5: Accountability

**Definition:** Who decided what, when, on what basis — and what happens when it was wrong.

Technically the most tractable layer. Designerically the most underestimated.

## Elements

| Element | Description |
|---|---|
| Logging | Decision trail: who, what, when, on what basis |
| Attribution | Agent, model, human, or delegation chain? |
| Explainability | Why — readable by the human, not just as a log |
| Error recovery | Reversal path, notification, remediation |
| Audit vs. transparency | Right information, right person, right time |
| Temporal gap | Agents act in ms; accountability runs at human speed |
| Inter-stack | Who is accountable when Agent A fails at Human B's stack? |

## The actual design problem

Agents act in milliseconds. Accountability runs at human speed. The gap is the work.

GitHub builds the flight recorder, not the instrument panel. Logs are the bare minimum. Accountability is only valuable when it surfaces at the right time for the right person.

## Two unsolved questions

1. **Cross-stack accountability.** When Agent A, acting for Human A, causes a failure at Human B's stack, who is accountable? No protocol answers this today.
2. **Design-time vs. legal-time accountability.** EU AI Act treats accountability as audit trail. Saarinen/Linear treat it as a pre-action design constraint. Both are real; they are not the same thing. Design for both.

## Common gaps

- **Logs without explanation.** A trail that no human can read in time is not accountability — it's evidence after the fact.
- **No reversal path.** Detecting a wrong decision is not enough; the system must support undoing it.
- **Audit-as-accountability conflation.** Audit serves regulators. Accountability serves the user in the moment something goes wrong.

## Design checklist

- [ ] Can the user see, in plain language, why the agent did what it did — at the moment of action, not in a log?
- [ ] Is there a reversal path for every consequential action?
- [ ] Where is the temporal gap (agent speed vs. human speed) bridged in the UX?
- [ ] How does accountability propagate across stacks?

## Connects to

- **Authority** — accountability presupposes bounded authority.
- **Orchestration** — architecture choice (hub vs. swarm) is also an accountability choice.
- **Inter-Stack Protocol** — multi-stack accountability is open research.
