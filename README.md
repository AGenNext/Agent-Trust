# Agent Trust

Agent Trust defines reusable trust, provenance, evidence, and audit contracts for AGenNext agentic systems.

## Scope

Agent Trust owns reusable trust concepts such as:

- provenance tracking
- evidence binding
- source reliability
- agent decision traceability
- A2A handoff auditability
- policy compliance evidence
- trust scoring
- human approval evidence
- artifact trust reports
- model/provider trust posture

## Consumers

- Agent-Team
- Agent-Knowledge
- Agent-Eval
- Agent-Analytics
- Model-Router
- Agent-Graph
- future AGenNext products

## Core Principle

```text
No trust without evidence.
No evidence without provenance.
No provenance without traceability.
```

## Trust Chain

```text
source evidence
  → extraction evidence
  → agent decision evidence
  → A2A handoff trace
  → artifact provenance
  → evaluation evidence
  → human approval evidence
```

## Repository Boundary

```text
Agent-Trust
  → defines trust and provenance contracts

Agent-Eval
  → evaluates quality and readiness

Agent-Analytics
  → measures trust-related events and metrics

Agent-Team
  → emits trust evidence through A2A and work logs

Agent-Knowledge
  → applies trust contracts to enterprise product workflows
```
