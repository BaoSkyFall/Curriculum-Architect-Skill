# Tech Radar

Last verified: 2026-10-01
Review interval: before every cohort, and immediately after a major release or access change.

## Summary

| Technology | Role | Status | Teach | Risk | Decision |
|---|---|---|---|---|---|
| OpenAI Codex | coding-agent implementation | active | optional primary | medium | Use if instructor already supports Codex; concepts remain portable |
| Claude Code | coding-agent implementation | active | optional primary | medium | Use as the single class track if Anthropic access is easier |
| Oh My Codex (OMX) | orchestration layer | active / fast-moving | optional | high | Teach orchestration concepts; demo only after native agent workflow works |
| Oh My ClaudeCode (OMC) | orchestration layer | active / fast-moving | optional | high | Same role as OMX; do not teach both in the core path |
| MCP | tool/data connection protocol | active | yes | medium | Teach the boundary and one safe server, not a catalog of servers |
| Google Stitch + Stitch MCP | design generation / handoff | active / fast-moving | optional | high | Use for design artifact if access is reliable; keep screenshot/spec fallback |
| UI/UX Pro Max | design intelligence skill | active community project | optional | medium | Use as a rubric/reference, not as the design foundation |
| Lovable | full-app abstraction | active | comparison only | high | Show why abstraction is useful and what it hides |
| React + Vite | frontend implementation | active | yes | low | Stable enough for a visible frontend boundary |
| Node.js API | backend implementation | active | yes | low | Keep endpoint logic small; use one language across FE/BE |
| SQLite / Postgres | persistence | active | yes | low | SQLite for lab; Postgres/Supabase optional for shared deployment |
| LLM provider SDK | model call | active / fast-moving | yes | medium | Teach messages and structured output; keep provider adapter thin |
| Embeddings + retrieval | semantic search concept | active | yes | medium | Implement small dataset first; vector DB is optional |

## Entries

### Codex / Claude Code

status: active
last_verified: 2026-10-01
evidence: [OpenAI Codex docs](https://platform.openai.com/docs/codex), [Claude Code overview](https://code.claude.com/docs/en/overview)

Teaching decision: choose one runtime for setup and labs. Outcomes are agent, context, tool, verification and task decomposition—not memorizing a CLI.

### OMX / OMC

status: active / fast-moving
last_verified: 2026-10-01
evidence: [oh-my-codex](https://github.com/Yeachan-Heo/oh-my-codex), [oh-my-claudecode](https://github.com/Yeachan-Heo/oh-my-claudecode)

Teaching decision: neither is obsolete based on current repository activity, but both are too fast-moving to be the course spine. Use one short implementation lab after native agent concepts.

### MCP

status: active
last_verified: 2026-10-01
evidence: [MCP introduction](https://modelcontextprotocol.io/docs/getting-started/intro)

Teaching decision: explain MCP as a standard boundary for exposing tools/data to an agent. Students must inspect permissions and failure modes; no broad server marketplace survey.

### Stitch / Stitch MCP

status: active / fast-moving
last_verified: 2026-10-01
evidence: [Google Stitch](https://stitch.withgoogle.com/), [Google Stitch skills](https://github.com/google-labs-code/stitch-skills), [Stitch MCP CLI](https://github.com/davideast/stitch-mcp)

Teaching decision: useful for generating design explorations and handoff artifacts. Because access and integration can change, every lab must work from a screenshot, HTML export or design brief if Stitch is unavailable.

### UI/UX Pro Max

status: active community project
last_verified: 2026-10-01
evidence: [repository](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)

Teaching decision: optional design-intelligence reference for hierarchy, typography, spacing and review. Do not make its command syntax a prerequisite.

### Lovable

status: active
last_verified: 2026-10-01
evidence: [Lovable docs](https://docs.lovable.dev/introduction)

Teaching decision: use for a 10-minute compare-and-contrast. It is a full-app abstraction, so it is not interchangeable with Stitch or UI/UX Pro Max and should not replace boundary lessons.

### LLM / retrieval stack

status: active / fast-moving
last_verified: 2026-10-01
evidence: [OpenAI embeddings](https://platform.openai.com/docs/guides/embeddings), [OpenAI retrieval](https://platform.openai.com/docs/guides/retrieval), [Supabase AI](https://supabase.com/docs/guides/ai)

Teaching decision: keep an adapter around the provider, use structured output, and evaluate retrieval on a small labeled test set. Do not promise model-specific behavior across providers.
