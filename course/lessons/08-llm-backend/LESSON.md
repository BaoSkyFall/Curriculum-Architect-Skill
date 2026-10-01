# Buổi 8 — Tích hợp LLM vào backend

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 7
Sản phẩm: endpoint trả output có cấu trúc và có fallback

## Mục tiêu

Dùng system/user messages, context, structured output và streaming ở mức đủ dùng; biết timeout, retry, giới hạn dữ liệu và ranh giới hallucination.

## Mô hình tư duy

```text
Backend chọn context → gửi messages → model trả output → backend kiểm tra → frontend hiển thị
```

## Bài thực hành

Chọn một tác vụ:

- Tóm tắt ghi chú cuộc họp.
- Trích xuất trường từ mô tả sự kiện.
- Phân loại yêu cầu hỗ trợ.

Yêu cầu model trả JSON gồm `label`, `summary`, `items[]`, `missing_data[]` và `confidence` phù hợp với tác vụ. Kiểm tra schema; nếu model lỗi hoặc trả dữ liệu thiếu, trả fallback và ghi log.

## Rào chắn

LLM chỉ đề xuất hoặc biến đổi dữ liệu theo contract. Các quy tắc an toàn, quyền truy cập, ngưỡng và quyết định cuối phải nằm ở code hoặc chính sách có thể kiểm tra.

## Đánh giá

Đạt khi học viên chỉ ra phần tất định, phần xác suất, dữ liệu nào được gửi đi và cách xử lý output không hợp lệ.

## Bài tập về nhà

Viết một prompt có ví dụ tốt/xấu và một test case thiếu dữ liệu hoặc chứa thông tin nhạy cảm.
