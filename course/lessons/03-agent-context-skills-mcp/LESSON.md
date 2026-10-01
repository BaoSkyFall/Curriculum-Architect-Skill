# Buổi 3 — Agent, context, skill, MCP và kiểm chứng

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 1–2
Sản phẩm: thỏa thuận làm việc với agent

## Mục tiêu

Phân biệt model, agent, tool, skill, MCP và context; viết một task có tiêu chí nghiệm thu.

## Mô hình tư duy

```text
Model + context + tools + instructions → agent action → artifact → verification
```

MCP là boundary để agent dùng tool/data; không phải “AI thông minh hơn”.

## Tiến trình

- 0–20: lập bản đồ khái niệm bằng một task tạo endpoint.
- 20–40: demo agent đọc repo, sửa một tệp và chạy bước kiểm tra.
- 40–55: demo quyền skill/MCP và tình huống lỗi.
- 55–80: lab viết và chạy task có phạm vi rõ.
- 80–90: rà soát output như một sản phẩm chưa thể mặc định tin cậy.

## Bài thực hành

Task: “Thêm mock `GET /companies/:id`; không đổi schema; chạy test/check; báo các tệp đã đổi.” Học viên phải ghi context, ràng buộc, tiêu chí nghiệm thu và bước kiểm chứng.

## Đánh giá

Đạt khi người học chỉ ra được agent đã đọc gì, sửa gì, bước kiểm tra nào chứng minh đúng và một điều chưa được kiểm tra.

## Bài tập về nhà

Viết lại một yêu cầu mơ hồ thành task có phạm vi, input và output rõ ràng.
