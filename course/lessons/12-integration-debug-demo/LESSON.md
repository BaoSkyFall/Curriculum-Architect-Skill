# Buổi 12 — Tích hợp, debugging, security và demo final

Duration: 90 phút
Prerequisites: tất cả buổi trước
Artifact: **Final ICP Chatbot**

## Final flow

```text
CRM → ingestion → database → signals/evidence → scoring rubric
                                      ↓
user question → frontend → backend → retrieval/LLM → answer + tier + evidence
```

## Flow

- 0–15: smoke test theo acceptance checklist.
- 15–35: mỗi nhóm chạy một failure scenario.
- 35–70: demo final 5 phút/nhóm.
- 70–85: peer review theo rubric.
- 85–90: reflection và next steps.

## Required demo

Import dataset, hỏi company giống Tier 1, xem evidence, xem score/tier, xem historical backtest và chỉ ra một giới hạn.

## Assessment

25% architecture/data-flow explanation; 25% working flow; 20% evidence and backtest; 15% debugging/security; 15% tool/decision reflection.

## Minimum security check

Không commit secrets; API key chỉ ở backend; dữ liệu demo đã ẩn danh; có fallback khi LLM/retrieval fail; không biến score thành quyết định tự động không giám sát.

## Exit ticket

Học viên trả lời: “Nếu Stitch, OMX hoặc model provider biến mất ngày mai, phần kiến thức nào của em vẫn dùng được và cần thay adapter nào?”.
