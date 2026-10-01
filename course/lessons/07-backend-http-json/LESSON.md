# Buổi 7 — Backend service, HTTP, JSON và error handling

Duration: 90 phút
Prerequisites: buổi 2, 6
Artifact: endpoint `/companies/score` hoặc mock scoring route

## Objectives

Học viên tạo route nhỏ, đọc JSON, validate input, trả status/error có nghĩa và giữ secret ở server.

## Flow

- 0–20: request/response deep dive.
- 20–40: demo Node API route và `.env`.
- 40–75: lab nối frontend midterm vào backend.
- 75–90: intentionally break invalid input và debug.

## Lab

Implement `POST /companies/score` nhận `{company_id, rubric_version}` và trả `{score, tier, evidence}` từ rule giả lập. Thêm lỗi 400 cho input thiếu và 404 cho company không tồn tại.

## Assessment

Pass khi route có happy path, validation, predictable error JSON và không expose key.

## Homework

Vẽ contract trước khi thêm LLM: fields required, optional và error states.
