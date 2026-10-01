# Các quyết định về chương trình

## ADR-001: 12 buổi thay vì 9 buổi

Ngày: 2026-10-01
Trạng thái: đã chấp nhận

### Câu hỏi

Khối lượng FE, BE, agent, LLM, pipeline, retrieval và capstone có thể dạy trong 9 buổi không?

### Quyết định

Dùng 12 buổi làm bản dạy chuẩn; có lộ trình rút gọn 10 buổi. 9 buổi chỉ phù hợp workshop giới thiệu, không đủ thời gian cho giữa kỳ và backtest.

### Hệ quả

Giữ được lát cắt dọc và workflow ICP cuối khóa; giáo viên có thể bỏ mục tiêu mở rộng thay vì bỏ dependency.

## ADR-002: Một agent track trong lớp

Ngày: 2026-10-01
Trạng thái: đã chấp nhận

### Câu hỏi

Có nên dạy cả OMC và OMX không?

### Quyết định

Dạy các khái niệm chung và chọn một runtime chính. Mặc định ghi lab theo track tương thích Codex/OMX nếu giáo viên đã có quyền truy cập; đổi sang Claude Code/OMC không làm thay đổi chuẩn đầu ra.

### Bối cảnh

Hai runtime đều là lớp điều phối thay đổi nhanh. Dạy song song làm tăng thời gian thiết lập và phân mảnh thời gian nhưng không thêm mô hình tư duy cốt lõi.

### Xem xét lại khi

Một runtime có capability khác biệt thực sự cần cho chuẩn đầu ra, hoặc khóa học có giấy phép/quyền truy cập không đồng nhất.

## ADR-003: Stitch không phải learning objective

Ngày: 2026-10-01
Trạng thái: đã chấp nhận

### Quyết định

Dạy design brief, hệ thống phân cấp, trạng thái và bàn giao trước. Stitch/MCP là triển khai sinh thiết kế tùy chọn; Lovable dùng để so sánh mức độ trừu tượng hóa; UI/UX Pro Max là tài liệu tham khảo về tư duy thiết kế.

### Lý do

Ba công cụ giải quyết ba lớp khác nhau và có thể thay đổi hoặc biến mất mà không làm mất kiến thức UI/UX.

## ADR-004: Không để LLM quyết định score một cách không kiểm soát

Ngày: 2026-10-01
Trạng thái: đã chấp nhận

### Quyết định

LLM chỉ đề xuất feature/evidence hoặc đánh giá có cấu trúc. Rubric, phiên bản, ngưỡng và bài kiểm thử lịch sử là các sản phẩm có thể kiểm tra; score cuối phải có rule hoặc chính sách được con người phê duyệt.

### Lý do

ICP là quyết định kinh doanh có khả năng gây bias; output tự do của LLM không đủ khả năng tái lập.
