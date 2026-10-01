# Curriculum Decisions

## ADR-001: 12 buổi thay vì 9 buổi

Date: 2026-10-01
Status: accepted

### Question

Khối lượng FE, BE, agent, LLM, pipeline, retrieval và capstone có thể dạy trong 9 buổi không?

### Decision

Dùng 12 buổi làm bản dạy chuẩn; có compression path 10 buổi. 9 buổi chỉ phù hợp workshop giới thiệu, không đủ thời gian cho midterm và backtest.

### Consequence

Giữ được vertical slice và final ICP workflow; giáo viên có thể bỏ stretch goals thay vì bỏ dependency.

## ADR-002: Một agent track trong lớp

Date: 2026-10-01
Status: accepted

### Question

Có nên dạy cả OMC và OMX không?

### Decision

Dạy concepts chung và chọn một runtime chính. Mặc định ghi lab theo Codex-compatible track/OMX nếu giáo viên đã có access; đổi sang Claude Code/OMC không đổi learning outcomes.

### Context

Hai runtime đều là lớp orchestration thay đổi nhanh. Dạy song song làm tăng setup và phân mảnh thời gian nhưng không thêm mental model cốt lõi.

### Revisit When

Một runtime có capability khác biệt thực sự cần cho outcome, hoặc cohort có license/access không đồng nhất.

## ADR-003: Stitch không phải learning objective

Date: 2026-10-01
Status: accepted

### Decision

Dạy design brief, hierarchy, states và handoff trước. Stitch/MCP là design-generation implementation tùy chọn; Lovable là abstraction comparison; UI/UX Pro Max là design-intelligence reference.

### Reason

Ba công cụ giải quyết ba lớp khác nhau và có thể thay đổi hoặc biến mất mà không làm mất kiến thức UI/UX.

## ADR-004: Không để LLM quyết định score một cách không kiểm soát

Date: 2026-10-01
Status: accepted

### Decision

LLM chỉ đề xuất feature/evidence hoặc structured assessment. Rubric, version, threshold và historical test là artifact có thể inspect; score cuối phải có rule hoặc human-approved policy.

### Reason

ICP là quyết định kinh doanh có khả năng gây bias; output tự do của LLM không đủ reproducible.
