# Buổi 1 — Mô hình tư duy phần mềm và vibe coding

Thời lượng: 90 phút
Điều kiện tiên quyết: không
Sản phẩm: sơ đồ hệ thống cho ICP chatbot

## Mục tiêu

Học viên vẽ được input, processing, storage, output và các điểm lỗi; phân biệt “AI tạo code” với “mình hiểu hệ thống”.

## Mô hình tư duy

```text
Người dùng → giao diện → service → dữ liệu/model → kết quả
                 ↘ lỗi / trạng thái / log ↗
```

## Tiến trình

- 0–10: hỏi “CRM có thể nói gì về khách hàng?”
- 10–30: giải thích app như hệ thống biến input thành output.
- 30–50: demo lần theo một câu hỏi ICP bằng giấy.
- 50–80: lab vẽ sơ đồ hệ thống và chú thích ranh giới.
- 80–90: học viên giải thích lại.

## Bài thực hành

Vẽ các block `browser`, `API`, `database`, `LLM`, `retrieval`, `data pipeline`; với mỗi block ghi input, output và một lỗi có thể xảy ra.

Tiêu chí đạt: người học lần theo được câu “Công ty nào giống Tier 1?” mà không dùng tên tool.

## Kiểm tra / đánh giá

Đánh giá bằng lời giải thích 2 phút và sửa một sơ đồ cố tình thiếu cơ sở dữ liệu. Không chấm thuật ngữ.

## Bài tập về nhà

Viết 5 câu hỏi mà chatbot ICP phải trả lời và đánh dấu dữ liệu cần để trả lời mỗi câu.
