# Đặc tả khóa học

Tên khóa học: Vibe Coding cho người non-tech: Xây dựng ICP Chatbot
CURRICULUM_VERSION: v0.1
Đối tượng: người non-tech, dùng máy tính tốt, có thể đã dùng AI chat nhưng chưa hiểu kiến trúc phần mềm
Điều kiện tiên quyết: trình duyệt, quản lý tệp, bảng tính cơ bản và sẵn sàng kiểm tra sản phẩm do AI tạo
Thời lượng: 12 buổi x 90 phút = 18 giờ
Hình thức giảng dạy: 25 phút mô hình tư duy + 20 phút demo + 35 phút thực hành có hướng dẫn + 10 phút kiểm tra giải thích

## Mục đích

Giúp học viên hiểu request, dữ liệu, trạng thái, lỗi và ranh giới của một ứng dụng AI; sau đó vibe-code một chatbot hỗ trợ quy trình xây dựng ICP thay vì chỉ tạo một giao diện “trông có vẻ chạy”.

## Khái niệm cốt lõi

Luồng phần mềm, frontend, backend, API, HTTP/JSON, cơ sở dữ liệu, agent, context, skill, MCP, delegation, UI/UX, LLM messages, structured output, streaming, ingestion, cleaning, chunking, embeddings, retrieval, RAG, đánh giá, riêng tư và debug.

## Lộ trình giảng dạy chính

- Một coding-agent runtime duy nhất trong lớp: Codex + OMX **hoặc** Claude Code + OMC.
- Các khái niệm dùng chung được dạy độc lập với vendor. Tool chỉ là phương tiện triển khai trong bài lab.
- Thiết kế UI dùng một sản phẩm thiết kế có thể xuất thành ảnh/HTML/spec; Stitch là lựa chọn ưu tiên nếu quyền truy cập ổn định, UI/UX Pro Max là lớp tư duy thiết kế tùy chọn, Lovable chỉ dùng để so sánh mức độ trừu tượng hóa.
- Backend dạy theo boundary rõ ràng: frontend riêng gọi API backend riêng.

## Trình tự mô-đun

1. Mô hình tư duy phần mềm và vibe coding
2. Frontend, backend, API, cơ sở dữ liệu
3. Agent, context, skill, MCP và kiểm chứng
4. Điều phối đa agent và phân rã task
5. Mô hình tư duy UI/UX và thiết kế có AI hỗ trợ
6. Từ sản phẩm thiết kế đến lát cắt frontend — **giữa kỳ**
7. Dịch vụ backend, HTTP, JSON và xử lý lỗi
8. Tích hợp LLM: messages, structured output, streaming
9. Cơ sở dữ liệu và mô hình dữ liệu ICP
10. Pipeline dữ liệu: CRM → làm sạch → enrichment → lưu trữ
11. Embeddings, retrieval, RAG và đánh giá
12. Tích hợp, debug, bảo mật và demo đồ án cuối khóa

## Chiến lược đánh giá

- Đánh giá thường xuyên: sản phẩm nhỏ sau mỗi buổi và câu hỏi “hãy giải thích luồng dữ liệu”.
- Giữa kỳ (buổi 6): ICP Discovery Prototype — schema dữ liệu, sơ đồ kiến trúc, UI và endpoint mock, có thể chấm bằng dữ liệu giả lập; chưa cần LLM/RAG.
- Cuối khóa (buổi 12): ICP Chatbot — pipeline, chấm điểm, phân tier, kiểm thử lịch sử, giải thích có căn cứ và danh sách prospect tương tự.
- Không chấm cú pháp như mục tiêu chính; chấm ranh giới, lập luận, hành vi quan sát được, xử lý lỗi và khả năng kiểm chứng.
