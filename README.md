# Efficiency Router

Two small agent skills for choosing a capable model and a suitable reasoning depth without turning every task into a model comparison. One skill is for Codex, and the other is for Claude Code.

The shared rule is simple: choose for the work in front of you, keep the user's choice and the current task intact, and save usage only when the result remains equally sound. A skill is guidance. It does not grant spending, change account settings, or switch models by itself.

## Install

Clone this repository, then copy the appropriate folder into your agent's skills directory:

| Agent | Project installation | User installation |
| --- | --- | --- |
| Codex | `.agents/skills/codex-efficiency-router/` | `~/.agents/skills/codex-efficiency-router/` |
| Claude Code | `.claude/skills/claude-efficiency-router/` | `~/.claude/skills/claude-efficiency-router/` |

For example, from your project root after cloning:

```sh
mkdir -p .agents/skills .claude/skills
cp -R efficiency-router/skills/codex-efficiency-router .agents/skills/
cp -R efficiency-router/skills/claude-efficiency-router .claude/skills/
```

Start a new agent session so it can discover the installed skill. Invoke `$codex-efficiency-router` or `$claude-efficiency-router` explicitly if your host supports skill invocation, or ask the agent to use the relevant skill for a substantive task.

## What it changes

- Match model capability to the outcome and uncertainty, then choose reasoning depth separately.
- Reuse a good route on ordinary follow-ups. Reassess when the task or evidence changes materially.
- Avoid account usage checks, repeated model trials, and duplicate handoffs merely to make a routing decision.
- Keep verification, security, release gates, and user permissions at their original strength.
- Detect context pressure at phase boundaries and, with explicit user authorization and host support, transfer work to a fresh session using a compact handover.

The skills use the models and controls actually available in the host. They do not assume that a model name, price, or control will remain available. If the host cannot change model or effort within the current task, the agent should continue on an adequate current route and report the limitation when it matters.

## Scope

The package contains only instructions, including successor-session triggers and safeguards against repeated transfers. It installs no background context monitor and grants no permission to create sessions. It includes no telemetry, account integration, automated switching script, provider key, or billing action. It does not replace project instructions or the user's explicit preferences.

## License

MIT. See [LICENSE](LICENSE).
