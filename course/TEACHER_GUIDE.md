# Hướng dẫn giảng viên

## Trước khi bắt đầu khóa

- Xác minh một track agent, provider model, phiên bản Node.js và các tài khoản.
- Chuẩn bị starter repo với `frontend/`, `backend/`, `data/`, `.env.example`, CSV seed và chế độ mock.
- Chuẩn bị 30–50 record company giả lập có kết quả mua/không mua.
- Chuẩn bị glossary in giấy và một sơ đồ kiến trúc.
- Kiểm thử phương án dự phòng không có Stitch, plugin điều phối và LLM trực tiếp.

## Quy tắc điều phối

- Không để khâu thiết lập chiếm cả 90 phút; ghép cặp học viên và cung cấp một checkpoint đã biết là hoạt động đúng.
- Sau mỗi demo, hỏi “đầu vào là gì, đầu ra là gì và có thể lỗi ở đâu?”.
- Học viên phải giải thích một thay đổi do AI tạo ra trước khi chấp nhận.
- Duy trì một ví dụ miền ổn định: company → outcome → signals → score → tier → evidence.

## Cách xử lý sự cố thường gặp

- Lỗi API key: chuyển sang provider mock.
- Lỗi agent/plugin: dùng agent native cùng checklist bàn giao.
- Lỗi retrieval: trình bày baseline theo từ khóa và kiểm tra chunk trước khi đổi model.
- Tool UI không khả dụng: dùng PNG/HTML được cung cấp và tiếp tục với states/spec.
