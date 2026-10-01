# Bản đồ điều kiện tiên quyết

```text
Mô hình tư duy phần mềm
  ├─> ranh giới frontend/backend/API/cơ sở dữ liệu
  │     ├─> HTTP + JSON + endpoint
  │     │     └─> dịch vụ backend
  │     │           └─> LLM call
  │     │                 └─> chat UI
  │     └─> schema cơ sở dữ liệu + persistence
  │           └─> pipeline ingestion + enrichment CRM
  │                 └─> clean/transform/store
  │                       └─> embeddings + retrieval
  │                             └─> RAG + evidence
  └─> agent/context/skill/MCP
        └─> phân rã task + kiểm chứng
              └─> hỗ trợ mọi bài lab, không thay thế kiến thức phần mềm
```

## Quy tắc điều kiện

- Không dạy RAG trước khi học viên đã gọi được LLM và đọc được JSON.
- Không dạy pipeline dữ liệu trước khi học viên hiểu lưu trữ bền vững và input/output.
- Không yêu cầu multi-agent nếu một task vẫn giải quyết tốt bằng một agent.
- Không đánh giá việc sinh UI nếu học viên chưa viết được trạng thái và tiêu chí nghiệm thu.
