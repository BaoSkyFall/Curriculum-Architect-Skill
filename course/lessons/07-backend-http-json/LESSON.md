# Buổi 7 — Dịch vụ backend, HTTP, JSON và xử lý lỗi

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 2, 6
Sản phẩm: endpoint `/companies/score` hoặc route chấm điểm giả lập

## Mục tiêu

Học viên tạo route nhỏ, đọc JSON, kiểm tra input, trả status/error có nghĩa và giữ secret ở server.

## Tiến trình

- 0–20: đào sâu request/response.
- 20–40: demo route Node API và `.env`.
- 40–75: lab nối frontend giữa kỳ vào backend.
- 75–90: cố tình gửi input không hợp lệ và debug.

## Bài thực hành

Triển khai `POST /companies/score` nhận `{company_id, rubric_version}` và trả `{score, tier, evidence}` từ rule giả lập. Thêm lỗi 400 cho input thiếu và 404 cho company không tồn tại.

## Đánh giá

Đạt khi route có luồng thành công, kiểm tra hợp lệ, JSON lỗi dễ dự đoán và không làm lộ key.

## Bài tập về nhà

Vẽ contract trước khi thêm LLM: field bắt buộc, field tùy chọn và trạng thái lỗi.
