# Buổi 9 — Cơ sở dữ liệu và schema cho ICP

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 2, 7
Sản phẩm: schema + CRUD + trường audit

## Mục tiêu

Hiểu table/row/column/ID/relationship/query; lưu được company, outcome, signal, score và evidence.

## Schema gợi ý

`companies`, `outcomes`, `signals`, `scores`, `documents`; mọi enrichment có `source` và `observed_at`.

## Bài thực hành

Nạp seed 30 company giả lập; viết query/filter “đã mua”, “ngành X”, “Tier 1”; hiển thị lịch sử score theo `rubric_version`.

## Lỗi thường gặp

Ghi đè score cũ; trộn raw và cleaned data; không lưu nguồn của signal.

## Đánh giá

Đạt khi schema trả lời được “score này dựa trên evidence nào và dữ liệu được quan sát lúc nào?”.

## Bài tập về nhà

Thêm một field có thể gây bias và ghi cách kiểm tra/loại bỏ nó.
