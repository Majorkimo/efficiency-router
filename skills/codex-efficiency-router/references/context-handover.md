# Context handover

Read only when evaluating a context trigger or preparing an authorized successor.

Check at task or phase boundaries using evidence already available, without a monitoring loop. Prepare a compact handover when either trigger occurs:

- The host reports current context occupancy at or above 80%, or warns that the context is nearly full. This threshold is a local safety margin, not a platform limit. Cumulative token totals, account usage, session age, and message count are not context occupancy.
- Since the latest verified checkpoint, context loss has required two separate recoveries of the same unchanged decision, owner, permission, or candidate from older history, despite its presence in that checkpoint. Note the two incidents briefly; checking a changed source does not count.

Without reliable telemetry, use only the second trigger and describe pressure qualitatively. A single compaction or large attachment alone is insufficient. Finish in place when only final verification and delivery remain and can be completed reliably; otherwise transfer at the next safe boundary before another substantial phase. A phase boundary alone never triggers a transfer.

Creating a successor requires explicit user authorization, including an applicable standing instruction. This skill grants none. With authorization and a supported host control, create one fresh session with the handover instead of copying the full history. Otherwise retain the checkpoint and explain the missing authorization or capability when it affects progress.

Include the goal, acceptance criteria, verified status, decisions, unresolved facts, open work, next action, permissions, pauses, source session, workspace, owners, exact candidate, evidence pointers, and active-run custodians. Transfer only task-relevant information to the authorized destination; reference secrets without copying their values. Resume without repeating settled discovery or routing the internal handover again.

Keep the existing workspace and owners. Do not interrupt a mutation, duplicate a writer, or restart an active run. Confirm receipt through a bounded host status check before ending overlapping source work; a creation receipt is not task completion. Track pending setup, and reconcile ambiguous creation results before retrying. Retain the original session and record its successor in an existing coordination record when applicable. Inherited trigger incidents never justify another rotation; the successor requires fresh evidence from its own context.

These are agent instructions, not an installed background monitor or a guarantee of lower token usage.
