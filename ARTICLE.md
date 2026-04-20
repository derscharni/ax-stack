# The AX Stack: A Design Framework for the Age of Agents

**Status:** final v2 | 2026-04-20

---

Every major technological shift brings with it a new design problem.

The web gave us information architecture. Mobile enabled touch interaction. Agents give us something more difficult: systems that act on behalf of humans, building or destroying trust, often without the human knowing what's happening.

Building trust is the defining design challenge of the AI age. And it cannot be approached directly. It emerges from five layers that can be designed.

This is the AX Stack.

---

## Why a stack?

In engineering, a stack is a set of layers where each depends on the one below. You can't run an application without an operating system. You can't have a network without a transport protocol.

The AX Stack works the same way. Each layer is a prerequisite for the next. And wrapping all of it: Relationship. Not as a layer you design, but as the outcome that emerges when all five layers work, or breaks when any one of them fails.

---

## Layer 1: Intent

What the human actually wants, and whether that matches what they expressed.

Intent is not input parsing. It is the validation process that happens before any agent acts: context recognition, world alignment, ambiguity resolution. And two questions most frameworks skip entirely.

Delegation detection: is this intent coming from a human or from another agent? That changes how it must be validated.

Intent drift: if a task runs for 20 minutes, is the original intent still valid?

---

## Layer 2: Authority

Who has the right to act, in whose name, under what conditions.

91% of organizations now use agents. 10% have a governance strategy (Fortune/JumpCloud, 2026). The gap is the Authority layer missing in production.

Not just "who can act" but which capabilities they can use. Not just authorization but revocation, how is authority taken back when context or trust changes?

A2A, the open agent-to-agent protocol now live in Copilot Studio, has no authority layer for cross-agent delegation. When Agent A delegates to Agent B, whose authority applies? The spec doesn't say.

---

## Layer 3: Context ★

Who the human is, what their perspective is, and who has the right to challenge it.

Context carries the ★ because it is the most contested layer. Every platform, every vendor, every protocol is trying to control this.

The elements most frameworks include: identity, perspective, recency. The element most frameworks miss: critique license. The agent is permitted, and expected, to challenge context when it is outdated, contradictory, or one-sided. Context that cannot be questioned is a filter bubble.

And the question that defines the next decade: who controls the canonical version of your context? That is Context Sovereignty.

---

## Layer 4: Orchestration

What gets automated, what requires human input, and how visible is all of it.

Most teams treat orchestration as a technical decision. It is not. The choice between hub-and-spoke and swarm determines where accountability lands. That is a design decision with governance consequences.

This is also where UX heuristics apply directly. Nielsen's 10 heuristics are not soft principles here, they are hard requirements. Visibility of system status. User control and freedom. Error prevention. The human needs to oversee a system acting faster than they can observe.

Zero friction vs. control: how do we achieve human-in-the-loop without it feeling like forms?

---

## Layer 5: Accountability

Who decided what, when, on what basis, and what happens when it was wrong.

Technically the most tractable layer. Designerically the most underestimated.

GitHub builds the flight recorder, not the instrument panel. Accountability is only valuable when it surfaces at the right time for the right person. Agents act in milliseconds. Accountability runs at human speed. The gap between them is the actual design problem.

And the unsolved question: when Agent A, acting for Human A, causes a failure at Human B's agent, who is accountable? No current protocol answers this.

---

## Relationship: The Outcome, Not the Layer

Relationship is not the sixth layer. It is what emerges when all five layers function consistently over time.

Trust is not designed. But if you design these layers, trust will emerge.

---

## The unsolved frontier

Everything above describes one human, one agent, one interaction context.

The harder problem: two humans, each with their own AX Stack, interacting through their respective agents.

A2A provides the pipe. It deliberately does not provide what sits above the pipe, the spec says so explicitly: agents collaborate "without needing access to each other's internal state, memory, or tools."

What sits above the pipe is Intention Disclosure: when an agent pushes something to another agent, it declares what it is, why now, and what response is expected. The receiving agent filters against the recipient's preferences, not the sender's optimization criteria.

What an agent pushes is never just data. It is always a crystallized, opinionated interpretation of something. Which means the receiving human does not just need the content. They need to know whose interpretation just arrived, and whether they actually need it in that moment.

That is the design problem the next generation of collaboration tools needs to solve. The infrastructure is almost there. The human-facing layer is not.

---

*The AX Stack is a living framework. Challenges and contributions welcome.*
*Context Sovereignty, Temporal UX, Killerjourney, and Intention Disclosure are developed further in related work.*
