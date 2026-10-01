# Buổi 6 — Từ sản phẩm thiết kế đến lát cắt frontend (Giữa kỳ)

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 2, 5
Sản phẩm: prototype frontend có boundary rõ

## Mục tiêu

Biến design brief thành frontend chạy được với dữ liệu mock; giữ contract ổn định; chốt kiến trúc trước khi thêm dịch vụ phức tạp.

## Đề bài giữa kỳ

Chọn một trong ba ngữ cảnh: ứng dụng danh sách việc, ứng dụng đặt lịch hoặc thư viện tài liệu. Prototype cần có màn hình danh sách, chi tiết và một thao tác chính. Chưa cần LLM, embeddings hay xác thực production.

## Tiến trình

- 0–15: kiểm tra starter repo và ranh giới.
- 15–30: demo xây một màn hình từ spec.
- 30–70: thực hành theo cặp.
- 70–80: mỗi nhóm demo 3 phút.
- 80–90: phản hồi về kiến trúc và contract.

## Bài thực hành / tiêu chí đạt

- Có ba màn hình hoặc một màn hình responsive với bốn trạng thái.
- Frontend lấy dữ liệu qua mock boundary, không hardcode mọi response trong component.
- Có README mô tả luồng dữ liệu, contract và các giới hạn đã biết.

## Đánh giá

30% giải thích luồng dữ liệu, 30% trạng thái UI quan sát được, 20% kỷ luật ranh giới, 20% nhật ký phản hồi/debug.

## Kết nối sang buổi sau

Buổi sau thay mock boundary bằng backend route thật; UI giữ nguyên contract nếu contract tốt.
