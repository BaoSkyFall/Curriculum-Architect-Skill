# Buổi 9 — Cơ sở dữ liệu và schema

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 2, 7
Sản phẩm: schema + CRUD + trường audit

## Mục tiêu

Hiểu table, row, column, ID, relationship và query; biết chọn dữ liệu nào cần lưu, dữ liệu nào chỉ là trạng thái tạm thời.

## Schema gợi ý

Chọn một ngữ cảnh và mô hình hóa các bảng phù hợp:

- Ứng dụng đặt lịch: `users`, `appointments`, `reminders`.
- Thư viện tài liệu: `documents`, `tags`, `document_tags`, `revisions`.
- Ứng dụng danh sách việc: `lists`, `tasks`, `task_events`.

Record thay đổi quan trọng nên có `created_at`, `updated_at`, `source` hoặc trường audit tương đương.

## Bài thực hành

Nạp dữ liệu giả lập, viết query cho ít nhất ba nhu cầu của ứng dụng và hiển thị lịch sử thay đổi của một record. Ghi rõ khóa chính, khóa liên kết và quy tắc dữ liệu bắt buộc.

## Lỗi thường gặp

- Ghi đè lịch sử khi chỉ cần tạo phiên bản mới.
- Trộn dữ liệu thô với dữ liệu đã chuẩn hóa.
- Không lưu nguồn hoặc thời điểm quan sát.
- Dùng một bảng khổng lồ để tránh thiết kế quan hệ.

## Đánh giá

Đạt khi schema trả lời được record này là gì, liên quan đến record nào, thay đổi lúc nào và có thể truy vấn ra sao.

## Bài tập về nhà

Thêm một field có thể gây thiên lệch hoặc rủi ro riêng tư; ghi cách giảm thiểu hoặc loại bỏ field đó.
