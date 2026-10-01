# Buổi 3 — Agent, context, skills, MCP và verification

Duration: 90 phút
Prerequisites: buổi 1–2
Artifact: agent working agreement

## Objectives

Phân biệt model, agent, tool, skill, MCP và context; viết một task có acceptance criteria.

## Mental model

```text
Model + context + tools + instructions → agent action → artifact → verification
```

MCP là boundary để agent dùng tool/data; không phải “AI thông minh hơn”.

## Flow

- 0–20: map khái niệm bằng một task tạo endpoint.
- 20–40: demo agent đọc repo, sửa một file, chạy check.
- 40–55: demo skill/MCP permission và failure.
- 55–80: lab viết và chạy task bounded.
- 80–90: review output như artifact chưa được tin.

## Lab

Task: “Thêm mock `GET /companies/:id`; không đổi schema; chạy test/check; báo file đã đổi.” Học viên phải ghi context, constraints, acceptance criteria và verification.

## Assessment

Pass khi người học chỉ ra được agent đã đọc gì, sửa gì, check nào chứng minh đúng và một điều chưa được kiểm tra.

## Homework

Viết lại một yêu cầu mơ hồ thành task bounded có input/output.
