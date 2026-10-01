# Buổi 2 — Frontend, backend, API và cơ sở dữ liệu

Thời lượng: 90 phút
Điều kiện tiên quyết: buổi 1
Sản phẩm: sơ đồ request/response + wireframe ba trạng thái

## Mục tiêu

Học viên giải thích được boundary FE/BE/API/DB, request/response, JSON và persistent memory.

## Mô hình tư duy

```text
Frontend gửi HTTP request → backend route xử lý → database đọc/ghi → JSON response
```

## Tiến trình

- 0–15: so sánh giao diện, nhân viên xử lý và hồ sơ lưu trữ.
- 15–35: demo `POST /chat` với JSON.
- 35–50: chỉ ra trạng thái đang tải, trống, thành công, lỗi.
- 50–80: lab vẽ request/response và wireframe chat/kết quả.
- 80–90: kiểm tra hiểu lầm.

## Bài thực hành

Viết một request mẫu và response mẫu cho “xếp hạng prospect”, sau đó tạo wireframe có 4 states.

Tiêu chí đạt: JSON có field rõ ràng; trạng thái lỗi không bị bỏ quên.

## Lỗi thường gặp

Gọi cơ sở dữ liệu là “biến toàn cục”; nghĩ API là cơ sở dữ liệu; nhét API key vào frontend.

## Đánh giá / bài tập về nhà

Giải thích đường đi của một click. Bài tập về nhà: chụp sơ đồ và ghi 3 điểm có thể thất bại.
