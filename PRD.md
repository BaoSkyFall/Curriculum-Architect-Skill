# PRD — Vibe Code Curriculum Architect Skill

## 1. Product Overview

### Product Name
`vibe-code-curriculum-architect`

### Product Type
Agent Skill / Curriculum Design Assistant

### Target Runtime
- Claude Code
- OpenAI Codex
- Các agent runtime hỗ trợ Agent Skills / `SKILL.md`

### Primary Goal

Xây dựng một AI Skill có khả năng hỗ trợ người thiết kế khóa học:

> “Vibe Coding for Non-Tech”

biến các ý tưởng, công nghệ, blocker và yêu cầu còn rời rạc thành một chương trình học:

- Có cấu trúc rõ ràng
- Có dependency giữa các kiến thức
- Có learning outcome
- Có module
- Có lesson plan
- Có lab
- Có project
- Có assessment
- Có capstone
- Có tài liệu cho giảng viên
- Có cơ chế research công nghệ hiện tại
- Có cơ chế phát hiện nội dung/tool có nguy cơ lỗi thời

Skill không chỉ là một Lesson Plan Generator.

Skill phải hoạt động như:

> Curriculum Architect + Technical Researcher + Learning Designer + Project-Based Learning Designer + Curriculum Reviewer.

---

# 2. Problem Statement

Khóa học hiện tại có mục tiêu:

> Dạy người không có nền tảng kỹ thuật đủ kiến thức và mental model để có thể sử dụng AI coding agents và vibe-code một ứng dụng thực tế.

Nhưng curriculum hiện tại còn nhiều vấn đề.

## 2.1 Nội dung đang tồn tại dưới dạng các “topic rời rạc”

Ví dụ:

- Frontend
- Backend
- API
- Database
- AI Coding Agent
- MCP
- Skills
- Multi-Agent
- Oh My ClaudeCode
- Oh My Codex
- UI/UX
- Stitch
- UI/UX Pro Max
- Lovable
- LLM
- Backend service
- Data Pipeline
- Embedding
- RAG
- Chatbot

Chưa rõ:

- học cái gì trước
- học cái gì sau
- học đến mức nào
- cái nào là concept
- cái nào là implementation
- cái nào bắt buộc
- cái nào optional
- cái nào chỉ dùng để demo

---

# 3. Core Product Principle

Curriculum phải được xây dựng theo:

```text
Concept → Mental Model → Implementation → Practice → Integration
```

Không được xây dựng curriculum theo:

```text
Tool A
Tool B
Tool C
Tool D
```

Ví dụ không nên có lesson:

```text
Lesson: Oh My ClaudeCode
```

Mà nên là:

```text
Lesson: Multi-Agent Coding Systems

Concepts:
- Agent
- Subagent
- Context
- Skill
- Tool
- MCP
- Delegation
- Orchestration
- Parallel Execution

Implementation Lab:
- Oh My ClaudeCode

Alternative:
- Oh My Codex
```

Như vậy nếu một tool biến mất hoặc lỗi thời, curriculum vẫn giữ nguyên giá trị.

---

# 4. Target User

## Primary User

Người thiết kế / giảng viên khóa học Vibe Coding.

User có thể có nền tảng kỹ thuật nhưng curriculum đang ở trạng thái chưa được chuẩn hóa.

User sẽ cung cấp các input dạng:

```text
Tôi muốn dạy người non-tech vibe coding.

Tôi nghĩ cần dạy:
- FE
- BE
- API
- Database
- OMC
- OMX
- Stitch
- UI UX
- LLM
- Data Pipeline
- RAG
- Chatbot

Nhưng tôi chưa biết:
- Stitch có lỗi thời không?
- Có nên dùng Lovable không?
- UI/UX Pro Max nằm ở đâu?
- OMC hay OMX?
- RAG có cần thiết không?
- Backend nên dùng framework nào?
```

Skill phải biến những input này thành một curriculum có cấu trúc.

---

# 5. Target Student

Khóa học hướng đến:

## Audience

Người:

