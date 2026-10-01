# Coherence Review — v0.1

## Result

Status: teachable with controlled setup
Critical issues: 0
Warnings: 4
Suggestions: 5

## Checks

- Goal alignment: pass — mọi module tạo artifact cho ICP chatbot.
- Prerequisite integrity: pass — LLM trước RAG, persistence trước pipeline.
- Difficulty progression: pass with warning — buổi 10–11 nặng, cần dùng starter repo.
- Concept coverage: pass — FE/BE/API/DB/agent/MCP/LLM/pipeline/retrieval đều có.
- Tool longevity: pass with warning — tool được đặt dưới concept và có alternatives.
- Project integration: pass — midterm là vertical slice, final là mở rộng liên tục.
- Assessment quality: pass — chấm data flow, evidence, debug và trade-off.
- Non-tech accessibility: pass with warning — cần chuẩn bị glossary, diagrams và paired lab.

## Warnings / Mitigations

1. Setup account/API có thể chiếm thời gian → chuẩn bị starter repo, `.env.example`, dataset và fallback mock.
2. Embedding/vector terminology nặng → dạy retrieval trên bảng nhỏ trước, chỉ sau đó dùng vector store.
3. Dữ liệu ICP dễ chứa PII → chỉ dùng dữ liệu giả lập/ẩn danh và có privacy checklist.
4. OMC/OMX/UI tools có thể đổi CLI → kiểm tra `TECH_RADAR.md` trước cohort; không chấm theo UI của tool.

## Next Review

Reverify technology entries trước mỗi cohort hoặc khi có major release/deprecation.
