# Curriculum Map

| Order | Module | Prerequisites | Learner outcome | Capstone artifact |
|---|---|---|---|---|
| 1 | Software mental model | None | Trace input, processing, storage, and output | Architecture sketch |
| 2 | Frontend, backend, API, database | Module 1 | Explain application boundaries | Static interface and data-flow map |
| 3 | AI coding agents, skills, and MCP | Module 1 | Delegate and verify bounded changes | Agent working agreement |
| 4 | Backend and LLM calls | Modules 2-3 | Send a message and receive a model response | `/chat` endpoint |
| 5 | Persistence and chat history | Module 4 | Store and retrieve conversations | Saved messages |
| 6 | Data ingestion and retrieval | Modules 2, 4-5 | Prepare and retrieve document context | Searchable document set |
| 7 | RAG and integration | Module 6 | Ground answers in retrieved context | Working knowledge chat |
| 8 | Debugging and capstone | All prior modules | Explain, test, and improve the system | Demonstrated final application |

## Sequence Rationale

The course introduces system boundaries before tools, then builds one request path before adding persistence and retrieval.
