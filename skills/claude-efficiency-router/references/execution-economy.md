# Execution economy

Read only for inter-session coordination, release submissions, resource-heavy jobs, tool-context decisions, or interpreting usage claims.

## Notifications that enable a decision

Message another session only within existing human authorization, when work finishes, a blocker needs action, a decision is needed, or a material risk changes. Suppress receipt-only acknowledgements, unchanged progress, and acknowledgement-of-acknowledgement loops. Required user progress updates and operational alerts still apply. Do not wake dormant sessions solely to distribute efficiency rules; apply them when work resumes. A receipt proves delivery, not completion.

Aim for eight short lines, not a hard cap. Include outcome and checked scope, exact candidate SHA/build identity when applicable, an accessible evidence path, deviations or unchecked gates, and any required decision or next action. Keep detailed test lists in existing evidence files. Include enough context to act without another clarification round; never omit a blocker to meet a length target. A path is useful only if the recipient can access it.

## Submit a complete candidate once

The implementation owner checks the existing gate checklist before submission: candidate identity, required artifacts and evidence, executed checks, known failures, and unrun acceptance steps. Reuse evidence only for the same applicable candidate and unchanged relevant environment; record exceptions honestly. Keep mandated independent review independent. Do not duplicate the same audit without a distinct required purpose.

Bundle compatible small fixes within the authorized release scope when this reduces resubmissions without expanding risk or delaying an urgent fix. A fresh review session, when authorized and useful, still needs the current criteria, candidate, baseline, prior unresolved findings, and relevant security decisions. Do not carry the entire development conversation or discard critical history.

## Avoid infrastructure retries

Before a resource-heavy job, use the project's existing storage, memory, concurrency, and ownership admission checks. Diagnose resource pressure before retrying. Do not schedule routine reboots, terminate unrelated processes, or change machine settings merely to save tokens.

Prefer existing deterministic scripts for repetitive packaging, status extraction, and evidence checks. Preserve exit codes and full local logs; return a concise summary plus relevant failures. Roughly 100 lines is an initial retrieval target, not a ceiling on a required diff or security review.

## Tool context and accounting

Prefer the host's supported deferred tool discovery. Check actual loaded definitions before attributing overhead to configured connectors. Do not disable shared plugins, permissions, or needed tools; any session-scoped reduction must preserve the work and be authorized.

Context occupancy is not billed usage. Separate available uncached input, cache reads, cache writes, output, and reasoning telemetry; do not double-count aggregate fields or infer subscription usage from API prices. Include retries, handoffs, and cache changes in any comparison. Use existing telemetry only, without monitoring loops or account queries. Never claim a cost multiplier or percentage saving from context size alone.