- Non-tech
- Không phải Software Engineer
- Không hiểu rõ software architecture
- Có thể chưa từng code
- Có thể sử dụng máy tính tốt
- Có khả năng dùng AI tools
- Muốn tạo ứng dụng bằng AI

Không yêu cầu học viên trở thành developer chuyên nghiệp.

---

# 6. Student Outcome

Sau khóa học, học viên phải hiểu:

```text
Frontend
Backend
API
Database
LLM
Data Pipeline
AI Coding Agent
Skills
MCP
Multi-Agent
```

không nhất thiết ở mức chuyên sâu, nhưng đủ để hiểu:

> Các thành phần này tồn tại để làm gì và chúng giao tiếp với nhau như thế nào.

Cuối khóa, học viên phải có khả năng vibe-code một ứng dụng dạng:

```text
User
 ↓
Frontend
 ↓
Backend API
 ↓
LLM
 ↓
Database / Knowledge Source
 ↓
Data Pipeline / Retrieval
 ↓
Response
```

Capstone mặc định:

> Xây dựng AI Chat Application sử dụng dữ liệu riêng.

---

# 7. Curriculum Philosophy

Skill phải ưu tiên:

### 7.1 Mental Model Before Syntax

Không bắt đầu bằng syntax.

Ví dụ:

Không bắt đầu bằng:

```javascript
app.get("/api/users", ...)
```

Mà phải giải thích:

```text
Frontend muốn dữ liệu
      ↓
gửi HTTP request
      ↓
Backend nhận request
      ↓
Backend xử lý
      ↓
Backend trả JSON
      ↓
Frontend hiển thị
```

Sau đó mới đưa code.

---

## 7.2 Build Before Theory Depth

Chỉ dạy theory đủ để unblock việc build.

Ví dụ:

Database:

Không cần dạy:

- B-tree internals
- query planner
- database engine internals

Nhưng cần hiểu:

- table
- row
- column
- ID
- relationship
- query
- CRUD
- database khác variable ở đâu

---

## 7.3 Project-Based Learning

Mọi module phải đóng góp vào capstone cuối khóa.

Ví dụ:

```text
Lesson: API
        ↓
Lab: gọi weather API

Lesson: Backend
        ↓
Lab: tạo endpoint

Lesson: LLM
        ↓
Lab: backend gọi model

Lesson: Database
        ↓
Lab: save chat messages

Lesson: Data Pipeline
        ↓
Lab: ingest tài liệu

Lesson: Retrieval
        ↓
Lab: chatbot trả lời từ tài liệu

        ↓

Final Capstone
```

---

# 8. Main Skill Responsibilities

Skill phải thực hiện 6 trách nhiệm chính.

## 8.1 Curriculum Architect

Biến requirement thành:

```text
Course
 ↓
Modules
 ↓
Lessons
 ↓
Activities
 ↓
Labs
 ↓
Assessments
 ↓
Capstone
```

---

# 8.2 Technical Researcher

Khi curriculum sử dụng công nghệ thay đổi nhanh, Skill phải research trước khi quyết định.

Ví dụ:

```text
Stitch
Lovable
OMC
OMX
Claude Code
Codex
UI/UX Pro Max
MCP
Agent Skills
LLM SDK
Vector Database
```

Phải kiểm tra:

- Official documentation
- Repository activity
- Last update
- Release activity
- Maintainer activity
- Adoption
- Stability
- Current alternatives
- Breaking changes
- Deprecation risk

---

# 8.3 Learning Designer

Skill phải xác định cho mỗi lesson:

- Learning objective
- Prerequisite
- Mental model
- Key concepts
- Teaching sequence
- Demo
- Lab
- Exercise
- Misconceptions
- Assessment
- Homework
- Teacher notes

---

# 8.4 Project Designer

Skill phải tạo practical labs.

Lab phải:

- nhỏ
- observable
- có output rõ ràng
- liên quan tới capstone
- không yêu cầu quá nhiều kiến thức chưa học

---

# 8.5 Coherence Reviewer

