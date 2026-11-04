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
