# Frameworks — what they cover, what they miss

A short field guide. The AX Stack is not a replacement for these — it sits across them.

## A2A (Agent-to-Agent Protocol)

**What it covers:** Transport for inter-agent communication. Routing, message format, capability advertisement.
**What it misses:** Authority delegation, semantic intent, accountability across boundaries.
**AX Stack relation:** A2A is the pipe. Inter-Stack Protocol is what sits above the pipe.

## MCP (Model Context Protocol)

**What it covers:** Tool and resource access for models. Standardized way for agents to read context and call tools.
**What it misses:** Sovereignty (whose vault?), provenance (where did the context come from?), critique license (can the agent challenge it?).
**AX Stack relation:** MCP serves the Context layer's plumbing. It does not address the Context Sovereignty question.

## Nielsen Heuristics (10 Usability Heuristics)

**What it covers:** UI design principles, applicable directly to the Orchestration layer.
**What it misses:** Anything about agent-to-agent flows, accountability, or context decay.
**AX Stack relation:** Hard requirements at Layer 4. Visibility, user control, error prevention all map.

## Karpathy IDEA.md pattern

**What it covers:** The idea is the asset, not the code. Foundational for `concepts/fork-the-idea.md`.
**What it misses:** Operational protocol; it's a pattern, not a stack.
**AX Stack relation:** Direct ancestor of Fork the Idea, indirectly informs Intent layer.

## Saarinen / Linear (Accountability as design constraint)

**What it covers:** Accountability must be a pre-action design constraint, not post-hoc logging.
**What it misses:** Cross-stack and EU AI Act–level legal-time accountability.
**AX Stack relation:** Reframes Accountability as constraining Orchestration, not the reverse.

## EU AI Act / governance frameworks

**What it covers:** Legal-time accountability, audit obligations, risk classification.
**What it misses:** Design-time accountability; the in-the-moment user surface.
**AX Stack relation:** Sits above Accountability layer. Design the layer; comply with the framework.

## Microsoft Governance Toolkit (2026)

**What it covers:** Per-message policy evaluation in inter-agent flows.
**What it misses:** Semantic intent layer.
**AX Stack relation:** Implements the plumbing of Intention Disclosure without naming it.

## What the AX Stack adds

A coherent map of where each of the above operates — and where the gaps between them produce the trust failures we are now seeing in production agent systems.
