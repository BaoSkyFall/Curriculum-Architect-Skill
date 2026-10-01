# Nghiên cứu: Ngăn xếp dữ liệu và retrieval

Xác minh: 2026-10-01

## Tiến trình học tập

1. Bắt đầu với các dòng CSV và một bảng có thể quan sát.
2. Lưu các record company/outcome/signal trong SQLite.
3. Thêm log ingestion và lý do loại bỏ từng dòng.
4. Thêm enrichment như một nguồn riêng có provenance.
5. Dạy chunking và metadata trên một tập tài liệu nhỏ.
6. So sánh lọc theo từ khóa với embeddings/retrieval.
7. Chỉ thêm RAG sau khi đã có bộ kiểm thử retrieval.

## Khuyến nghị

Dùng SQLite cho các bài thực hành đầu tiên, sau đó dùng một triển khai retrieval cục bộ đơn giản hoặc Postgres/pgvector/Supabase cho đồ án cuối khóa tích hợp. Cơ sở dữ liệu vector được quản lý là tùy chọn, không bắt buộc để hiểu RAG.

## Đánh giá

Mỗi demo retrieval đều có câu hỏi được gắn nhãn và evidence kỳ vọng. Theo dõi việc câu trả lời có trích dẫn đúng record liên quan hay không, thay vì chỉ xem câu trả lời có trôi chảy.

## An toàn

Dùng dữ liệu CRM giả lập hoặc ẩn danh, ghi nguồn và thời điểm của enrichment, đồng thời hướng dẫn học viên xóa hoặc che thông tin trong record trước khi gửi context cho LLM.
