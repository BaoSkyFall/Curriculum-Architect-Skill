# Buổi 4 — Điều phối đa agent và phân rã task

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 3
Sản phẩm: bảng phân rã + log bàn giao

## Mục tiêu

Biết khi nào một agent là đủ; chia tính năng thành task độc lập; nêu chi phí và rủi ro của công việc song song.

## Mô hình tư duy

```text
Outcome → work packages → agent/subagent → handoff → integration → verification
```

## Tiến trình

- 0–15: mốc chuẩn với một agent.
- 15–30: phân biệt công việc có thể chạy song song và công việc dùng chung trạng thái.
- 30–45: demo OMX hoặc OMC theo track đã chọn.
- 45–75: lab phân rã pipeline ICP.
- 75–90: so sánh “nhiều agent” với “một agent có checklist”.

## Bài thực hành

Chia tính năng “import CRM và hiển thị Tier” thành 3 task: schema, ingestion, UI. Mỗi task có phạm vi sở hữu tệp, input, output, dependency và bước kiểm chứng. Chạy tối đa hai task song song nếu runtime hỗ trợ.

## Đánh giá

Đạt khi có bàn giao rõ ràng và không có hai task cùng sửa một ranh giới mà không thỏa thuận.

## Bài tập về nhà

Viết một trường hợp multi-agent sẽ làm chậm dự án và lý do.
