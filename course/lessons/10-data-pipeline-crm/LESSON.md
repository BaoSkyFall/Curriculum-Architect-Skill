# Buổi 10 — Pipeline dữ liệu: CRM → làm sạch → enrichment → lưu trữ

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 9
Sản phẩm: báo cáo một lần chạy ingestion

## Mục tiêu

Mô tả pipeline raw/load/clean/transform/store; giữ provenance và các dòng bị loại; không xem enrichment là sự thật tuyệt đối.

## Tiến trình

- 0–15: kiểm tra CSV lộn xộn.
- 15–30: demo log pipeline.
- 30–75: lab ingest + chuẩn hóa + kiểm tra hợp lệ.
- 75–90: phân tích lỗi.

## Bài thực hành

Đọc CSV CRM và file enrichment; chuẩn hóa tên/domain/size band; loại dòng thiếu ID; ghi `run_id`, số lượng và lý do loại; upsert vào cơ sở dữ liệu.

## Tiêu chí đạt

Có số lượng raw, số lượng clean, số lượng bị loại, source, timestamp và một mẫu trước/sau transform.

## Đánh giá

Đạt khi chạy lại pipeline không tạo bản ghi trùng và người học giải thích được nguồn gốc dữ liệu.

## Bài tập về nhà

Chọn một transform có thể làm sai ICP và viết test dữ liệu cho nó.
