# Intention Disclosure

**Status:** growing
**Origin:** "The Address Problem" article discussion

## Core idea

When an agent proactively pushes something to another agent (or human), it must explicitly declare:

- **What** it is (analysis, decision-vehicle, FYI, actionable item)
- **Why now** (trigger: job done, deadline, relevance event)
- **What is expected** (action: nothing, review, decide, forward)

The receiving agent filters against the recipient's preferences, not the sender's optimization criteria.

## Why this matters

A2A protocol is the transport layer. It deliberately does not specify what sits above the pipe. Without intention disclosure, every push is an unsolicited interruption with no semantic header.

What an agent pushes is never just data. It is a crystallized, opinionated interpretation of something. The receiving human needs to know whose interpretation just arrived — and whether they actually need it now.

## Industry signal

Microsoft Governance Toolkit (April 2026): "every inter-agent message is evaluated against policy before execution." That is intention disclosure as infrastructure — without the semantic layer.

The pattern is being implemented without being named.

## Design implications

- A push without a declared `what / why-now / expected-action` triple is malformed.
- Receiver-side filtering is the AX Stack equivalent of inbox rules — but at the Authority layer, not the UI layer.
- Intention Disclosure is the handshake protocol between two AX Stacks. It does not replace A2A; it sits above it.

## Open questions

- What is the canonical schema for the disclosure header?
- Who maintains the recipient's filter rules — the user, the agent, or a vendor?
- How are bad-faith disclosures (sender lies about urgency) detected?
