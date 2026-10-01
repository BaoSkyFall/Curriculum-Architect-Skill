# Nghiên cứu: Ngăn xếp LLM

Xác minh: 2026-10-01

## Cam kết giảng dạy

Học viên phải hiểu ở mức khái quát về `system message`, `user message`, context, token, structured output, streaming, gọi tool và xử lý lỗi/timeout.

## Lựa chọn triển khai

Dùng provider đã có sẵn với giảng viên. Bọc lời gọi trong một hàm backend để bài học có thể đổi giữa OpenAI Responses và Anthropic Messages mà không sửa frontend. Lưu tên model và key trong biến môi trường.

## Rào chắn riêng cho ICP

LLM có thể trích xuất signal, tóm tắt evidence và đề xuất cách giải thích score. Phiên bản rubric, các ngưỡng và tier cuối phải là sản phẩm có thể kiểm tra, đồng thời phải kiểm thử được trên dữ liệu lịch sử.

## Ngoài phạm vi

Toán học Transformer, fine-tuning, quyết định bán hàng tự động và việc coi output của model là sự thật tuyệt đối.