Skill phải review toàn curriculum để phát hiện:

### Missing prerequisite

Ví dụ:

```text
Teaching RAG
```

nhưng học viên chưa biết:

```text
HTTP
JSON
Database
LLM API
Embedding
```

→ phải báo lỗi curriculum.

---

### Duplicate content

Ví dụ cùng giải thích REST API ở 3 module.

---

### Complexity jump

Ví dụ:

```text
Lesson 5:
Frontend basic

Lesson 6:
Build distributed vector search pipeline
```

→ complexity jump quá lớn.

---

# 8.6 Tech Radar Maintainer

Skill phải duy trì file:

```text
TECH_RADAR.md
```

để curriculum không bị phụ thuộc vào kiến thức cũ.

---

# 9. Tech Radar

Mỗi technology phải có:

```yaml
name: Google Stitch

category: design

status: active

last_verified: 2026-10-01

role:
  AI-native UI design and prototyping

curriculum_role:
  implementation-tool

teach:
  yes

module:
  UI/UX & Product Design

alternatives:
  - Lovable
  - Figma AI
  - v0

risk:
  medium

reason:
  Tool ecosystem changes quickly.
```

Các status:

```text
recommended
active
experimental
optional
watch
deprecated
remove
```

---

# 10. Architecture Decisions

Skill phải lưu các quyết định quan trọng vào:

```text
DECISIONS.md
```

Ví dụ:

```text
ADR-001

Question:
Should we teach Lovable as the main app builder?

Decision:
No.

Reason:
The curriculum aims to teach how software components
interact instead of hiding them behind a full-stack abstraction.

Lovable can be demonstrated later as an abstraction layer.
```

---

# 11. Initial Curriculum Backbone

Curriculum ban đầu nên theo structure:

```text
0. Vibe Coding Mental Model

1. How Software Works

2. Frontend / Backend / API / Database

3. AI Coding Agents

4. Context, Prompt, Skills and MCP

5. Multi-Agent Coding Systems

6. UI/UX Mental Model

7. AI-Assisted Design

8. From Design to Frontend

9. Backend Service Basics

10. HTTP, API and JSON

11. Using LLMs from Backend

12. Building Chat Interfaces

13. Database Basics

14. Data Ingestion

15. Data Pipelines

16. Embeddings and Retrieval

17. RAG

18. Building the AI Chat Application

19. Debugging AI-generated Software

20. Capstone
```

Đây chỉ là initial hypothesis.

Skill phải có quyền:

- merge module
- split module
- reorder module
- remove module
- add prerequisite

nếu research và curriculum reasoning cho thấy cần thiết.

---

# 12. Curriculum Dependency Graph

Skill phải tạo:

```text
PREREQUISITE_MAP.md
```

Ví dụ:

```text
Software Mental Model
       │
       ├──── Frontend
       │
       ├──── Backend
       │
       └──── Database
                │
                ↓
               API
                │
                ↓
             HTTP/JSON
                │
                ↓
           Backend Service
                │
                ↓
               LLM
                │
                ↓
             Chat App
                │
         ┌──────┴──────┐
         │             │
     Database      Data Pipeline
                       │
                    Embedding
                       │
                    Retrieval
                       │
                      RAG
                       │
                       ▼
               Final AI Product
```

---

# 13. AI Agent Curriculum

Phần này phải dạy:

```text
AI Model
   ↓
Agent
   ↓
Tools
   ↓
Skills
   ↓
MCP
   ↓
Subagents
   ↓
Multi-Agent Orchestration
```

Không được đồng nhất:

```text
Claude Code = Agent concept
```

hoặc:

```text
OMC = Multi-agent concept
```

Tool chỉ là implementation.

---

# 14. OMC / OMX Strategy

Curriculum không nên bắt học viên học cả hai.

Phải hỗ trợ:

```text
Claude Track
    ↓
Oh My ClaudeCode
```

hoặc:

```text
Codex Track
    ↓
Oh My Codex
```

Core knowledge chung:

