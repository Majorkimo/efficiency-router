# Execution economy

Read only for inter-session coordination, gate submissions, heavy runs, tool-context decisions, or interpreting usage claims.

## Notifications that enable a decision

Send only authorized done, blocked, or question messages. Route a material risk requiring action as blocked or question, without hiding urgency. Preserve required user updates and operational alerts. Never acknowledge receipt, answer pure information, or wake dormant sessions solely to distribute rules. A receipt proves delivery, not completion.

Use this template, aiming for at most eight short lines:

```text
Status: DONE | BLOCKED | QUESTION
Scope: outcome and checked surface
Candidate: exact SHA or build identity
Evidence: accessible path
Checks: GREEN/RED; required checks still unrun
Deviations: failures, risks, or scope differences
Action: decision needed or next action and owner
```

Omit irrelevant fields, not important uncertainty. Keep detailed logs and test lists in evidence files. Eight lines is guidance, not a reason to omit a blocker. The receiver acts only if action is needed, without a receipt-only response.

## Ownership and deterministic status

The master coordinates decisions, blockers, results, owners, and evidence pointers; the assigned product session executes. Assign one owner to each distinct check. Required independent review remains a separate check with its own owner. Large agent fan-outs need Kimo's explicit yes; this rule does not authorize smaller delegations.

Use existing scripts for repetitive status extraction and monitoring. If none exists and recurring status work is necessary, create a minimal deterministic check within scope. It should identify the candidate, state, exit code, and evidence path, report relevant changes, and preserve full logs. Invoke model judgment only for changes that affect a decision or next action. Do not build a new monitoring service, poll unchanged states through model turns, or restart active runs merely to get a status report. Bound waits and preserve required user updates.

## Submit a complete candidate once

Before submission, the implementation owner checks the existing gate checklist: exact candidate, required artifacts, evidence, executed checks, known failures, unrun acceptance steps, and approvals. Record source SHA, any uncommitted candidate digest, checked scope, and relevant environment with evidence. Relevant environment includes configuration, dependencies, runtime, and deployed identity where applicable, without copying secrets.

Reuse evidence while those premises remain valid; rerun affected checks after relevant changes or unresolved failures. A different SHA needs an explicit applicability assessment, not an automatic green status. Never treat a local build as deployment or authenticated live acceptance. Preserve mandated independent review; do not duplicate the same audit without a distinct required purpose.

Bundle compatible small fixes within the authorized scope when this reduces resubmissions without expanding risk or delaying an urgent fix. An authorized fresh review needs current criteria, candidate, baseline, unresolved findings, and relevant security decisions, not the whole development history.

## Avoid infrastructure retries

Before heavy runs, use existing storage, memory, concurrency, and ownership admission checks. Diagnose resource pressure before retrying. Do not schedule routine reboots, terminate unrelated processes, or change machine settings merely to save tokens.

Prefer deterministic scripts for packaging and evidence checks. Keep full local logs and exit codes; return concise summaries and relevant failures. About 100 lines is an initial retrieval target, not a ceiling on necessary review. Filter at the source and expand relevant ranges when needed.

## Tool context and accounting

Discover tools and connectors on demand through supported host controls. Check actual loaded definitions before attributing overhead to configured connectors. Any session-scoped reduction must be authorized and preserve required capabilities; do not disable shared plugins or alter permissions.

Usage bands describe estimated work: low for narrow tasks, medium for bounded discovery and verification, high for broad context or difficult diagnosis, and extreme for several such drivers across systems. They are not token counts.

Context occupancy is not billed usage. Separate available uncached input, cache reads, cache writes, output, and reasoning telemetry; do not double-count aggregate fields or infer subscription usage from API prices. Include retries, handovers, and cache changes in comparisons. Use existing telemetry; no routine account queries or measurement loops. Shared account deltas are not task tokens, and resets invalidate subtraction. Never infer a saving percentage from context size or model size. Report actual avoided work without inventing a numerical saving.
