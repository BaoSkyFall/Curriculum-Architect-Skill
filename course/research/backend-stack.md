# Nghiên cứu: Ngăn xếp backend

Xác minh: 2026-10-01

## Khuyến nghị

Dùng một ngôn ngữ xuyên suốt cho lộ trình nhập môn: React/Vite cho trình duyệt, một HTTP API Node.js nhỏ cho backend, SQLite để lưu trữ cục bộ và tùy chọn triển khai Postgres/Supabase về sau.

Đây là lựa chọn phục vụ giảng dạy, không phải khẳng định đây là ngăn xếp production duy nhất. Ranh giới quan trọng là:

```text
browser → HTTP JSON endpoint → server logic → storage/LLM → JSON response
```

## Vì sao chọn lộ trình này

- Một ngôn ngữ giúp giảm việc chuyển đổi tư duy.
- API tách riêng giúp nhìn rõ ranh giới FE/BE.
- SQLite khiến bài thực hành lưu trữ đầu tiên rẻ và dễ chạy cục bộ.
- Có thể giới thiệu Postgres/Supabase như một lựa chọn triển khai mà không thay đổi mô hình tư duy về schema.

## Những nội dung chủ động lược bỏ

Khóa học cốt lõi không đi sâu vào xác thực, hàng đợi, microservice, ORM hay khả năng quan sát trong môi trường production. Chỉ bổ sung các nội dung này ở khóa nâng cao tiếp theo.
