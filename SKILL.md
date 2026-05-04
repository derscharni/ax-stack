---
name: ax-stack
description: Apply the AX Stack — a five-layer design framework for human-agent interaction (Intent → Authority → Context → Orchestration → Accountability → Relationship). Use this skill when analyzing agent setups, designing agentic products, evaluating governance gaps, reviewing multi-agent architectures, or producing design artifacts (briefings, audits, recommendations) for systems where humans and AI agents work together.
version: 0.1.0
author: Jens Scharnetzki
---

# AX Stack — Claude Skill

A design framework for the age of agents. Five operational layers. One emergent outcome (trust).

## When to invoke

Trigger this skill when the user asks for any of the following:

- **Audit:** "Analyze my agent setup against the AX Stack" / "Where are the weaknesses in my Authority layer?"
- **Design:** "Design the Context layer for this product" / "What does Accountability mean for our multi-agent flow?"
- **Diagnosis:** "Why is trust breaking down in this agent flow?" / "Which layer is missing?"
- **Bridging:** "How do two AX Stacks interact?" (Inter-Stack Protocol)
- **Role-conditioned framing:** when the user identifies as Designer, Architect, Product Owner, or CTO and is reasoning about agent products

## Method

1. **Identify the question's layer.** Not every question spans all five. Locate the one(s) that matter.
2. **Read the relevant layer file** in `layers/`. Each layer file has: definition, elements, common gaps, design checklist.
3. **Cross-link with concepts** in `concepts/` when the question is about cross-stack behavior (Intention Disclosure, Inter-Stack Protocol) or scaling effects (Collective Forgetting, Fork the Idea).
4. **Frame outputs by role:**
   - **Designer:** what does this layer feel like for the user?
   - **Architect:** what protocols, contracts, data flows live here?
   - **Product Owner:** what trade-offs, what next milestone, what risk?
   - **CTO:** what governance, what compliance, what blast radius?
5. **Name the gap before naming the fix.** AX Stack work is diagnostic first, prescriptive second.

## Files

- `README.md` — framework overview (visual stack, layer summaries)
- `ARTICLE.md` — long-form narrative version of the framework
- `layers/01-intent.md` … `layers/05-accountability.md` — per-layer deep dives
- `concepts/intention-disclosure.md` — handshake protocol between two stacks
- `concepts/inter-stack-protocol.md` — semantic layer above A2A
- `concepts/fork-the-idea.md` — send the idea, not the artifact
- `concepts/collective-forgetting.md` — anti-Habsburg-effect in agent networks
- `references/frameworks.md` — Nielsen, A2A, MCP, Karpathy, Saarinen — what they cover and what they miss
- `references/related-work.md` — Context Sovereignty, Temporal UX, Killerjourney

## Trust contract

The AX Stack is opinionated and incomplete. Use it as a diagnostic lens, not as a checklist. When applying it:

- Surface uncertainty explicitly. Mark `[UNVERIFIED]` for any quantitative claim not directly cited.
- Distinguish design-time accountability from legal-time accountability (EU AI Act, etc.).
- Flag when a problem belongs above the framework (governance, regulation) or below (transport protocols).
