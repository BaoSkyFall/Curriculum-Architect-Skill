# Buổi 11 — Embeddings, retrieval, RAG và evaluation

Duration: 90 phút
Prerequisites: buổi 8–10
Artifact: retrieval test set + grounded answer

## Objectives

Hiểu embedding là biểu diễn để tìm tương đồng; phân biệt retrieval với generation; tạo câu trả lời có evidence và biết đo lỗi.

## Mental model

```text
câu hỏi → tìm record/chunk liên quan → đưa context vào prompt → LLM trả lời có citation/evidence
```

## Lab

Tạo 10–20 company notes/chunks; viết 5 câu hỏi có expected evidence; chạy keyword baseline rồi semantic retrieval nếu stack hỗ trợ; so sánh kết quả.

## Guardrails

Không gửi toàn bộ database vào prompt; không gọi câu trả lời đúng chỉ vì nghe tự tin; log retrieved IDs.

## Assessment

Pass khi có test set, ghi hit/miss và giải thích một false positive hoặc false negative.

## Homework

Viết một câu trả lời “insufficient evidence” cho truy vấn không có dữ liệu.
