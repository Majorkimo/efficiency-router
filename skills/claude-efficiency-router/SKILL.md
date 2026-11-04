---
name: claude-efficiency-router
description: Choose an available Claude Code model and reasoning depth for substantive work, while preserving quality, user control, and included-usage boundaries.
---

# Claude Efficiency Router

Use this skill when starting a substantive task or when new evidence changes the task's difficulty. Keep the current route for routine follow-ups, and skip routing for trivial requests.

1. Decide what must be delivered and verified. Use the context already available; do not query usage, launch comparison runs, or inspect unrelated project files just to pick a model.
2. Choose from the model families and controls actually shown by the host. A bounded, mechanical task may fit a smaller model. Ordinary implementation and debugging may fit a balanced model. Conflicting evidence, difficult architecture, or consequential synthesis may justify a stronger model. These are task judgments, not claims about fixed prices or benchmarks.
3. Set reasoning depth separately: low for known steps, medium for dependent steps, and high for difficult diagnosis or interacting constraints. Use higher settings only when the unresolved work warrants them and the host supports them. Follow an explicit user choice.
4. State one brief recommendation: `Route: <available model>, <supported effort> | Usage: <low/medium/high/extreme> | Driver: <main source of work>`. Reassess only after a material change.
5. Change settings only through a supported control at a safe boundary. Do not interrupt a running task or claim a switch based on a recommendation alone. If switching is unavailable, continue on an adequate current route.

Reduce repeated reads, unchanged retries, and duplicate handoffs, but never weaken tests, security, migration safety, or release checks to save usage. Keep one source writer unless the user explicitly authorizes separate work. An internal handoff does not need another routing pass. Account-wide usage figures do not measure this task's cost.

This skill is guidance, not spending permission. Do not enable paid continuation, recharge, fast modes, API billing, new keys, or account changes. Stop at a genuine allowance boundary and ask for a decision only when needed. Finish with an observed task delta if available, otherwise a usage band, main driver, and actual waste avoided.
