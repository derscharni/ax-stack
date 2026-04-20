# AX Stack

A design framework for human-agent interaction. Five operational layers. One emergent outcome.

**Version:** April 2026
**Author:** Jens Scharnetzki

---

## Overview

```
┌─────────────────────────────────────────┐
│              RELATIONSHIP               │
│         (Trust or Distrust)             │
│   emerges from all five layers working  │
│                                         │
│  ┌───────────────────────────────────┐  │
│  │         Accountability            │  │
│  ├───────────────────────────────────┤  │
│  │          Orchestration            │  │
│  ├───────────────────────────────────┤  │
│  │           Context ★               │  │
│  ├───────────────────────────────────┤  │
│  │           Authority               │  │
│  ├───────────────────────────────────┤  │
│  │            Intent                 │  │
│  └───────────────────────────────────┘  │
│                                         │
│  A2A / A2H interaction → Trust/Distrust │
└─────────────────────────────────────────┘
```

Each layer is a prerequisite for the one above it. Relationship is not a layer — it is the outcome that emerges when all five work, or breaks when any one fails.

---

## Layer 1: Intent

What the human actually wants — and whether that matches what they expressed.

| Element | Description |
|---|---|
| Context recognition | Situation awareness: time, environment, state |
| Intent validation | Does expressed request match actual need? |
| World alignment | Relevant external information (company, events, changes) |
| Ambiguity resolution | What needs clarification before acting? |
| Delegation detection | Is intent from a human or another agent? |
| Intent drift | Is the original intent still valid mid-task? |

---

## Layer 2: Authority

Who has the right to act, in whose name, under what conditions.

| Element | Description |
|---|---|
| Authorization | Granted rights: scope, duration, granularity |
| Capability gating | Which capabilities are permitted, not just who |
| Delegation chains | Does authority transfer when agents delegate? |
| Temporal scope | Does authority persist or expire? |
| Revocation | How is authority withdrawn when trust changes? |

**Current gap:** A2A protocol has no authority layer for cross-agent delegation.

---

## Layer 3: Context ★

Who the human is, what their perspective is, and who has the right to challenge it.

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

★ = most contested layer. Every platform is trying to control this.

---

## Layer 4: Orchestration

What gets automated, what requires human input, and how visible is all of it.

| Element | Description |
|---|---|
| Automation scope | What is autonomous vs. requires approval vs. never delegated |
| Agent-to-agent handoffs | What can agents pass without involving the human? |
| Human-in-the-loop | Practical oversight, not theoretical |
| Zero friction vs. control | HITL without forms: notifications, progressive disclosure |
| UX heuristics | Nielsen's 10 heuristics apply directly here |
| Temporal UX | When must the human know something changed mid-task? |

**Note:** Architecture choice (hub-and-spoke vs. swarm) is an orchestration decision and an accountability decision. They are not separable.

---

## Layer 5: Accountability

Who decided what, when, on what basis — and what happens when it was wrong.

| Element | Description |
|---|---|
| Logging | Decision trail: who, what, when, on what basis |
| Attribution | Agent, model, human, or delegation chain? |
| Explainability | Why — readable by the human, not just as a log |
| Error recovery | Reversal path, notification, remediation |
| Audit vs. transparency | Right information, right person, right time |
| Temporal gap | Agents act in ms; accountability runs at human speed |
| Inter-stack | Who is accountable when Agent A fails at Human B's stack? |

---

## Relationship

Not a layer. The outcome.

Trust between human and agent — or between two humans mediated by their agents — emerges from five layers functioning consistently over time. It cannot be designed directly. The conditions for it can.

**Trust emerges when:**
- Intent is correctly understood
- Authority is appropriately bounded
- Context is current and honest
- Orchestration is visible and controllable
- Accountability is clear and actionable

**Distrust follows when any layer breaks.**

---

## The Inter-Stack Problem

The AX Stack describes one human, one agent, one context. The unsolved problem is two humans, each with their own stack, interacting through agents.

```
[Human A] → AX Stack A
                 |
         Inter-Stack Protocol
         - Intention Disclosure
         - Addressable Endpoint
         - Shared Vault (optional)
                 |
[Human B] → AX Stack B
```

**Intention Disclosure:** Every cross-stack push declares what it is, why now, and what response is expected. The receiving agent filters against the recipient's preferences, not the sender's optimization criteria.

A2A provides the transport. It does not provide the inter-stack governance layer.

---

## Related Work

- **Context Sovereignty** — who controls the canonical version of your context?
- **Temporal UX** — coordination problems across Human→Agent, Agent→Agent, Network→Network axes
- **Killerjourney** — apps are doors, not destinations; agents change who walks through them
- **Intention Disclosure** — the handshake protocol between two AX Stacks
- **Fork the Idea** — don't send the artifact, send the thinking

---

*Living document. Contributions and challenges welcome.*
