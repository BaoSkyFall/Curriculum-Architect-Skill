# Buổi 6 — Từ design artifact đến frontend vertical slice (Giữa kỳ)

Duration: 90 phút
Prerequisites: buổi 2, 5
Artifact: **ICP Discovery Prototype**

## Objectives

Biến design brief thành frontend chạy được với mock data và boundary rõ; chốt architecture trước LLM.

## Midterm brief

Tạo prototype có chat input, bảng company/tier và company detail. Có mock API hoặc local JSON; chưa cần LLM, embeddings hay production auth.

## Flow

- 0–15: inspect starter repo và boundary.
- 15–30: demo build một screen từ spec.
- 30–70: paired lab.
- 70–80: 3-minute demo mỗi nhóm.
- 80–90: architecture feedback.

## Lab / success criteria

- Có 3 screen hoặc một screen responsive với 4 states.
- Frontend lấy data qua mock boundary, không hardcode mọi response trong component.
- Có README data flow và known limitations.

## Assessment

30% data-flow explanation, 30% observable UI states, 20% boundary discipline, 20% reflection/debug log.

## Bridge

Buổi sau thay mock boundary bằng backend route thật; UI giữ nguyên contract nếu contract tốt.
