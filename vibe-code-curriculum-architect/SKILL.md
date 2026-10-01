---
name: vibe-code-curriculum-architect
description: Design, research, and review coherent technical curricula for non-technical learners, especially Vibe Coding courses.
metadata:
  short-description: Build researched, project-driven curricula
---

# Vibe Code Curriculum Architect

## Purpose

Turn rough course ideas, topic lists, blockers, and tool questions into a teachable curriculum. Work as one coordinated skill with six responsibilities: curriculum architecture, technical research, learning design, project design, coherence review, and tech-radar maintenance.

## Use This Skill When

- A user wants to design or restructure a course.
- A topic list needs sequencing, prerequisites, lessons, labs, or assessment.
- A current tool, SDK, model, platform, or agent framework must be evaluated for teaching.
- An existing curriculum needs a coherence review.

Do not use it for LMS management, course hosting, video production, automatic full-app delivery, or whole-course grading.

## Core Rule

Build every topic through:

```text
Concept -> Mental Model -> Implementation -> Practice -> Integration
```

Teach the system before the vendor tool. A tool is an implementation example, not the learning objective.

## Workflow

1. **Intake:** extract audience, goals, constraints, duration, current topics, and unknown decisions. Preserve the user's language in generated prose.
2. **Research gate:** verify every fast-moving technology with current official documentation and other relevant evidence. Record date, sources, role, alternatives, stability, cost, and risk in `TECH_RADAR.md`.
3. **Outcomes:** write observable student outcomes before choosing lessons. Keep outcomes at mental-model and architecture level unless syntax is explicitly required.
4. **Dependencies:** create `PREREQUISITE_MAP.md`; add, reorder, merge, or remove topics when prerequisites or difficulty progression require it.
5. **Architecture:** produce course, module, lesson, lab, assessment, and capstone specifications using the templates in this package.
6. **Review:** check goal alignment, prerequisite integrity, difficulty progression, concept coverage, practicality, tool longevity, project integration, assessment quality, and non-tech accessibility.
7. **Emit:** write a self-contained course workspace with `README.md`, `COURSE_SPEC.md`, `LEARNING_OUTCOMES.md`, `CURRICULUM_MAP.md`, `PREREQUISITE_MAP.md`, `TECH_RADAR.md`, `DECISIONS.md`, `CAPSTONE.md`, `research/`, and `lessons/`.

## Research Gate

Never rely on model memory alone for current tools, frameworks, libraries, models, SDKs, platforms, MCP servers, or agent products. If live research is unavailable, mark the decision as unverified and avoid presenting it as a current recommendation. Prefer official documentation, release notes, active repositories, and maintainer statements. Separate facts from the teaching decision.

Use `references/research-policy.md` and `references/tool-selection.md` when selecting or comparing tools. Use `templates/tech-radar.md` and `templates/adr.md` to record the result.

## Curriculum Decisions

- Start with software mental models, then introduce syntax only when it unblocks building.
- Make each module contribute an observable artifact toward the capstone.
- Teach frontend, backend, API, database, LLM, data pipeline, retrieval, agents, skills, MCP, and multi-agent systems as distinct concepts.
- Distinguish design knowledge, design-generation tools, and full-app abstractions.
- Default to one Claude track or one Codex track; teach the shared agent concepts once.
- For non-technical learners, explain request/response, data flow, state, errors, and boundaries with diagrams or plain language before code.

## Output Contract

At minimum, return:

- course purpose, audience, prerequisites, duration, and outcomes;
- ordered modules with prerequisites and capstone links;
- lesson, lab, and assessment specifications;
- a prerequisite graph and coherence review;
- technology decisions with freshness dates, alternatives, and risks;
- explicit assumptions, unresolved risks, and recommended next research.

Read only the supporting reference needed for the current output. Templates are output contracts, not mandatory prose to copy verbatim.

## Versioning

Put `CURRICULUM_VERSION` in the course workspace. Update `DECISIONS.md` when a tool, sequence, prerequisite, or assessment strategy changes. Reverify radar entries after the configured review interval or when a user questions freshness.

## Trigger Examples

"Turn these topics into a course", "What should students learn before RAG?", "Should I teach Stitch or Lovable?", "Create a lesson plan", and "Review this curriculum" are in scope.
