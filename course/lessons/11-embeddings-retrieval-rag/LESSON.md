# Buổi 11 — Embeddings, retrieval, RAG và đánh giá

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 8–10
Sản phẩm: bộ kiểm thử retrieval + câu trả lời có căn cứ

## Mục tiêu

Hiểu embedding là biểu diễn để tìm tương đồng; phân biệt retrieval với generation; tạo câu trả lời có evidence và biết đo lỗi.

## Mô hình tư duy

```text
câu hỏi → tìm record/chunk liên quan → đưa context vào prompt → LLM trả lời có citation/evidence
```

## Bài thực hành

Tạo 10–20 ghi chú/chunk về company; viết 5 câu hỏi có evidence kỳ vọng; chạy baseline theo từ khóa rồi semantic retrieval nếu ngăn xếp hỗ trợ; so sánh kết quả.

## Rào chắn

Không gửi toàn bộ database vào prompt; không gọi câu trả lời đúng chỉ vì nghe tự tin; log retrieved IDs.

## Đánh giá

Đạt khi có bộ kiểm thử, ghi hit/miss và giải thích một dương tính giả hoặc âm tính giả.

## Bài tập về nhà

Viết một câu trả lời “không đủ bằng chứng” cho truy vấn không có dữ liệu.
