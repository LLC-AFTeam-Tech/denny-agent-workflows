# Denny Agent Workflows

Reusable skills for preparing Denny Office assignments, handing context between Claude Code and Codex sessions, and reviewing an agent's result against its brief.

**Made in Russia by AFTEAM.**

This is a skills-only workflow package. It works with user-provided conversation context, files and review evidence. It does not include the native Denny Agents application, an MCP server or lifecycle hooks. It does not connect to a Mac, start agents, send Office assignments, activate a license or change application settings.

## Skills

| Skill | Result |
| --- | --- |
| `denny-office-brief` | A scoped, ready-to-paste Office assignment with acceptance criteria and validation requirements. |
| `denny-agent-handoff` | A continuation packet with decisions, changed artifacts, test evidence, blockers and the next action. |
| `denny-result-review` | An evidence-based acceptance recommendation or a focused rework request. |

The templates are Markdown documents for a person to paste or save. They are not a Denny wire protocol or an automatic import format. The skills work without a Denny license or account; the native application's functionality and access conditions are separate.

## Claude Code

Add this repository as a marketplace, then install the workflow package:

```text
/plugin marketplace add LLC-AFTeam-Tech/denny-agent-workflows
/plugin install denny-agent-workflows@afteam
```

Examples:

```text
/denny-agent-workflows:denny-office-brief
/denny-agent-workflows:denny-agent-handoff
/denny-agent-workflows:denny-result-review
```

For a local check, use `claude plugin validate /path/to/denny-agent-workflows` and load that folder with Claude Code's `--plugin-dir` option.

## Codex

The root `plugin.json` uses the portable Agent Plugins format. Add this repository through **Add plugin marketplace**, then select Denny Agent Workflows if your Codex version supports repository marketplaces. A separate ZIP of the plugin folder can be used for directory submission. Public directory review and publication are separate from this repository; this README does not claim either platform has approved the plugin.

Example prompts:

- “Turn this request into a Denny Office assignment with acceptance criteria.”
- “Prepare a handoff from this Claude Code session to Codex; preserve failed checks.”
- “Review this agent result against the brief and draft a rework request if needed.”

## Data and permissions

There is no backend, telemetry, bundled executable or automatic external request. The host assistant processes the inputs you provide under its own data policies. No skill asks for passwords, API keys, license keys or complete private session archives. Read [Privacy](PRIVACY.md) and [Support](SUPPORT.md).

The workflow text is MIT licensed. AFTEAM artwork has separate [asset terms](LICENSE-ASSETS.md). The native Denny applications are separate products and are not relicensed by this repository.

[Denny Agents](https://afteam.tech/denny/agents/en/) · [Denny](https://afteam.tech/denny/) · [AFTEAM](https://afteam.tech/)

Independent of Anthropic and OpenAI. Third-party product names identify the tools the workflows can be used with.
