# Buổi 8 — Tích hợp LLM vào backend

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 7
Sản phẩm: endpoint trích xuất có cấu trúc/giải thích chấm điểm

## Mục tiêu

Dùng system/user messages, context, structured output và streaming ở mức đủ dùng; biết timeout, retry và ranh giới hallucination.

## Mô hình tư duy

```text
Backend chọn context → gửi messages → model trả output → backend validate → frontend render
```

## Bài thực hành

Tạo route nhận hồ sơ company + evidence, yêu cầu model trả JSON gồm `signals[]`, `summary`, `missing_data[]`, `confidence`. Kiểm tra schema; nếu model lỗi thì trả fallback và ghi log.

## Rào chắn

LLM không tự đổi rubric hoặc tier threshold. Nó chỉ trích xuất/giải thích; rule version và score policy nằm trong code/data.

## Đánh giá

Đạt khi người học chỉ ra phần tất định, phần xác suất và cách xử lý output không hợp lệ.

## Bài tập về nhà

Viết một prompt có ví dụ tốt/xấu và một test case thiếu dữ liệu.
