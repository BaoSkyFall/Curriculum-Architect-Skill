# Teacher Guide

## Before the cohort

- Verify one agent track, model provider, Node.js version and accounts.
- Prepare starter repo with `frontend/`, `backend/`, `data/`, `.env.example`, seed CSV and mock mode.
- Prepare 30–50 synthetic company records with purchased/non-purchased outcomes.
- Prepare a printed glossary and one architecture diagram.
- Test the fallback path without Stitch, without orchestration plugin and without live LLM.

## Facilitation rules

- Never let setup consume the whole 90 minutes; pair students and provide a known-good checkpoint.
- Ask “what went in, what came out, and where can it fail?” after every demo.
- Students explain one generated change before accepting it.
- Keep one stable domain example: company → outcome → signals → score → tier → evidence.

## Common recovery moves

- API key failure: switch to mock provider.
- Agent/plugin failure: use native agent plus handoff checklist.
- Retrieval failure: show keyword baseline and inspect chunks before changing models.
- UI tool unavailable: use supplied PNG/HTML and continue with states/spec.
