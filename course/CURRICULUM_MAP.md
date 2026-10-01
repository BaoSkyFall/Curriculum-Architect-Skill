# Curriculum Map

| Buổi | Module | Prerequisites | Artifact trong buổi | Link tới capstone |
|---:|---|---|---|---|
| 1 | Software mental model | Không | System map của ICP chatbot | Kiến trúc tổng thể |
| 2 | FE/BE/API/DB | 1 | Request/response map + UI wireframe | Boundary của app |
| 3 | Agent, skills, MCP | 1 | Agent working agreement + verified task | Cách dùng agent an toàn |
| 4 | Multi-agent orchestration | 3 | Task decomposition + handoff log | Chia pipeline thành việc nhỏ |
| 5 | UI/UX và AI design | 1–2 | Design brief + screen states | Màn hình chat, score và evidence |
| 6 | Frontend vertical slice | 2, 5 | **Midterm ICP Discovery Prototype** | UI + mock API |
| 7 | Backend service | 2, 6 | `POST /companies/score` hoặc mock route | Boundary chấm điểm |
| 8 | LLM backend | 7 | LLM extraction/scoring endpoint | AI phân tích pattern |
| 9 | Database | 2, 7 | Schema + CRUD + audit fields | Lưu company/evidence/score |
| 10 | Data pipeline | 9 | Ingestion run report | CRM và enrichment flow |
| 11 | Retrieval/RAG/evaluation | 8–10 | Retrieval test set + grounded answer | Evidence và giải thích score |
| 12 | Integration/debug/demo | Tất cả | **Final ICP Chatbot** | Sản phẩm hoàn chỉnh |

## Sequence Rationale

Khóa học dạy boundary trước tool, request path trước data complexity, persistence trước pipeline và pipeline/retrieval trước RAG. Midterm khóa lại architecture trước khi thêm LLM.

## 10-Buổi Compression

Nếu chỉ có 10 buổi, gộp (3 + 4) thành một buổi agentic workflow và gộp (7 + 8) thành một buổi backend + LLM. Không gộp database với pipeline vì đó là dependency quan trọng.

## Coverage Gaps To Revisit

- Authentication, production deployment, billing và observability chưa phải outcome của khóa này.
- Vector database chuyên dụng là optional; bản đầu dùng retrieval đơn giản hoặc Postgres/pgvector nếu cohort đủ khả năng.
