# Buổi 4 — Multi-agent orchestration và task decomposition

Duration: 90 phút
Prerequisites: buổi 3
Artifact: decomposition board + handoff log

## Objectives

Biết khi nào một agent đủ dùng; chia feature thành task độc lập; nêu chi phí và rủi ro parallel work.

## Mental model

```text
Outcome → work packages → agent/subagent → handoff → integration → verification
```

## Flow

- 0–15: single-agent baseline.
- 15–30: phân biệt parallelizable và shared-state work.
- 30–45: demo OMX hoặc OMC theo track đã chọn.
- 45–75: lab decomposition cho ICP pipeline.
- 75–90: compare “nhiều agent” với “một agent có checklist”.

## Lab

Chia feature “import CRM và hiển thị Tier” thành 3 task: schema, ingestion, UI. Mỗi task có file ownership, input, output, dependency và verification. Chạy tối đa hai task song song nếu runtime hỗ trợ.

## Assessment

Pass khi có handoff rõ và không có hai task cùng sửa một boundary mà không thỏa thuận.

## Homework

Viết một trường hợp multi-agent sẽ làm chậm dự án và lý do.
