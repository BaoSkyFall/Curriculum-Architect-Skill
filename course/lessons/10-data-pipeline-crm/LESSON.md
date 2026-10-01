# Buổi 10 — Data pipeline: CRM → clean → enrich → store

Duration: 90 phút
Prerequisites: buổi 9
Artifact: ingestion run report

## Objectives

Mô tả pipeline raw/load/clean/transform/store; giữ provenance và rejected rows; không xem enrichment là sự thật tuyệt đối.

## Flow

- 0–15: inspect messy CSV.
- 15–30: demo pipeline log.
- 30–75: lab ingest + normalize + validate.
- 75–90: failure analysis.

## Lab

Đọc CSV CRM và file enrichment; chuẩn hóa tên/domain/size band; reject row thiếu ID; ghi `run_id`, counts và lý do reject; upsert vào database.

## Success criteria

Có raw count, clean count, rejected count, source, timestamp và một sample trước/sau transform.

## Assessment

Pass khi chạy lại pipeline không tạo duplicate và người học giải thích được data lineage.

## Homework

Chọn một transform có thể làm sai ICP và viết test dữ liệu cho nó.
