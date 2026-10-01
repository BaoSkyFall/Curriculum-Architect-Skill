# Buổi 10 — Pipeline dữ liệu: nạp, làm sạch, biến đổi và lưu trữ

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 9
Sản phẩm: báo cáo một lần chạy pipeline

## Mục tiêu

Mô tả pipeline `raw → load → clean → transform → store`; giữ provenance, dòng bị loại và khả năng chạy lại an toàn.

## Tiến trình

- 0–15: kiểm tra một CSV lộn xộn từ danh sách sách, sự kiện hoặc yêu cầu hỗ trợ.
- 15–30: demo log pipeline.
- 30–75: lab nạp, chuẩn hóa và kiểm tra hợp lệ.
- 75–90: phân tích lỗi và dữ liệu bị thay đổi ngoài dự kiến.

## Bài thực hành

Chọn một dataset nhỏ, chuẩn hóa tên cột và giá trị, loại dòng thiếu khóa chính, ghi `run_id`, số lượng từng bước và lý do loại. Upsert vào cơ sở dữ liệu mà không tạo bản ghi trùng khi chạy lại.

## Tiêu chí đạt

Có số lượng raw, clean, rejected và stored; có source, timestamp; có một mẫu trước/sau transform; có log để lần theo một record.

## Đánh giá

Đạt khi học viên giải thích được nguồn gốc của một record và chứng minh lần chạy thứ hai không nhân đôi dữ liệu.

## Bài tập về nhà

Chọn một transform có thể làm mất hoặc đổi nghĩa dữ liệu và viết một kiểm tra nhỏ cho nó.
