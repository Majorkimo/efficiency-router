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

## Context pressure and successor sessions

Check at task or phase boundaries using evidence already available, without a monitoring loop. Prepare a compact handover when either trigger occurs:

- The host reports current context occupancy at or above 80%, or warns that the context is nearly full. This threshold is a local safety margin, not a platform limit. Cumulative token totals, account usage, session age, and message count are not context occupancy.
- Since the latest verified checkpoint, context loss has required two separate recoveries of the same unchanged decision, owner, permission, or candidate from older history, despite its presence in that checkpoint. Note the two incidents briefly; checking a changed source does not count.

Without reliable telemetry, use only the second trigger and describe pressure qualitatively. A single compaction or large attachment alone is insufficient. Finish in place when only final verification and delivery remain and can be completed reliably; otherwise transfer at the next safe boundary before another substantial phase.

Creating a successor requires explicit user authorization, including an applicable standing instruction. This skill grants none. With authorization and a supported host control, create one fresh session with the handover instead of copying the full history. Otherwise retain the checkpoint and explain the missing authorization or capability when it affects progress.

Include the goal, acceptance criteria, verified status, decisions, unresolved facts, open work, next action, permissions, pauses, source session, workspace, owners, exact candidate, evidence pointers, and active-run custodians. Transfer only task-relevant information to the authorized destination; reference secrets without copying their values. Resume without repeating settled discovery or routing the internal handover again.

Keep the existing workspace and owners. Do not interrupt a mutation, duplicate a writer, or restart an active run. Confirm receipt through a bounded host status check before ending overlapping source work; a creation receipt is not task completion. Track pending setup, and reconcile ambiguous creation results before retrying. Retain the original session and record its successor in an existing coordination record when applicable. Inherited trigger incidents never justify another rotation; the successor requires fresh evidence from its own context.

These are agent instructions, not an installed background monitor or a guarantee of lower token usage.
