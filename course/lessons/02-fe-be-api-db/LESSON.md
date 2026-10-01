# Buổi 2 — Frontend, backend, API và database

Duration: 90 phút
Prerequisites: buổi 1
Artifact: request/response map + wireframe ba trạng thái

## Objectives

Học viên giải thích được boundary FE/BE/API/DB, request/response, JSON và persistent memory.

## Mental model

```text
Frontend gửi HTTP request → backend route xử lý → database đọc/ghi → JSON response
```

## Flow

- 0–15: so sánh giao diện, nhân viên xử lý và hồ sơ lưu trữ.
- 15–35: demo `POST /chat` với JSON.
- 35–50: chỉ ra loading, empty, success, error.
- 50–80: lab vẽ request/response và wireframe chat/results.
- 80–90: misconception check.

## Lab

Viết một request mẫu và response mẫu cho “xếp hạng prospect”, sau đó tạo wireframe có 4 states.

Success: JSON có field rõ ràng; state error không bị bỏ quên.

## Common mistakes

Gọi database là “biến toàn cục”; nghĩ API là database; nhét API key vào frontend.

## Assessment / homework

Giải thích đường đi của một click. Homework: chụp sơ đồ và ghi 3 điểm có thể fail.
