# Buổi 2 — Frontend, backend, API và cơ sở dữ liệu

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 1
Sản phẩm: sơ đồ request/response + wireframe bốn trạng thái

## Mục tiêu

Học viên giải thích được ranh giới FE/BE/API/DB, request/response, JSON và sự khác nhau giữa dữ liệu tạm thời với dữ liệu được lưu bền vững.

## Mô hình tư duy

```text
Frontend gửi HTTP request → backend xử lý → cơ sở dữ liệu đọc/ghi → JSON response
```

## Tiến trình

- 0–15: dùng ví dụ đặt lịch để phân biệt giao diện, bộ phận xử lý và nơi lưu hồ sơ.
- 15–35: demo `POST /appointments` với JSON.
- 35–50: nhận diện trạng thái đang tải, trống, thành công và lỗi.
- 50–80: lab vẽ request/response và wireframe.
- 80–90: sửa các hiểu lầm phổ biến.

## Bài thực hành

Viết request và response mẫu cho thao tác tạo lịch hẹn, sau đó vẽ giao diện cho bốn trạng thái: chưa có dữ liệu, đang gửi, thành công và thất bại.

## Lỗi thường gặp

- Nghĩ API là cơ sở dữ liệu.
- Lưu dữ liệu quan trọng chỉ trong biến của giao diện.
- Đưa API key hoặc logic nhạy cảm vào frontend.
- Chỉ thiết kế trạng thái thành công.

## Đánh giá / bài tập về nhà

Đạt khi học viên giải thích được đường đi của một click. Bài tập về nhà: chọn một thao tác khác và ghi ba điểm có thể thất bại.
