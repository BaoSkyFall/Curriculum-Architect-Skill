# Buổi 4 — Điều phối đa agent và phân rã task

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 3
Sản phẩm: bảng phân rã + log bàn giao

## Mục tiêu

Biết khi nào một agent là đủ; chia tính năng thành các phần độc lập; nhận diện dependency, shared state và chi phí phối hợp.

## Mô hình tư duy

```text
Kết quả cần đạt → gói công việc → agent/subagent → bàn giao → tích hợp → kiểm chứng
```

## Tiến trình

- 0–15: thiết lập mốc chuẩn bằng một agent.
- 15–30: phân biệt công việc có thể chạy song song và công việc dùng chung trạng thái.
- 30–45: demo runtime điều phối đã chọn.
- 45–75: lab phân rã một tính năng nhập sự kiện từ CSV.
- 75–90: so sánh nhiều agent với một agent có checklist.

## Bài thực hành

Chia tính năng “nhập danh sách sự kiện và hiển thị lịch” thành ba task: schema, import và UI. Mỗi task phải có phạm vi sở hữu tệp, input, output, dependency và bước kiểm chứng.

Chỉ chạy song song khi hai task không cùng sửa một ranh giới hoặc phụ thuộc kết quả của nhau.

## Đánh giá

Đạt khi có bàn giao rõ ràng, không trùng quyền sở hữu và có bước tích hợp cuối.

## Bài tập về nhà

Viết một trường hợp đa agent làm chậm công việc và giải thích vì sao dùng một agent sẽ tốt hơn.
