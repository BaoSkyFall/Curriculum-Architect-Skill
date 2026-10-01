# Buổi 12 — Tích hợp, debug, bảo mật và demo cuối khóa

Thời lượng: 90 phút
Điều kiện tiên quyết: tất cả buổi trước
Sản phẩm: một ứng dụng nền tảng hoàn chỉnh do nhóm tự chọn

## Quy trình cuối khóa

```text
nguồn dữ liệu → ingestion → database → business rules
                                      ↓
user action → frontend → backend → retrieval/LLM → response
```

## Ngữ cảnh được chọn

Mỗi nhóm chọn một ứng dụng: danh sách việc, đặt lịch, thư viện tài liệu, hỏi đáp nội bộ hoặc một ý tưởng tương đương. Domain chỉ là vỏ minh họa; các ranh giới và bằng chứng kiểm chứng mới là tiêu chí chính.

## Tiến trình

- 0–15: smoke test theo checklist nghiệm thu.
- 15–35: mỗi nhóm chạy một kịch bản lỗi.
- 35–70: mỗi nhóm demo cuối khóa 5 phút.
- 70–85: đánh giá chéo theo rubric.
- 85–90: phản hồi và bước tiếp theo.

## Demo bắt buộc

Cho thấy một luồng hoàn chỉnh từ thao tác người dùng đến response, một trạng thái lỗi, một record có thể truy vết, một kiểm thử retrieval hoặc rule, và một giới hạn đã biết.

## Đánh giá

25% giải thích kiến trúc/luồng dữ liệu; 25% luồng hoạt động; 20% bằng chứng và kiểm thử; 15% debug/bảo mật; 15% phản hồi về tool và quyết định thiết kế.

## Kiểm tra bảo mật tối thiểu

Không commit secrets; API key chỉ ở backend; dữ liệu demo không chứa PII thật; có fallback khi LLM/retrieval fail; không biến output xác suất thành quyết định tự động không giám sát.

## Phiếu kết thúc

Học viên trả lời: “Nếu framework UI, runtime agent hoặc model provider biến mất ngày mai, phần kiến thức nào vẫn dùng được và cần thay adapter nào?”.
