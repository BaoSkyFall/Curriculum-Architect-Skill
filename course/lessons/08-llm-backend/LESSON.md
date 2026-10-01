# Buổi 8 — Nhúng LLM vào backend

Duration: 90 phút
Prerequisites: buổi 7
Artifact: structured extraction/scoring explanation endpoint

## Objectives

Dùng system/user messages, context, structured output và streaming ở mức đủ dùng; biết timeout, retry và hallucination boundary.

## Mental model

```text
Backend chọn context → gửi messages → model trả output → backend validate → frontend render
```

## Lab

Tạo route nhận company profile + evidence, yêu cầu model trả JSON gồm `signals[]`, `summary`, `missing_data[]`, `confidence`. Validate schema; nếu model lỗi thì trả fallback và log.

## Guardrail

LLM không tự đổi rubric hoặc tier threshold. Nó chỉ trích xuất/giải thích; rule version và score policy nằm trong code/data.

## Assessment

Pass khi người học chỉ ra phần deterministic, phần probabilistic và cách xử lý output không hợp lệ.

## Homework

Viết một prompt có ví dụ tốt/xấu và một test case thiếu dữ liệu.
