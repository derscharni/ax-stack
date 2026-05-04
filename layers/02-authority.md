# Layer 2: Authority

**Definition:** Who has the right to act, in whose name, under what conditions.

## Elements

| Element | Description |
|---|---|
| Authorization | Granted rights: scope, duration, granularity |
| Capability gating | Which capabilities are permitted, not just who |
| Delegation chains | Does authority transfer when agents delegate? |
| Temporal scope | Does authority persist or expire? |
| Revocation | How is authority withdrawn when trust changes? |

## Critical gap

**A2A protocol has no authority layer for cross-agent delegation.** When Agent A delegates to Agent B, whose authority applies? The spec is silent. Production multi-agent systems are inheriting this gap.

**Industry signal:** 91% of organizations now use agents. ~10% have a governance strategy (Fortune/JumpCloud, 2026 [UNVERIFIED — secondary citation]). The gap is the Authority layer missing in production.

## Common gaps

- **Conflating authentication with authorization.** Knowing who is acting is not the same as bounding what they can do.
- **No revocation pathway.** Authority granted at task-start often persists past task-end.
- **Capability-blind authorization.** "User X can use Agent Y" without specifying which of Y's capabilities. A research agent shouldn't auto-buy.

## Design checklist

- [ ] What is the smallest scope of authority that still gets the job done?
- [ ] Is authority bounded in time, not just role?
- [ ] How does authority propagate (or not) across agent-to-agent handoffs?
- [ ] What is the revocation interface — and is it human-operable in seconds, not days?

## Connects to

- **Intent** — intent must be validated against permitted scope.
- **Accountability** — authority bounds determine who is on the hook when something fails.
