# Radar công nghệ

Xác minh gần nhất: 2026-10-01
Chu kỳ rà soát: trước mỗi khóa và ngay sau khi có bản phát hành lớn hoặc thay đổi quyền truy cập.

## Tóm tắt

| Công nghệ | Vai trò | Trạng thái | Dạy | Rủi ro | Quyết định |
|---|---|---|---|---|---|
| OpenAI Codex | triển khai coding agent | đang hoạt động | tùy chọn chính | trung bình | Dùng nếu giảng viên đã hỗ trợ Codex; khái niệm vẫn có thể chuyển đổi |
| Claude Code | triển khai coding agent | đang hoạt động | tùy chọn chính | trung bình | Dùng làm track duy nhất nếu quyền truy cập Anthropic thuận tiện hơn |
| Oh My Codex (OMX) | lớp điều phối | đang hoạt động / thay đổi nhanh | tùy chọn | cao | Dạy khái niệm điều phối; chỉ demo sau khi workflow agent native đã chạy |
| Oh My ClaudeCode (OMC) | lớp điều phối | đang hoạt động / thay đổi nhanh | tùy chọn | cao | Vai trò giống OMX; không dạy cả hai trong lộ trình cốt lõi |
| MCP | giao thức kết nối tool/dữ liệu | đang hoạt động | có | trung bình | Dạy ranh giới và một server an toàn, không dạy cả danh mục server |
| Google Stitch + Stitch MCP | sinh thiết kế / bàn giao | đang hoạt động / thay đổi nhanh | tùy chọn | cao | Dùng để tạo sản phẩm thiết kế nếu quyền truy cập ổn định; luôn giữ phương án screenshot/spec |
| UI/UX Pro Max | skill về tư duy thiết kế | dự án cộng đồng đang hoạt động | tùy chọn | trung bình | Dùng như rubric/tài liệu tham khảo, không làm nền tảng thiết kế |
| Lovable | trừu tượng hóa toàn ứng dụng | đang hoạt động | chỉ so sánh | cao | Cho thấy lợi ích của trừu tượng hóa và những gì nó che giấu |
| React + Vite | triển khai frontend | đang hoạt động | có | thấp | Đủ ổn định để thể hiện rõ ranh giới frontend |
| Node.js API | triển khai backend | đang hoạt động | có | thấp | Giữ logic endpoint nhỏ; dùng một ngôn ngữ cho FE/BE |
| SQLite / Postgres | lưu trữ | đang hoạt động | có | thấp | SQLite cho bài lab; Postgres/Supabase tùy chọn cho triển khai dùng chung |
| SDK của provider LLM | lời gọi model | đang hoạt động / thay đổi nhanh | có | trung bình | Dạy messages và structured output; giữ adapter provider mỏng |
| Embeddings + retrieval | khái niệm tìm kiếm ngữ nghĩa | đang hoạt động | có | trung bình | Trước tiên triển khai trên tập dữ liệu nhỏ; vector DB là tùy chọn |

## Chi tiết

### Codex / Claude Code

trạng thái: đang hoạt động
last_verified: 2026-10-01
bằng chứng: [Tài liệu OpenAI Codex](https://platform.openai.com/docs/codex), [Tổng quan Claude Code](https://code.claude.com/docs/en/overview)

Quyết định giảng dạy: chọn một runtime cho khâu thiết lập và bài lab. Chuẩn đầu ra là agent, context, tool, verification và phân rã task — không phải ghi nhớ một CLI.

### OMX / OMC

trạng thái: đang hoạt động / thay đổi nhanh
last_verified: 2026-10-01
bằng chứng: [oh-my-codex](https://github.com/Yeachan-Heo/oh-my-codex), [oh-my-claudecode](https://github.com/Yeachan-Heo/oh-my-claudecode)

Quyết định giảng dạy: chưa có cơ sở để xem công cụ nào đã lỗi thời dựa trên hoạt động repository hiện tại, nhưng cả hai thay đổi quá nhanh để làm trục chính của khóa học. Chỉ dùng một bài lab triển khai ngắn sau khi dạy khái niệm agent native.

### MCP

trạng thái: đang hoạt động
last_verified: 2026-10-01
bằng chứng: [Giới thiệu MCP](https://modelcontextprotocol.io/docs/getting-started/intro)

Quyết định giảng dạy: giải thích MCP như một ranh giới tiêu chuẩn để cung cấp tool/dữ liệu cho agent. Học viên phải kiểm tra quyền và các dạng lỗi; không khảo sát lan rộng các marketplace server.

### Stitch / Stitch MCP

trạng thái: đang hoạt động / thay đổi nhanh
last_verified: 2026-10-01
bằng chứng: [Google Stitch](https://stitch.withgoogle.com/), [Skill Google Stitch](https://github.com/google-labs-code/stitch-skills), [Stitch MCP CLI](https://github.com/davideast/stitch-mcp)

Quyết định giảng dạy: hữu ích để sinh bản khám phá thiết kế và sản phẩm bàn giao. Vì quyền truy cập và tích hợp có thể thay đổi, mọi bài lab phải chạy được từ screenshot, HTML export hoặc design brief nếu Stitch không khả dụng.

### UI/UX Pro Max

trạng thái: dự án cộng đồng đang hoạt động
last_verified: 2026-10-01
bằng chứng: [repository](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)

Quyết định giảng dạy: tài liệu tham khảo tùy chọn về tư duy thiết kế, hệ thống phân cấp, typography, khoảng cách và rà soát. Không biến cú pháp lệnh của công cụ thành điều kiện tiên quyết.

### Lovable

trạng thái: đang hoạt động
last_verified: 2026-10-01
bằng chứng: [Tài liệu Lovable](https://docs.lovable.dev/introduction)

Quyết định giảng dạy: dùng cho phần so sánh 10 phút. Đây là công cụ trừu tượng hóa toàn ứng dụng, nên không thể thay thế Stitch hoặc UI/UX Pro Max và không được thay cho các bài học về ranh giới.

### Ngăn xếp LLM / retrieval

trạng thái: đang hoạt động / thay đổi nhanh
last_verified: 2026-10-01
bằng chứng: [OpenAI embeddings](https://platform.openai.com/docs/guides/embeddings), [OpenAI retrieval](https://platform.openai.com/docs/guides/retrieval), [Supabase AI](https://supabase.com/docs/guides/ai)

Quyết định giảng dạy: giữ một adapter quanh provider, dùng structured output và đánh giá retrieval trên bộ kiểm thử nhỏ có gắn nhãn. Không hứa hẹn hành vi đặc thù của một model sẽ giống nhau giữa các provider.
