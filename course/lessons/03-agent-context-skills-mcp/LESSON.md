# Buổi 3 — Agent, context, skill, MCP và kiểm chứng

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 1–2
Sản phẩm: thỏa thuận làm việc với agent

## Mục tiêu

Phân biệt model, agent, tool, skill, MCP và context; viết một task có phạm vi, ràng buộc, tiêu chí nghiệm thu và bước kiểm chứng.

## Mô hình tư duy

```text
Model + context + tools + instructions → agent action → sản phẩm → kiểm chứng
```

MCP là ranh giới để agent sử dụng tool hoặc dữ liệu; không tự làm model thông minh hơn.

## Tiến trình

- 0–20: lập bản đồ khái niệm bằng một task sửa ứng dụng ghi chú.
- 20–40: demo agent đọc repo, sửa một tệp và chạy bước kiểm tra.
- 40–55: demo quyền truy cập và một tình huống tool thất bại.
- 55–80: lab viết và chạy task có phạm vi rõ.
- 80–90: rà soát output trước khi chấp nhận.

## Bài thực hành

Task mẫu: “Thêm mock `GET /notes/:id`; không đổi schema; xử lý trường hợp không tìm thấy; chạy bước kiểm tra; báo các tệp đã đổi.”

Học viên phải ghi rõ context, phạm vi được sửa, điều không được sửa, output mong đợi và bằng chứng hoàn thành.

## Đánh giá

Đạt khi học viên chỉ ra được agent đã đọc gì, sửa gì, bước kiểm tra nào chứng minh kết quả và điều gì chưa được kiểm tra.

## Bài tập về nhà

Viết lại một yêu cầu mơ hồ thành task có input, output và tiêu chí nghiệm thu rõ ràng.
