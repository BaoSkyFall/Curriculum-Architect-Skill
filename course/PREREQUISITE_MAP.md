# Prerequisite Map

```text
Software mental model
  ├─> frontend/backend/API/database boundaries
  │     ├─> HTTP + JSON + endpoint
  │     │     └─> backend service
  │     │           └─> LLM call
  │     │                 └─> chat UI
  │     └─> database schema + persistence
  │           └─> CRM ingestion + enrichment pipeline
  │                 └─> clean/transform/store
  │                       └─> embeddings + retrieval
  │                             └─> RAG + evidence
  └─> agent/context/skill/MCP
        └─> task decomposition + verification
              └─> hỗ trợ mọi lab, không thay thế kiến thức software
```

## Gating Rules

- Không dạy RAG trước khi học viên đã gọi được LLM và đọc được JSON.
- Không dạy data pipeline trước khi học viên hiểu persistent storage và input/output.
- Không yêu cầu multi-agent nếu một task vẫn giải quyết tốt bằng một agent.
- Không đánh giá UI generation nếu học viên chưa viết được states và acceptance criteria.