```text
Agent
Subagent
Skill
MCP
Context
Delegation
Task decomposition
Orchestration
Parallel execution
Verification
```

---

# 15. UI / UX Module

Skill phải phân biệt:

## Design Knowledge

Ví dụ:

```text
UI/UX Pro Max
```

Role:

```text
Design intelligence
Design rules
Typography
Spacing
Color
UX patterns
Visual hierarchy
```

---

## Design Generation

Ví dụ:

```text
Google Stitch
```

Role:

```text
Prompt → visual design
Design exploration
Prototype
Design system generation
```

---

## Full App Abstraction

Ví dụ:

```text
Lovable
```

Role:

```text
Prompt → application
```

Không được xem ba tool này là interchangeable.

---

# 16. Backend Curriculum

Backend module chỉ dạy mức đủ dùng.

Student cần hiểu:

```text
request
response
route
endpoint
server
environment variable
API key
JSON
async request
error handling
```

Backend project:

```text
POST /chat

Input:
{
  "message": "hello"
}

Backend:
      ↓
LLM API

Response:
{
  "answer": "..."
}
```

---

# 17. LLM Curriculum

Phải bao gồm mental model:

```text
Prompt
Messages
Context
Tokens
System Prompt
Temperature
Structured Output
Streaming
Tool Calling
```

Không cần đi sâu:

```text
Transformer mathematics
Attention equations
Training infrastructure
```

trừ khi được yêu cầu.

---

# 18. Data Pipeline Curriculum

Phải bắt đầu từ:

```text
Raw Data
   ↓
Load
   ↓
Clean
   ↓
Transform
   ↓
Store
   ↓
Retrieve
```

Sau đó mới nâng thành:

```text
Documents
   ↓
Extract
   ↓
Clean
   ↓
Chunk
   ↓
Metadata
   ↓
Embedding
   ↓
Vector Store
   ↓
Retrieve
   ↓
LLM
```

---

# 19. RAG Module

RAG phải được giải thích bằng mental model:

```text
User Question
      ↓
Find relevant information
      ↓
Put information into LLM context
      ↓
Generate answer
```

Sau đó mới giới thiệu:

```text
Embedding
Vector Search
Chunking
Top-K
Metadata Filtering
```

---

# 20. Capstone

## Default Capstone

Build:

> Personal Knowledge AI Chat Application

Architecture:

```text
User
 ↓
Frontend
 ↓
Backend
 ↓
LLM
 ↓
Retrieval
 ↓
Vector Store
 ↑
Data Pipeline
 ↑
Documents / APIs
```

Student phải có khả năng giải thích từng block.

Không chỉ demo app hoạt động.

---

# 21. Skill Workflow

Khi user đưa curriculum requirement mới:

```text
INPUT
  ↓
Extract goals
  ↓
Identify unknowns
  ↓
Research blockers
  ↓
Update Tech Radar
  ↓
Define student outcomes
  ↓
Build prerequisite graph
  ↓
Build curriculum map
  ↓
Generate modules
  ↓
Generate lessons
  ↓
Generate labs
  ↓
Generate assessment
  ↓
Coherence review
  ↓
Output curriculum
```

---

# 22. Research Gate

Skill bắt buộc research khi gặp:

```text
current tool
framework
library
AI model
agent framework
MCP
product
platform
SDK
```

Nếu công nghệ có khả năng thay đổi nhanh:

```text
Never rely solely on training knowledge.
```

Phải xác minh current status trước khi đưa vào curriculum.

---

# 23. Tool Selection Framework

Skill phải đánh giá tool theo:

```text
Educational Value
Technical Relevance
Abstraction Level
Stability
Maintenance
Learning Curve
Vendor Lock-in
Cost
Setup Complexity
Student Experience
Longevity
```

Không đơn giản chọn tool vì:

```text
nhiều stars
```

hoặc:

```text
đang trending
```

---

# 24. Output Structure

Skill tạo workspace:

