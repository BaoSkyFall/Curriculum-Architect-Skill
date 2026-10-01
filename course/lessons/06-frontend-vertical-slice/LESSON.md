# Buổi 6 — Từ sản phẩm thiết kế đến lát cắt frontend (Giữa kỳ)

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 2, 5
Sản phẩm: **ICP Discovery Prototype**

## Mục tiêu

Biến design brief thành frontend chạy được với dữ liệu mock và ranh giới rõ; chốt kiến trúc trước LLM.

## Đề bài giữa kỳ

Tạo prototype có ô nhập chat, bảng company/tier và chi tiết company. Có mock API hoặc JSON cục bộ; chưa cần LLM, embeddings hay xác thực production.

## Tiến trình

- 0–15: kiểm tra starter repo và ranh giới.
- 15–30: demo xây một màn hình từ spec.
- 30–70: thực hành theo cặp.
- 70–80: mỗi nhóm demo 3 phút.
- 80–90: phản hồi về kiến trúc.

## Bài thực hành / tiêu chí đạt

- Có 3 màn hình hoặc một màn hình responsive với 4 trạng thái.
- Frontend lấy dữ liệu qua ranh giới mock, không hardcode mọi response trong component.
- Có README mô tả luồng dữ liệu và các giới hạn đã biết.

## Đánh giá

30% giải thích luồng dữ liệu, 30% trạng thái UI quan sát được, 20% kỷ luật ranh giới, 20% nhật ký phản hồi/debug.

## Kết nối sang buổi sau

Buổi sau thay mock boundary bằng backend route thật; UI giữ nguyên contract nếu contract tốt.
