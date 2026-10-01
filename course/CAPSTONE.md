# Capstone: ICP Chatbot

## Problem

Xây một chatbot hỗ trợ quy trình xác định **Ideal Customer Profile** từ dữ liệu khách hàng cũ và danh sách prospect mới.

## Required Flow

```text
CRM cũ: ai đã mua / ai không mua
        ↓
bổ sung dữ liệu công ty (ngành, quy mô, địa điểm, tín hiệu)
        ↓
AI phân tích pattern và sinh feature/evidence
        ↓
scoring criteria có thể giải thích
        ↓
Tier 1 / Tier 2 / Tier 3
        ↓
test lại trên dữ liệu lịch sử
        ↓
tìm prospect mới giống Tier 1
        ↓
chatbot trả lời kèm evidence, confidence và giới hạn
```

## Minimum Product

- Upload/import CSV giả lập hoặc seed dataset.
- Hiển thị company, outcome mua/không mua, feature và evidence.
- Có scoring rubric phiên bản hóa; không để LLM tự âm thầm đổi tiêu chí.
- Có endpoint chat nhận câu hỏi và trả JSON gồm `answer`, `tier`, `score`, `evidence[]`, `confidence`, `caveats[]`.
- Có historical backtest: precision@Tier1 hoặc bảng TP/FP/FN đơn giản.
- Có prospect ranking cho danh sách mới và giải thích “vì sao tương đồng”.

## Suggested Data Contract

`companies(id, name, industry, size_band, region, source)`
`outcomes(company_id, purchased, deal_value, closed_at)`
`signals(company_id, key, value, source, observed_at)`
`scores(company_id, rubric_version, score, tier, evidence_json)`
`documents(id, company_id, text, metadata_json, embedding_ref)`

## Acceptance Evidence

1. Người học trace được một câu hỏi từ browser đến response.
2. Có ít nhất 30 company giả lập, trong đó có cả mua và không mua.
3. Pipeline có log số bản ghi raw, rejected và stored.
4. Score có evidence; câu trả lời không có evidence phải được đánh dấu thiếu dữ liệu.
5. Historical test có ít nhất một failure analysis.
6. Demo được một câu hỏi “Công ty nào giống Tier 1 và tại sao?”.
7. Người học nêu được một rủi ro privacy, một rủi ro hallucination và một giới hạn của dữ liệu.

## Out of Scope

CRM production integration, automated outbound email, guaranteed revenue prediction, autonomous sales decisions và xử lý PII thật.
