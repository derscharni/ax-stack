# Inter-Stack Protocol

**Status:** growing
**Origin:** "The Address Problem" + Multiplayer AI discussion

## Core idea

The AX Stack describes a single stack: one human, one agent, one interaction.

```
Intent → Authority → Context ★ → Orchestration → Accountability → Relationship
```

The unsolved problem is **two humans, each with their own stack, interacting through agents.**

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

## What sits above A2A

A2A and MCP solve transport and tool access. They do not solve:

- **Semantics** — what does this push mean to the recipient?
- **Authority handoff** — does Agent A's authority extend to Agent B?
- **Context fidelity** — does context survive the crossing intact?
- **Accountability** — who is on the hook for inter-stack failures?

The Inter-Stack Protocol is the semantic header layer above A2A.

## Three components

1. **Intention Disclosure** — every cross-stack push declares what / why-now / expected-action.
2. **Addressable Endpoint** — agents need a stable, recipient-controlled inbox, not best-effort delivery.
3. **Shared Vault (optional)** — for ongoing collaboration, both stacks may converge on shared context with explicit sovereignty rules.

## Why this is not solved

MCP+A2A are becoming the de-facto stack for inter-agent communication. The TCP-analogy holds — these protocols solve transport, not semantics. No external source yet names the semantic header layer this concept proposes.

## Open questions

- Is the Inter-Stack Protocol a spec, an open-source library, or an emergent convention?
- How does it interact with regulated cross-organization data flows?
- What is the failure mode when one side speaks the protocol and the other does not?
