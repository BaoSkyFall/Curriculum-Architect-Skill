# Course Specification

Course name: Vibe Coding cho người non-tech: Xây dựng ICP Chatbot
CURRICULUM_VERSION: v0.1
Audience: người non-tech, dùng máy tính tốt, có thể đã dùng AI chat nhưng chưa hiểu software architecture
Prerequisites: browser, file management, basic spreadsheet, willingness to inspect AI-generated work
Duration: 12 buổi x 90 phút = 18 giờ
Teaching format: 25 phút mental model + 20 phút demo + 35 phút guided lab + 10 phút explanation check

## Purpose

Giúp học viên hiểu request, data, state, errors và boundaries của một ứng dụng AI; sau đó vibe-code một chatbot hỗ trợ quy trình xây dựng ICP thay vì chỉ tạo một giao diện “trông có vẻ chạy”.

## Core Concepts

Software flow, frontend, backend, API, HTTP/JSON, database, agent, context, skill, MCP, delegation, UI/UX, LLM messages, structured output, streaming, ingestion, cleaning, chunking, embeddings, retrieval, RAG, evaluation, privacy và debugging.

## Primary Teaching Path

- Một coding-agent runtime duy nhất trong lớp: Codex + OMX **hoặc** Claude Code + OMC.
- Shared concepts được dạy độc lập với vendor. Tool chỉ là implementation lab.
- UI design dùng một design artifact có thể xuất thành ảnh/HTML/spec; Stitch là lựa chọn ưu tiên nếu access ổn định, UI/UX Pro Max là lớp design intelligence tùy chọn, Lovable chỉ dùng để so sánh abstraction.
- Backend dạy theo boundary rõ ràng: frontend riêng gọi API backend riêng.

## Module Sequence

1. Software mental model và vibe coding
2. Frontend, backend, API, database
3. Agent, context, skills, MCP và verification
4. Multi-agent orchestration và task decomposition
5. UI/UX mental model và AI-assisted design
6. Từ design artifact đến frontend vertical slice — **giữa kỳ**
7. Backend service, HTTP, JSON và error handling
8. Nhúng LLM: messages, structured output, streaming
9. Database và model dữ liệu ICP
10. Data pipeline: CRM → clean → enrich → store
11. Embeddings, retrieval, RAG và đánh giá
12. Tích hợp, debugging, security và demo capstone

## Assessment Strategy

- Formative: artifact nhỏ sau mỗi buổi và câu hỏi “hãy giải thích data flow”.
- Midterm (buổi 6): ICP Discovery Prototype — schema dữ liệu, architecture map, UI và endpoint mock, có thể chấm bằng dữ liệu giả lập; chưa cần LLM/RAG.
- Final (buổi 12): ICP Chatbot — pipeline, scoring, tiering, historical backtest, grounded explanation và danh sách prospect tương tự.
- Không chấm syntax như mục tiêu chính; chấm boundary, reasoning, observable behavior, error handling và khả năng kiểm chứng.
