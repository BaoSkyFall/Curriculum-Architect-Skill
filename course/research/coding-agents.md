# Research: Coding Agents and Orchestration

Verified: 2026-10-01

## Evidence

- Claude Code official docs describe an agentic coding tool that reads a codebase, edits files, runs commands and integrates with development tools: <https://code.claude.com/docs/en/overview>.
- OpenAI maintains current Codex documentation at <https://platform.openai.com/docs/codex>.
- Oh My ClaudeCode describes a teams-first multi-agent orchestration layer: <https://github.com/Yeachan-Heo/oh-my-claudecode>.
- Oh My Codex describes hooks, agent teams and workflow support for Codex CLI: <https://github.com/Yeachan-Heo/oh-my-codex>.
- MCP has a current protocol introduction and getting-started material: <https://modelcontextprotocol.io/docs/getting-started/intro>.

## Teaching decision

Teach the stable model first:

```text
model → agent → context → tools → skills/MCP → subagents → orchestration → verification
```

Then run one tool lab. Students write an agent working agreement containing task, context files, constraints, acceptance criteria and verification command. They do not need to install both OMC and OMX.

## Risks

- CLI flags, installation and names can change quickly.
- Multi-agent parallelism can increase cost, context collisions and debugging difficulty.
- A successful generated patch is not proof of correctness.

## Fallback

If an orchestration layer fails, use native agent tasks and a written handoff table. The learning objective remains decomposition and verification.
