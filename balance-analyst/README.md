# Balance Analyst

An LLM agent that reads game playtest telemetry (per-run JSON logs), computes balance statistics through tool calls, writes a balance report and proposes tuning changes.

**Planned:**
- Node.js + TypeScript, Claude API with tool use
- Tools: load runs, win/loss per level, damage taken by module, weapon usage, wave duration
- Structured output: report + proposed changes to tuning values
- Evals: every number the model claims is checked against computed stats
- Cost tracking per report

Status: not started.
