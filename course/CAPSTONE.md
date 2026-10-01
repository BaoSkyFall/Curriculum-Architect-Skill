# Capstone: ICP Chatbot

## Bài toán

Xây một chatbot hỗ trợ quy trình xác định **Ideal Customer Profile** từ dữ liệu khách hàng cũ và danh sách prospect mới.

## Quy trình bắt buộc

```text
CRM cũ: ai đã mua / ai không mua
        ↓
bổ sung dữ liệu công ty (ngành, quy mô, địa điểm, tín hiệu)
        ↓
AI phân tích mẫu hình và sinh feature/evidence
        ↓
scoring criteria có thể giải thích
        ↓
Tier 1 / Tier 2 / Tier 3
        ↓
kiểm thử lại trên dữ liệu lịch sử
        ↓
tìm prospect mới giống Tier 1
        ↓
chatbot trả lời kèm evidence, độ tin cậy và giới hạn
```

## Sản phẩm tối thiểu

- Tải lên/import CSV giả lập hoặc nạp dataset seed.
- Hiển thị company, outcome mua/không mua, feature và evidence.
- Có scoring rubric phiên bản hóa; không để LLM tự âm thầm đổi tiêu chí.
- Có endpoint chat nhận câu hỏi và trả JSON gồm `answer`, `tier`, `score`, `evidence[]`, `confidence`, `caveats[]`.
- Có backtest lịch sử: precision@Tier1 hoặc bảng TP/FP/FN đơn giản.
- Có xếp hạng prospect cho danh sách mới và giải thích “vì sao tương đồng”.

## Hợp đồng dữ liệu gợi ý

`companies(id, name, industry, size_band, region, source)`
`outcomes(company_id, purchased, deal_value, closed_at)`
`signals(company_id, key, value, source, observed_at)`
`scores(company_id, rubric_version, score, tier, evidence_json)`
`documents(id, company_id, text, metadata_json, embedding_ref)`

## Bằng chứng nghiệm thu

1. Người học lần theo được một câu hỏi từ trình duyệt đến response.
2. Có ít nhất 30 company giả lập, trong đó có cả mua và không mua.
3. Pipeline có log số bản ghi raw, rejected và stored.
4. Score có evidence; câu trả lời không có evidence phải được đánh dấu thiếu dữ liệu.
5. Bài kiểm thử lịch sử có ít nhất một phân tích lỗi.
6. Demo được một câu hỏi “Công ty nào giống Tier 1 và tại sao?”.
7. Người học nêu được một rủi ro riêng tư, một rủi ro hallucination và một giới hạn của dữ liệu.

## Ngoài phạm vi

Tích hợp CRM production, email outbound tự động, dự đoán doanh thu được đảm bảo, quyết định bán hàng tự động và xử lý PII thật.
