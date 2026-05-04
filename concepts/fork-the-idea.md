# Fork the Idea

**Status:** growing
**Origin:** Karpathy's IDEA.md pattern + agent-collaboration thinking

## Core principle

> **Don't send the artifact. Send the idea.**

The most valuable thing in a repo is not the code; it is the idea behind it. Applied to collaboration: the most valuable thing in a document is not the format, it is the thinking that produced it.

## Why this matters in agent flows

Agents are excellent at producing artifacts (slides, briefs, plans, posts). They are weaker at communicating the underlying intent that gives the artifact its meaning.

When Agent A pushes an output to Agent B, B receives a finished artifact. The reasoning that shaped it — what was rejected, what tradeoffs were considered, what assumptions are load-bearing — is gone.

Forking the idea preserves that reasoning. The downstream agent (or human) gets a working seed, not a closed deliverable.

## Design implications

- Cross-agent handoffs should travel with an `idea-md`-style summary: what we were trying to do, why this approach, what's still uncertain.
- This is the inverse of artifact-centric collaboration. The output is the byproduct; the idea is the asset.
- It is the cooperative version of Intention Disclosure: instead of "I'm pushing this finished thing," it is "I am sharing the thinking — fork it."

## Connects to

- **Intention Disclosure** — declares the push; Fork the Idea reframes what is in the push.
- **Inter-Stack Protocol** — proposes the carrier; Fork the Idea proposes the payload structure.
- **Agent Orchestration** — coordinated networks need a shared way to communicate underlying principles, not just outputs.
