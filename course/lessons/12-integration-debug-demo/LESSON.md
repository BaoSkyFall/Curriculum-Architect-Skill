# Buổi 12 — Tích hợp, debug, bảo mật và demo cuối khóa

Thời lượng: 90 phút
Điều kiện tiên quyết: tất cả buổi trước
Sản phẩm: **Final ICP Chatbot**

## Quy trình cuối khóa

```text
CRM → ingestion → database → signals/evidence → scoring rubric
                                      ↓
user question → frontend → backend → retrieval/LLM → answer + tier + evidence
```

## Tiến trình

- 0–15: smoke test theo checklist nghiệm thu.
- 15–35: mỗi nhóm chạy một kịch bản lỗi.
- 35–70: mỗi nhóm demo cuối khóa 5 phút.
- 70–85: đánh giá chéo theo rubric.
- 85–90: phản hồi và bước tiếp theo.

## Demo bắt buộc

Import dataset, hỏi company giống Tier 1, xem evidence, xem score/tier, xem backtest lịch sử và chỉ ra một giới hạn.

## Đánh giá

25% giải thích kiến trúc/luồng dữ liệu; 25% luồng hoạt động; 20% evidence và backtest; 15% debug/bảo mật; 15% phản hồi về tool/quyết định.

## Kiểm tra bảo mật tối thiểu

Không commit secrets; API key chỉ ở backend; dữ liệu demo đã ẩn danh; có fallback khi LLM/retrieval fail; không biến score thành quyết định tự động không giám sát.

## Phiếu kết thúc

Học viên trả lời: “Nếu Stitch, OMX hoặc model provider biến mất ngày mai, phần kiến thức nào của em vẫn dùng được và cần thay adapter nào?”.
