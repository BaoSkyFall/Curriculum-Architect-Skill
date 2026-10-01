# Buổi 11 — Embeddings, retrieval, RAG và đánh giá

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 8–10
Sản phẩm: bộ kiểm thử retrieval + câu trả lời có căn cứ

## Mục tiêu

Hiểu embedding là biểu diễn phục vụ tìm tương đồng; phân biệt retrieval với generation; biết đo hit/miss và không nhầm câu trả lời trôi chảy với câu trả lời đúng.

## Mô hình tư duy

```text
câu hỏi → tìm record/chunk liên quan → đưa context vào prompt → model trả lời có citation
```

## Bài thực hành

Chọn một tập 10–20 ghi chú thuộc một trong các ngữ cảnh: hướng dẫn sử dụng thư viện, tài liệu sản phẩm, quy định sự kiện hoặc câu hỏi thường gặp. Viết 5 câu hỏi có evidence kỳ vọng; chạy baseline theo từ khóa rồi semantic retrieval nếu ngăn xếp hỗ trợ; so sánh kết quả.

## Rào chắn

- Không gửi toàn bộ cơ sở dữ liệu vào prompt.
- Không gọi câu trả lời là đúng chỉ vì nghe tự tin.
- Log ID của các record/chunk được truy xuất.
- Nếu không có context phù hợp, trả lời rõ là chưa đủ bằng chứng.

## Đánh giá

Đạt khi có bộ kiểm thử, ghi hit/miss và giải thích một dương tính giả hoặc âm tính giả.

## Bài tập về nhà

Viết một câu trả lời “không đủ bằng chứng” cho truy vấn không có dữ liệu liên quan.
