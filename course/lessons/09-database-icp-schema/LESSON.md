# Buổi 9 — Database và schema cho ICP

Duration: 90 phút
Prerequisites: buổi 2, 7
Artifact: schema + CRUD + audit fields

## Objectives

Hiểu table/row/column/ID/relationship/query; lưu được company, outcome, signal, score và evidence.

## Suggested schema

`companies`, `outcomes`, `signals`, `scores`, `documents`; mọi enrichment có `source` và `observed_at`.

## Lab

Seed 30 company giả lập; viết query/filter “đã mua”, “ngành X”, “Tier 1”; hiển thị score history theo `rubric_version`.

## Common mistakes

Ghi đè score cũ; trộn raw và cleaned data; không lưu nguồn của signal.

## Assessment

Pass khi schema trả lời được “score này dựa trên evidence nào và dữ liệu được quan sát lúc nào?”.

## Homework

Thêm một field có thể gây bias và ghi cách kiểm tra/loại bỏ nó.