```text
course/
│
├── README.md
│
├── COURSE_SPEC.md
├── LEARNING_OUTCOMES.md
├── CURRICULUM_MAP.md
├── PREREQUISITE_MAP.md
├── TECH_RADAR.md
├── DECISIONS.md
├── CAPSTONE.md
│
├── research/
│   ├── design-tools.md
│   ├── coding-agents.md
│   ├── backend-stack.md
│   ├── llm-stack.md
│   └── data-stack.md
│
└── lessons/
    │
    ├── 01-software-mental-model/
    │   ├── LESSON.md
    │   ├── LAB.md
    │   ├── TEACHER_NOTES.md
    │   └── ASSESSMENT.md
    │
    ├── 02-fe-be-api-db/
    │
    ├── 03-agentic-coding/
    │
    └── ...
```

---

# 25. COURSE_SPEC.md

Phải chứa:

```text
Course name
Audience
Prerequisites
Duration
Teaching format
Course objectives
Learning outcomes
Tools
Core concepts
Capstone
Assessment strategy
```

---

# 26. Module Specification

Mỗi module phải có:

```text
Module Name

Why this module exists

Prerequisites

Learning Outcomes

Concepts

Mental Models

Tools

Demo

Lessons

Labs

Assessment

Connection to Capstone
```

---

# 27. Lesson Specification

Mỗi `LESSON.md` phải có:

```text
Lesson Title

Duration

Prerequisites

Learning Objectives

Why students need this

Mental Model

Core Concepts

Instructor Explanation

Visual Explanation

Demo

Hands-on Lab

Common Mistakes

Check for Understanding

Assessment

Homework

Connection to Next Lesson
```

---

# 28. Lab Specification

Mỗi Lab phải có:

```text
Goal

Expected Output

Prerequisites

Tools

Step-by-step tasks

Success Criteria

Common Errors

Debugging Guide

Stretch Goal
```

---

# 29. Assessment

Assessment không tập trung vào syntax.

Phải đánh giá học viên có hiểu architecture không.

Ví dụ:

```text
Question:

When a user sends a message in your chatbot,
explain what happens from the browser
until the response is displayed.
```

Expected answer:

```text
Frontend
 ↓
HTTP request
 ↓
Backend
 ↓
LLM/API/Database
 ↓
Backend response
 ↓
Frontend render
```

---

# 30. Coherence Score

Skill phải đánh giá curriculum theo:

```text
Goal Alignment
Prerequisite Integrity
Difficulty Progression
Concept Coverage
Practicality
Tool Longevity
Project Integration
Assessment Quality
Non-Tech Accessibility
```

Có thể output:

```text
Curriculum Review

Critical Issues: 2
Warnings: 4
Suggestions: 7
```

Không cần numeric ranking bắt buộc.

---

# 31. Skill Internal Architecture

Logical roles:

```text
Curriculum Architect
        │
 ┌──────┼──────────┐
 │      │          │
 ▼      ▼          ▼
Researcher     Learning
             Designer
 │                 │
 └────────┬────────┘
          ▼
    Project Designer
          │
          ▼
   Coherence Reviewer
```

Các role có thể nằm trong một Skill duy nhất.

Không bắt buộc phải triển khai thành nhiều agent riêng.

---

# 32. Skill Directory

Recommended:

```text
vibe-code-curriculum-architect/
│
├── SKILL.md
│
├── references/
│   ├── curriculum-design.md
│   ├── pedagogy.md
│   ├── non-tech-teaching.md
│   ├── project-based-learning.md
│   ├── tool-selection.md
│   └── research-policy.md
│
├── templates/
│   ├── course-spec.md
│   ├── curriculum-map.md
│   ├── module.md
│   ├── lesson.md
│   ├── lab.md
│   ├── assessment.md
│   ├── tech-radar.md
│   └── adr.md
│
├── rubrics/
│   ├── curriculum-review.md
│   └── lesson-review.md
│
└── examples/
    └── vibe-coding/
```

---

# 33. Main SKILL.md Behaviour

Skill phải tự trigger khi user nói những câu như:

