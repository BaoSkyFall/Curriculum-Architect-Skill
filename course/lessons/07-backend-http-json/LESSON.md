# Buổi 7 — Dịch vụ backend, HTTP, JSON và xử lý lỗi

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 2, 6
Sản phẩm: endpoint cho một thao tác nghiệp vụ nhỏ

## Mục tiêu

Tạo route nhỏ, kiểm tra input, trả status/error có nghĩa, giữ secret ở server và không để logic backend trôi vào giao diện.

## Tiến trình

- 0–20: đào sâu request/response.
- 20–40: demo route Node API và `.env`.
- 40–75: lab nối prototype giữa kỳ vào backend.
- 75–90: cố tình gửi input không hợp lệ và debug.

## Bài thực hành

Chọn một route phù hợp với prototype:

- `POST /tasks` nhận `{title, due_at}`.
- `POST /appointments` nhận `{start_at, duration_minutes}`.
- `POST /documents/search` nhận `{query, limit}`.

Trả JSON có cấu trúc; thêm lỗi 400 cho input thiếu hoặc sai kiểu và 404 cho tài nguyên không tồn tại.

## Đánh giá

Đạt khi route có luồng thành công, kiểm tra hợp lệ, JSON lỗi dễ dự đoán và không làm lộ key.

## Bài tập về nhà

Vẽ contract trước khi thêm LLM: field bắt buộc, field tùy chọn, mã lỗi và trạng thái giao diện tương ứng.
