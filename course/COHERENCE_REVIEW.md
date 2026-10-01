# Rà soát tính nhất quán — v0.1

## Kết quả

Trạng thái: có thể giảng dạy với khâu thiết lập được kiểm soát
Vấn đề nghiêm trọng: 0
Cảnh báo: 4
Đề xuất: 5

## Kiểm tra

- Mức phù hợp với mục tiêu: đạt — mọi mô-đun tạo sản phẩm cho ICP chatbot.
- Tính toàn vẹn của điều kiện tiên quyết: đạt — LLM trước RAG, persistence trước pipeline.
- Tiến triển độ khó: đạt kèm cảnh báo — buổi 10–11 nặng, cần dùng starter repo.
- Độ phủ khái niệm: đạt — có đầy đủ FE/BE/API/DB/agent/MCP/LLM/pipeline/retrieval.
- Độ bền của công cụ: đạt kèm cảnh báo — tool được đặt dưới khái niệm và có phương án thay thế.
- Tích hợp dự án: đạt — giữa kỳ là vertical slice, cuối khóa là mở rộng liên tục.
- Chất lượng đánh giá: đạt — chấm luồng dữ liệu, evidence, debug và trade-off.
- Khả năng tiếp cận với người non-tech: đạt kèm cảnh báo — cần chuẩn bị glossary, sơ đồ và bài lab theo cặp.

## Cảnh báo / Biện pháp giảm thiểu

1. Thiết lập tài khoản/API có thể chiếm thời gian → chuẩn bị starter repo, `.env.example`, dataset và fallback mock.
2. Thuật ngữ embedding/vector nặng → dạy retrieval trên bảng nhỏ trước, chỉ sau đó dùng vector store.
3. Dữ liệu ICP dễ chứa PII → chỉ dùng dữ liệu giả lập/ẩn danh và có checklist riêng tư.
4. OMC/OMX/UI tools có thể đổi CLI → kiểm tra `TECH_RADAR.md` trước khóa; không chấm theo UI của tool.

## Lần rà soát tiếp theo

Xác minh lại các mục công nghệ trước mỗi khóa hoặc khi có bản phát hành lớn/ngừng hỗ trợ.
