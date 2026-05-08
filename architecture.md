# Prompt System Architecture

## 1) Core principle

One signal can lead to different outcomes:

- content opportunity,
- sales opportunity,
- both,
- backlog,
- delete.

The architecture uses routing instead of a single linear generation chain.

## 2) Layer map

1. **Signal Intelligence Layer**
   - Research Agent
   - Filter Agent
   - Signal Evaluator Agent
2. **Routing Layer**
   - Signal Router
3. **Content Production Layer**
   - Hook Agent
   - Content Agent
   - Anti-Generic Agent
   - Grader Agent
   - Learning Log Agent
4. **Commercial Activation Layer**
   - Lead Qualification Agent
   - Product Match Agent
   - Outreach Angle Agent
   - Pre-Diagnostic Draft Agent
   - Solution Steer Agent
   - Deal Follow-Up Agent
5. **Quality + Learning Layer**
   - Quality Review
   - Commercial Grader
   - Commercial Learning Log

## 3) Routing decision schema

```json
{
  "routing_decision": "content | commercial | both | backlog | delete",
  "reason": "",
  "next_agents": [],
  "priority": "high | medium | low"
}
```

## 4) Anti-generic protocol

Every customer-facing draft must pass these checks:

- concrete event reference,
- concrete business tension,
- clear next step,
- no abstract marketing filler,
- no claims without evidence.

## 5) Human-in-the-loop points

Mandatory manual review before:

- first outbound message,
- pre-diagnostic delivery,
- commercial proposal,
- sensitive follow-up.

## 6) Operational outcomes

- faster first response cycle,
- stronger signal-to-action conversion,
- less "generic AI" output,
- clearer upgrade path from initial task to strategic engagement.
