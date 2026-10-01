# Bản đồ chương trình

| Buổi | Mô-đun | Điều kiện tiên quyết | Sản phẩm trong buổi | Liên kết tới đồ án cuối khóa |
|---:|---|---|---|---|
| 1 | Mô hình tư duy phần mềm | Không | Sơ đồ hệ thống của ICP chatbot | Kiến trúc tổng thể |
| 2 | FE/BE/API/DB | 1 | Request/response map + UI wireframe | Boundary của app |
| 3 | Agent, skill, MCP | 1 | Thỏa thuận làm việc với agent + task đã kiểm chứng | Cách dùng agent an toàn |
| 4 | Điều phối đa agent | 3 | Phân rã task + log bàn giao | Chia pipeline thành việc nhỏ |
| 5 | UI/UX và thiết kế AI | 1–2 | Design brief + trạng thái màn hình | Màn hình chat, score và evidence |
| 6 | Lát cắt frontend | 2, 5 | **ICP Discovery Prototype giữa kỳ** | UI + mock API |
| 7 | Dịch vụ backend | 2, 6 | `POST /companies/score` hoặc mock route | Ranh giới chấm điểm |
| 8 | Backend LLM | 7 | Endpoint trích xuất/chấm điểm bằng LLM | AI phân tích pattern |
| 9 | Cơ sở dữ liệu | 2, 7 | Schema + CRUD + trường audit | Lưu company/evidence/score |
| 10 | Pipeline dữ liệu | 9 | Báo cáo một lần chạy ingestion | Luồng CRM và enrichment |
| 11 | Retrieval/RAG/đánh giá | 8–10 | Bộ kiểm thử retrieval + câu trả lời có căn cứ | Evidence và giải thích score |
| 12 | Tích hợp/debug/demo | Tất cả | **ICP Chatbot cuối khóa** | Sản phẩm hoàn chỉnh |

## Lý do sắp xếp

Khóa học dạy ranh giới trước tool, đường đi của request trước độ phức tạp dữ liệu, persistence trước pipeline và pipeline/retrieval trước RAG. Giữa kỳ chốt kiến trúc trước khi thêm LLM.

## Phương án rút gọn còn 10 buổi

Nếu chỉ có 10 buổi, gộp (3 + 4) thành một buổi workflow dùng agent và gộp (7 + 8) thành một buổi backend + LLM. Không gộp cơ sở dữ liệu với pipeline vì đó là dependency quan trọng.

## Khoảng trống cần xem xét lại

- Xác thực, triển khai production, tính phí và observability chưa phải chuẩn đầu ra của khóa này.
- Cơ sở dữ liệu vector chuyên dụng là tùy chọn; bản đầu dùng retrieval đơn giản hoặc Postgres/pgvector nếu khóa học đủ năng lực.
