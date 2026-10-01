# Buổi 1 — Software mental model và vibe coding

Duration: 90 phút
Prerequisites: không
Artifact: system map cho ICP chatbot

## Objectives

Học viên vẽ được input, processing, storage, output và failure points; phân biệt “AI tạo code” với “mình hiểu hệ thống”.

## Mental model

```text
Người dùng → giao diện → service → dữ liệu/model → kết quả
                 ↘ lỗi / trạng thái / log ↗
```

## Flow

- 0–10: hỏi “CRM có thể nói gì về khách hàng?”
- 10–30: giải thích app như hệ thống biến input thành output.
- 30–50: demo trace một câu hỏi ICP bằng giấy.
- 50–80: lab vẽ system map và annotate boundary.
- 80–90: explain-back.

## Lab

Vẽ các block `browser`, `API`, `database`, `LLM`, `retrieval`, `data pipeline`; với mỗi block ghi input, output và một lỗi có thể xảy ra.

Success: người học trace được câu “Công ty nào giống Tier 1?” mà không dùng tên tool.

## Check / assessment

Đánh giá bằng lời giải thích 2 phút và sửa một sơ đồ cố tình thiếu database. Không chấm thuật ngữ.

## Homework

Viết 5 câu hỏi mà chatbot ICP phải trả lời và đánh dấu dữ liệu cần để trả lời mỗi câu.