```text
Help me design a course.

Create curriculum.

Create lesson plan.

I want to teach X.

My curriculum is unclear.

Review this curriculum.

What should students learn before X?

Should I teach tool A or tool B?

Is this technology outdated?

Create a module for X.

Turn these topics into a course.
```

---

# 34. Example Interaction

User:

```text
Tôi muốn dạy Data Pipeline nhưng không biết
nên đặt nó trước hay sau database.
```

Skill:

```text
Data Pipeline requires students to understand:

- data
- basic persistence
- input/output
- APIs
- basic backend

Recommended sequence:

Database
   ↓
External APIs
   ↓
Data ingestion
   ↓
Transformation
   ↓
Data pipeline
```

Sau đó update:

```text
CURRICULUM_MAP.md
PREREQUISITE_MAP.md
```

---

# 35. Example Tool Decision

User:

```text
Nên dạy Stitch hay Lovable?
```

Skill phải:

1. Research current status
2. Compare role
3. Determine learning objective
4. Map tool to curriculum

Không chỉ trả lời:

```text
Stitch tốt hơn.
```

Mà:

```text
If objective = learn UI design workflow:
→ Stitch

If objective = rapidly generate full apps:
→ Lovable

For this curriculum:
Stitch fits Module: AI-Assisted Design.

Lovable fits later as an abstraction/comparison lesson.
```

---

# 36. Versioning

Curriculum phải có:

```text
CURRICULUM_VERSION
```

Ví dụ:

```text
v0.1
Initial architecture

v0.2
Added RAG

v0.3
Changed design tool

v1.0
First teaching-ready version
```

---

# 37. Tech Review

Mỗi tool phải có:

```text
Last verified
```

Ví dụ:

```text
Google Stitch
Last verified: 2026-10-01
```

Nếu quá một khoảng thời gian cấu hình trước:

```text
reverify
```

trước khi dùng lại recommendation.

---

# 38. Non-Goals

Skill không nhằm:

- thay thế LMS
- quản lý học viên
- chấm điểm tự động toàn khóa
- host khóa học
- tạo video
- tạo website course
- tạo full application automatically

Primary job:

> Design, research, maintain and refine the curriculum.

---

# 39. MVP

Version đầu tiên phải hỗ trợ:

```text
1. Accept rough course idea

2. Extract learning goals

3. Build dependency graph

4. Research uncertain technology decisions

5. Generate TECH_RADAR

6. Generate curriculum structure

7. Generate module specifications

8. Generate lesson plans

9. Generate labs

10. Generate capstone

11. Run curriculum coherence review
```

---

# 40. Phase 2

Future capabilities:

```text
Automatic slide generation

Teacher handbook

Student workbook

Quiz bank

Assignment generator

Rubric generator

Diagram generation

Course duration optimizer

Difficulty adaptation

Beginner / Intermediate tracks

Claude / Codex specific tracks
```

---

# 41. Success Criteria

Skill được xem là thành công khi một input thô như:

```text
Tôi muốn dạy người non-tech vibe code.

Cần FE, BE, API, DB, agent, MCP,
design, LLM, chatbot và data pipeline.

Tôi chưa biết sắp xếp thế nào.
```

có thể trở thành:

```text
Course Architecture
+
Dependency Graph
+
Tech Decisions
+
Modules
+
Lessons
+
Labs
+
Assessments
+
Capstone
+
Teacher Notes
```

mà curriculum:

- logic
- teachable
- project-driven
- dễ maintain
- không phụ thuộc quá mức vào một tool cụ thể
- có khả năng cập nhật khi ecosystem thay đổi.

---

# 42. Product Definition

Product cuối cùng không phải:

> AI Lesson Plan Generator.

Product cuối cùng là:

> AI Curriculum Architect for fast-moving technical education.

Với domain ban đầu:

> Vibe Coding for Non-Technical Learners.

Mục tiêu dài hạn:

```text
Ideas
+
Blockers
+
Current Technology
+
Pedagogy
        ↓
Centralize
        ↓
Research
        ↓
Structure
        ↓
Validate
        ↓
Crystallize
        ↓
Teaching-Ready Curriculum
```
