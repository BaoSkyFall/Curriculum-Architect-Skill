# Research: Data and Retrieval Stack

Verified: 2026-10-01

## Learning progression

1. Start with CSV rows and a visible table.
2. Persist company/outcome/signal records in SQLite.
3. Add ingestion logs and rejected-row reasons.
4. Add enrichment as a separate source with provenance.
5. Teach chunking and metadata on a small document set.
6. Compare keyword filtering with embeddings/retrieval.
7. Add RAG only after the retrieval test set exists.

## Recommendation

Use SQLite for the first labs and either a simple local retrieval implementation or Postgres/pgvector/Supabase for the integrated capstone. A managed vector database is optional; it is not required to understand RAG.

## Evaluation

Every retrieval demo has labeled questions and expected evidence. Track whether the answer cites a relevant record, not only whether it sounds fluent.

## Safety

Use synthetic or anonymized CRM data, record source and timestamp for enrichment, and show students how to delete or redact a record before sending context to an LLM.
