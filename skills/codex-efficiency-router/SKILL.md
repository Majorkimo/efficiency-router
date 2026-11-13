---
name: codex-efficiency-router
description: Choose an available Codex model and reasoning effort for a substantive task, balancing complete, verified work against avoidable usage.
---

# Codex Efficiency Router

## Shared mandatory core

Choose an available model suited to each substantive task and, independently, the lowest sufficient reasoning depth. Optimize total effort through a verified result, including failed attempts, context loading, reviews, and handovers. Prefer lower usage among equally suitable routes; never sacrifice correctness, security, required checks, or approvals. Respect explicit user choices. Reuse an adequate route on continuations and reassess when the task or evidence materially changes. Skip routing for trivial requests; never route an internal handover twice.

Use existing context to assess uncertainty, interacting constraints, tools, and consequences of error. Mechanical work may suit a smaller model; implementation may need balanced capability; unresolved consequential complexity may need stronger judgment. Low reasoning fits known steps, medium fits dependent steps, and high fits difficult diagnosis. Higher settings need demonstrated need or explicit instruction. Neither prompt length nor a task label fixes the route. Missing access is not a model failure.

Give one short route line with model, effort, estimated usage band, and main driver. Apply changes only through supported host controls; a recommendation or receipt does not prove a switch. Continue on an adequate current route when switching is unavailable. Report only material estimate changes.

Before each action, silently ask: necessary, valid evidence already available, smaller query sufficient? This check needs no extra call or reasoning turn. Read details on demand, search known paths, batch independent reads, and use deterministic tools. Inspect a failed attempt before choosing another; retry only when evidence or conditions justify it.

Bound tool output to relevant hits, ranges, errors, and summaries, initially about 100 lines. Keep full logs and exit codes on disk. Expand when required evidence warrants it; never truncate away a risk or failure. Bind evidence to the exact source SHA or candidate identity, checked scope, and relevant environment. Reuse it until its premises change; rerun affected checks when they do.

Keep the master session focused on coordination: decisions, blockers, results, owners, and evidence pointers. Product sessions own execution. Assign one owner per check and avoid duplicate audits while preserving mandatory independent review. Delegate only within authorization; large agent fan-outs require Kimo's explicit yes. Do not create agents merely to claim savings.

Send authorized inter-session messages only for done, blocked, or a question requiring action. Aim for eight lines using status, scope, SHA, evidence path, green/red checks, deviations, and decision or next action. Never send acknowledgements or answer pure information. Preserve necessary user updates and risk alerts; do not broadcast to dormant sessions.

Use deterministic scripts for repetitive status checks and monitoring; involve the model only when a relevant change needs judgment. Preserve failures and active-run ownership. Before submission, self-check the existing gate checklist, candidate, artifacts, executed checks, and unrun acceptance steps. Bundle compatible small fixes within scope. A plan, dispatch, or build alone is not completion.

Transfer context only at a reported current occupancy of at least 80%, an equivalent host warning, or repeated context loss: two recoveries of the same unchanged checkpointed fact. A phase boundary is the transfer time, never an independent trigger. Without reliable occupancy telemetry, use repeated loss only. Finish reliable final verification in place; otherwise transfer at the next safe boundary with authorization, a compact complete checkpoint, and one successor. Preserve owners, permissions, unresolved facts, and active runs; verify receipt without overlapping execution.

Load tools and connectors according to each session's needs using supported deferred discovery. Preserve required capabilities and shared configuration. Before heavy runs, check storage, memory, concurrency, and ownership admission; diagnose resource pressure instead of imposing a fixed restart schedule.

At completion, use existing task telemetry or an honest estimated usage band, main driver, and actual avoided waste. Do not query accounts solely for reporting, infer task cost from shared percentages, or claim unmeasured savings. These instructions grant no spending, permission changes, or release authority and install no automatic enforcement.

## Codex adapter

Use the model IDs and reasoning efforts actually exposed by Codex. When authorized native same-task routing is available, apply it without a separate launcher. Verify host settings and the subsequent turn's recorded route before claiming a switch; a queued handoff is insufficient. If that control is absent, retain an adequate route and disclose the limitation when material. Do not create another task merely to switch models or infer spending permission.

## Details on demand

Read [execution-economy.md](references/execution-economy.md) for inter-session coordination, gate submission, heavy runs, tool context, or usage comparisons. Read [context-handover.md](references/context-handover.md) only when evaluating a context trigger or preparing an authorized successor.
