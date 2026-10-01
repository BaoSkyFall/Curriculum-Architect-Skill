# Nghiên cứu: Coding agent và điều phối

Xác minh: 2026-10-01

## Bằng chứng

- Tài liệu chính thức của Claude Code mô tả đây là công cụ coding agent có thể đọc codebase, sửa tệp, chạy lệnh và tích hợp với công cụ phát triển: <https://code.claude.com/docs/en/overview>.
- OpenAI duy trì tài liệu Codex hiện hành tại <https://platform.openai.com/docs/codex>.
- Oh My ClaudeCode mô tả một lớp điều phối đa agent ưu tiên làm việc theo nhóm: <https://github.com/Yeachan-Heo/oh-my-claudecode>.
- Oh My Codex mô tả hooks, nhóm agent và hỗ trợ workflow cho Codex CLI: <https://github.com/Yeachan-Heo/oh-my-codex>.
- MCP có tài liệu giới thiệu giao thức và bắt đầu sử dụng hiện hành: <https://modelcontextprotocol.io/docs/getting-started/intro>.

## Quyết định giảng dạy

Trước tiên dạy mô hình ổn định:

```text
model → agent → context → tools → skills/MCP → subagents → orchestration → verification
```

Sau đó thực hiện một bài thực hành công cụ. Học viên viết thỏa thuận làm việc với agent, gồm task, tệp ngữ cảnh, ràng buộc, tiêu chí nghiệm thu và lệnh kiểm tra. Không cần cài cả OMC lẫn OMX.

## Rủi ro

- Cờ CLI, cách cài đặt và tên gọi có thể thay đổi nhanh.
- Chạy song song nhiều agent có thể làm tăng chi phí, xung đột context và độ khó khi debug.
- Một bản vá được tạo thành công không phải bằng chứng rằng nó đúng.

## Phương án dự phòng

Nếu lớp điều phối gặp lỗi, dùng task native của agent và bảng bàn giao bằng văn bản. Mục tiêu học tập vẫn là phân rã công việc và kiểm chứng.
