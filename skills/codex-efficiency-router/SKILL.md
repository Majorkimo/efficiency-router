---
name: codex-efficiency-router
description: Choose an available Codex model and reasoning effort for a substantive task, balancing complete, verified work against avoidable usage.
---

# Codex Efficiency Router

Use this skill when a new substantive task, or materially changed evidence, warrants a routing decision. Skip greetings, trivial lookups, and ordinary follow-ups that fit the current route.

1. Identify the required outcome, uncertainty, tools, verification gates, and cost of a wrong result from context already in hand. Do not inspect unrelated files, query account usage, or run competing models just to classify the task.
2. Choose among models actually offered by the current host. A clear extraction or mechanical edit usually needs less capability than implementation across several components. Conflicting evidence, novel architecture, or consequential release decisions may need more. A long prompt or the word "production" alone does not decide the model.
3. Choose reasoning effort independently. Use low for known steps, medium for several dependent steps, and high for genuinely difficult diagnosis or interacting constraints. Higher levels need exceptional unresolved complexity or an explicit user request. Respect the user's model and effort choice.
4. Give one short recommendation: `Route: <available model>, <supported effort> | Usage: <low/medium/high/extreme> | Driver: <main source of work>`. Reuse it until the task changes materially.
5. Apply a switch only through a supported host control and at a safe task boundary. If no control exists, continue on an adequate current route. A suggested route, queued handoff, or tool acknowledgement does not prove the next turn used it.

Among comparably capable routes, prefer lower total usage. Preserve correctness, security checks, tests, release evidence, and the user's authorization. Avoid repeated unchanged attempts, duplicate context reads, unnecessary agents, and a second routing decision on an internal handoff. A missing permission or unavailable service is not a model failure.

Finish the authorized work. A plan, build, or dispatch is not a completed outcome. Report an observed task usage delta only when available; otherwise give an honest usage band and main driver. Do not infer task cost from shared account percentages. This skill authorizes no purchase, billing change, permission change, deployment, or automatic model switch.

## Context pressure and successor sessions

Check at task or phase boundaries using evidence already available, without a monitoring loop. Prepare a compact handover when either trigger occurs:

- The host reports current context occupancy at or above 80%, or warns that the context is nearly full. This threshold is a local safety margin, not a platform limit. Cumulative token totals, account usage, session age, and message count are not context occupancy.
- Since the latest verified checkpoint, context loss has required two separate recoveries of the same unchanged decision, owner, permission, or candidate from older history, despite its presence in that checkpoint. Note the two incidents briefly; checking a changed source does not count.

Without reliable telemetry, use only the second trigger and describe pressure qualitatively. A single compaction or large attachment alone is insufficient. Finish in place when only final verification and delivery remain and can be completed reliably; otherwise transfer at the next safe boundary before another substantial phase.

Creating a successor requires explicit user authorization, including an applicable standing instruction. This skill grants none. With authorization and a supported host control, create one fresh session with the handover instead of copying the full history. Otherwise retain the checkpoint and explain the missing authorization or capability when it affects progress.

Include the goal, acceptance criteria, verified status, decisions, unresolved facts, open work, next action, permissions, pauses, source session, workspace, owners, exact candidate, evidence pointers, and active-run custodians. Transfer only task-relevant information to the authorized destination; reference secrets without copying their values. Resume without repeating settled discovery or routing the internal handover again.

Keep the existing workspace and owners. Do not interrupt a mutation, duplicate a writer, or restart an active run. Confirm receipt through a bounded host status check before ending overlapping source work; a creation receipt is not task completion. Track pending setup, and reconcile ambiguous creation results before retrying. Retain the original session and record its successor in an existing coordination record when applicable. Inherited trigger incidents never justify another rotation; the successor requires fresh evidence from its own context.

These are agent instructions, not an installed background monitor or a guarantee of lower token usage.
