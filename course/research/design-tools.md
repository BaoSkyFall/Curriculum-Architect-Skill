# Research: Design Tools

Verified: 2026-10-01

## Role separation

| Layer | Tool example | What learners should understand |
|---|---|---|
| Design knowledge | UI/UX Pro Max, teacher rubric | hierarchy, spacing, typography, states, accessibility and review |
| Design generation | Google Stitch + MCP | prompt/brief → visual exploration → handoff artifact |
| Full-app abstraction | Lovable | prompt → application, with boundaries hidden behind a platform |

## Recommendation

Use a tool-agnostic `DESIGN_BRIEF.md` as the source of truth. Stitch is the preferred optional generator when the account and MCP integration work. Export a screenshot/HTML/spec and continue the lab without Stitch. Use UI/UX Pro Max to critique the artifact, not to define the course. Show Lovable only to make abstraction trade-offs visible.

## Why not choose one winner?

The tools do not solve the same problem. Picking Lovable because it creates a full app quickly would undermine the course outcome: students must understand the frontend/backend/API boundary. Picking Stitch as the foundation would make the course brittle if access or MCP packaging changes.

## Fallback artifact

The teacher supplies three screens as PNG or HTML: chat, company detail, and tier/results table. Students still write states and acceptance criteria.
