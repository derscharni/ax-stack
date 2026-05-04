# Layer 3: Context ★

**Definition:** Who the human is, what their perspective is, and who has the right to challenge it.

★ = the most contested layer. Every platform is trying to control this.

## Elements

| Element | Description |
|---|---|
| Identity | Values, frameworks, priorities, working style |
| Perspective | The angle from which the agent reasons |
| Recency | Is this context still valid? |
| Provenance | Where did this context come from, when? |
| Critique license | Agent is expected to challenge stale or biased context |
| Sovereignty | Who controls the canonical version? |
| Shared context | Whose version is canonical when two humans share context? |
| Context decay | Context goes stale without being declared stale |

## The defining question

**Who controls the canonical version of your context?**

That is **Context Sovereignty.** It is the design problem of the next decade — and it is largely uncontested in current product architecture.

Most frameworks treat context as a memory bag. The AX Stack treats it as a layered, time-stamped, provenance-tagged, critique-licensed object.

## Common gaps

- **Context as memory dump.** No structure, no recency, no critique license. Agents echo what's there.
- **Filter-bubble agents.** Agents trained to align without permission to challenge produce stale, one-sided reasoning.
- **No sovereignty model.** Vendor's vault becomes the canonical version by default. The user does not own a portable, signed, structured context.
- **No fidelity model in multi-agent flows.** Context is reconstructed at runtime — sovereignty is a fidelity problem, not only a storage problem.

## Design checklist

- [ ] Is context typed (identity vs. perspective vs. recency)?
- [ ] Does the agent have explicit critique license — and does it use it?
- [ ] Is context portable across vendors, or vendor-locked?
- [ ] When context decays, what surfaces it?
- [ ] In multi-agent flows, what guarantees fidelity end-to-end?

## Connects to

- **`concepts/inter-stack-protocol.md`** — when two stacks meet, whose context is canonical?
- **`concepts/collective-forgetting.md`** — at scale, shared context produces semantic monoculture. Forgetting is a feature.
- **`references/related-work.md`** → Context Sovereignty, Temporal UX.
