# Research: Backend Stack

Verified: 2026-10-01

## Recommendation

Use one language end-to-end for the beginner path: React/Vite for the browser, a small Node.js HTTP API for the backend, SQLite for local persistence, and an optional Postgres/Supabase deployment later.

This is a teaching choice, not a claim that it is the only production stack. The important boundary is:

```text
browser → HTTP JSON endpoint → server logic → storage/LLM → JSON response
```

## Why this path

- One language reduces cognitive switching.
- A separate API keeps the FE/BE boundary visible.
- SQLite makes the first persistence lab cheap and local.
- Postgres/Supabase can be introduced as a deployment option without changing the schema mental model.

## Deliberate omissions

No auth, queues, microservices, ORM deep dive or production observability in the core course. Add them only in an advanced follow-up.
