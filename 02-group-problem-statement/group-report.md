# Group Report — Day 02

Case nhóm chọn: **Đọc report team dự án trước và sau AI**

Nhóm đang phân tích bài toán người quản lý/mentor phải đọc nhiều report của team dự án để đánh giá tiến độ làm việc và mức độ hoàn thành. Mục tiêu của bản này là đi từ candidates ban đầu → chọn candidate problem → kiểm chứng nhanh → research giải pháp → workflow trước/sau → Problem Statement v0/v1 → quyết định Rule / Workflow / Agent.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|-----|-----------|-------------|--------------------|
| 1 | Nguyễn Tấn Hoàng | 2A202601198 | Đưa candidate, validation/research, workflow, Problem Statement |
| 2 |  |  |  |
| 3 |  |  |  |
| 4 |  |  |  |
| 5 |  |  |  |

---

# Phase 3 — Group convergence

## Trình bày candidates

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
|---:|---|---|---|---|---|
| 1 | Nguyễn Tấn Hoàng | Tốn nhiều thời gian đọc report của team dự án để đánh giá tiến độ làm việc và hoàn thành của team | Người quản lý/mentor/team lead | Đọc nhiều report rời rạc, không cùng format, phải tự tổng hợp trạng thái task | Workflow rõ, impact có thể đo |
| 2 | Nguyễn Tấn Hoàng | Chưa hiểu và không theo kịp chương trình training | Học viên tham gia training | Tự hệ thống lại kiến thức sau buổi học, không biết mình đang thiếu phần nào | Pain thật nhưng scope rộng |
| 3 | Nguyễn Tấn Hoàng | Quên các lịch workshop, sự kiện của chương trình học tập K20 | Học viên K20 | Lịch nằm rải rác ở nhiều kênh, không tự chuyển thành reminder cá nhân | Dễ giải bằng rule/calendar |

## Gom trùng / cluster

| Cluster | Candidate examples | Pattern chung |
|---|---|---|
| Báo cáo / tổng hợp thông tin | Đọc report team dự án | Gom nhiều nguồn thông tin rồi viết lại thành trạng thái dễ ra quyết định |
| Học tập / training | Không theo kịp training | Người học nhận nhiều nội dung mới và cần tự hệ thống lại |
| Reminder / follow-up | Quên lịch workshop K20 | Thông tin quan trọng bị phân tán, dễ bỏ sót nếu không có nhắc lại |

## Shortlist và score

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Đọc report team dự án | 5 | 5 | 3 | 4 | 4 | 5 | 4 | 30 |
| Quên lịch workshop/sự kiện K20 | 5 | 4 | 3 | 3 | 5 | 3 | 5 | 28 |
| Không theo kịp training | 5 | 3 | 3 | 3 | 3 | 4 | 4 | 25 |

Nhóm chọn: **Đọc report team dự án**.

Vì sao chọn:

- Actor cụ thể: người quản lý/mentor/team lead.
- Workflow hiện tại nhìn thấy rõ: nhận report → đọc từng report → tìm trạng thái → so với kế hoạch → hỏi lại nếu thiếu.
- Bottleneck rõ: đọc và tổng hợp report rời rạc, không cùng format.
- Impact có thể đo bằng thời gian tổng hợp, số lần phải hỏi lại, số task bị thiếu trạng thái.
- Có thể so sánh Rule / Workflow / Agent mà không bị quá rộng.

Vì sao không chọn các bài còn lại:

- **Không theo kịp training:** pain thật nhưng rộng, cần thu hẹp vào một buổi học, một dạng tài liệu hoặc một bài lab cụ thể.
- **Quên lịch workshop/sự kiện K20:** workflow rõ nhưng có thể xử lý bằng calendar/pin message/rule trước, chưa cần làm trọng tâm AI.

Nếu có disagreement:

```text
Nhóm dùng score để ép mỗi người nói rõ lý do. Candidate nào có actor, workflow, bottleneck và metric rõ hơn sẽ được ưu tiên, không chọn chỉ vì nghe "AI" hơn.
```

---

# Phase 4 — Quick validation + research giải pháp

## Quick validation

Trạng thái hiện tại: nhóm chưa có dữ liệu phỏng vấn thật đủ để chốt baseline. Vì vậy phần dưới được ghi theo đúng worksheet như một validation plan + tín hiệu cần thu, không bịa số liệu survey/interview.

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Quick interview | Cần hỏi 2-3 người quản lý/mentor/team lead | Họ phải đọc nhiều report/update thủ công; bước đau nhất là tổng hợp trạng thái, blocker, next step | Họ đã có dashboard/task board rõ và gần như không đọc report rời rạc | Thu hẹp problem vào "report rời rạc, không cùng format, chưa có dashboard chuẩn" |
| Micro survey / poll | Cần hỏi 5-10 người từng quản lý/làm project | Nhiều người đánh giá mức đáng giải quyết 4-5/5; hay phải hỏi lại vì thiếu status/blocker | Đa số nói chỉ cần template hoặc calendar/checklist là đủ | Điều chỉnh solution về template/process trước, AI chỉ hỗ trợ phần tóm tắt |
| Log / review / ticket | Cần xem 1-2 report gần nhất | Report thiếu owner/status/deadline/blocker hoặc mỗi người viết một kiểu | Report đã có field đầy đủ, task rõ owner/status/deadline | Nếu vấn đề chính là format, ưu tiên chuẩn hóa report trước khi dùng AI |

Insight tạm sau validation:

```text
Pain không nằm ở việc "đọc cho xong report". Pain nằm ở đoạn biến nhiều cập nhật rời rạc thành một bức tranh tiến độ đủ rõ: task nào done, task nào late, blocker nào cần xử lý, và câu hỏi follow-up nào cần gửi lại team.
```

## Research giải pháp

Nhóm tìm các hướng đã có sẵn để tránh tự nghĩ trong chân không.

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Jira burndown/reporting | [Atlassian burndown charts](https://www.atlassian.com/agile/tutorials/burndown-charts) | Theo dõi work remaining, sprint/epic/release progress và phát hiện risk trong sprint | Tốt khi task đã nằm trong Jira và được cập nhật đều | Không tự đọc report văn bản rời rạc; không thể hiện đủ ngữ cảnh blocker nếu team không cập nhật task tốt | Dashboard/rule đủ cho dữ liệu có cấu trúc, chưa đủ cho report tự do |
| Asana status report template | [Asana status report template](https://asana.com/templates/status-report) | Chuẩn hóa status, summary, accomplishments, blockers, next steps | Format dễ scan, giảm việc gom thông tin thủ công nếu team dùng chung workspace | Cần team nhập đúng format; nếu report nằm ở chat/doc riêng vẫn phải chuyển đổi | Output nên theo format cố định: health, done, in progress, blocker, risk, next step |
| ClickUp AI project updates/summaries | [ClickUp project management](https://clickup.com/teams/project-management) | Tóm tắt discussion, pull updates, tạo action items | Có pattern AI hỗ trợ cập nhật dự án và next action | Phụ thuộc dữ liệu nằm trong ClickUp; AI có thể tóm tắt sai nếu context thiếu | Hướng hợp lý là AI draft summary, người quản lý review trước khi gửi |

Research takeaway:

```text
Không nên nhảy ngay sang một agent tự đánh giá tiến độ hoàn toàn. Hướng hợp lý hơn là kết hợp: rule/template để chuẩn hóa input, workflow/AI để tóm tắt và phân loại, người quản lý review trước khi quyết định.
```

---

# Phase 5 — Workflow before/after + Problem Statement

## Current workflow

```text
CURRENT STATE — 8 bước, thời gian baseline chưa đo

[1 Team gửi report/cập nhật]
→ [2 Người quản lý mở từng report]
→ [3 Đọc nội dung từng report]
→ [4 Tìm task done / doing / blocked / late]
→ [5 So sánh với kế hoạch/deadline]
→ [6 Tổng hợp nhận định tiến độ]  <-- bottleneck
→ [7 Hỏi lại team nếu thiếu thông tin]
→ [8 Gửi feedback / quyết định follow-up]
```

| Bước | Actor | Input | Output | Thời gian/tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Thành viên team | Công việc đã làm, blocker, kế hoạch tiếp theo | Report/cập nhật dự án | Hằng ngày hoặc hằng tuần | Format có thể khác nhau |
| 2 | Người quản lý/mentor | Nhiều report rời rạc | Danh sách nội dung cần đọc | Mỗi lần review tiến độ | Dễ mất thời gian nếu report nằm nhiều nơi |
| 3 | Người quản lý/mentor | Nội dung report | Task done/in progress/blocked/late | Mỗi lần review | Cần hiểu ngữ cảnh |
| 4 | Người quản lý/mentor | Task status + kế hoạch | Nhận định on track/at risk/off track | Mỗi lần review | Phải tự so sánh deadline |
| 5 | Người quản lý/mentor | Điểm thiếu thông tin | Câu hỏi follow-up/feedback | Khi report thiếu rõ ràng | Dễ bỏ sót blocker |

Bottleneck chính:

```text
Tổng hợp thủ công nhiều report rời rạc để suy ra trạng thái thật của dự án.
```

## Future workflow

```text
FUTURE STATE — 7 bước, target thời gian cần đo sau baseline

[1 Team gửi report theo template tối thiểu] -- Rule
→ [2 Hệ thống kiểm field bắt buộc]          -- Rule
→ [3 AI chuẩn hóa report]                  -- Workflow step
→ [4 AI phân loại done/doing/blocked/late] -- Workflow step
→ [5 AI draft summary + follow-up]         -- Workflow step
→ [6 Người quản lý review + sửa]           -- Human boundary
→ [7 Gửi feedback / quyết định follow-up]

Fallback:
AI tóm tắt sai hoặc không đủ nguồn → người quản lý quay lại đọc report gốc.
```

Before/after impact:

| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| Tổng thời gian | Chưa đo | Giảm sau khi đo baseline | Không ghi số phút khi chưa có dữ liệu thật |
| Số bước | 8 | 7 | Giảm ít bước, nhưng giảm effort ở bước tổng hợp |
| Bước thủ công | 6 | 3 | Người quản lý vẫn review, sửa và quyết định |
| Bottleneck chính | Tổng hợp report | Review summary và kiểm tra điểm AI chưa chắc | Human boundary |
| Risk mới | Không có hallucination | AI có thể phân loại sai hoặc bỏ sót ngữ cảnh | Cần link về report gốc và review bắt buộc |

## Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Người quản lý/mentor/team lead cần theo dõi tiến độ dự án. |
| **Workflow** | Nhận report từ team, đọc từng report, tìm trạng thái task, so sánh với kế hoạch, tổng hợp nhận định, hỏi lại team nếu thiếu thông tin. |
| **Bottleneck** | Bước tổng hợp thủ công từ nhiều report rời rạc, không cùng format. |
| **Impact** | Review tiến độ chậm, dễ bỏ sót blocker/task trễ, feedback cho team thiếu kịp thời. |
| **Success Metric** | Giảm thời gian tổng hợp report so với baseline; giảm số lần phải hỏi lại vì thiếu status/blocker; tăng tỷ lệ task có trạng thái rõ sau review. |
| **Boundary** | AI không tự đánh giá hiệu suất cá nhân, không tự gửi feedback, không thay người quản lý quyết định tiến độ cuối cùng. |

---

# Phase 6 — Rule / Workflow / Agent + Decision

## So sánh Rule / Workflow / Agent

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | Template report bắt buộc field done/doing/blocker/next step/deadline | Đủ nếu team cập nhật đều và format chuẩn | Không xử lý tốt report tự do hoặc thiếu ngữ cảnh | Dùng cho input, không chọn làm toàn bộ |
| **Workflow** | Rule kiểm input → AI chuẩn hóa → AI phân loại → AI draft summary → người quản lý review | Đủ cho pilot vì các bước khá rõ và có human review | Draft có thể sai/nhạt, cần kiểm report gốc | Chọn cho pilot |
| **Agent** | Agent đọc nhiều nguồn, đối chiếu kế hoạch, tự hỏi thêm khi thiếu và draft follow-up | Chỉ cần khi nhiều nguồn dữ liệu, nhiều nhánh xử lý, cần tự quyết bước tiếp theo | Quá rộng nếu chưa có baseline/input ổn định | Chưa chọn ngay |

Mức chọn:

```text
Workflow.
```

Vì sao:

- Rule/template cần có để input sạch hơn.
- AI hữu ích nhất ở bước đọc hiểu, chuẩn hóa, phân loại và draft summary.
- Người quản lý vẫn review nên rủi ro kiểm soát được.
- Chưa cần Agent ngay vì chưa có dữ liệu thật, permission và baseline đủ rõ.

## Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Người quản lý/mentor/team lead cần theo dõi tiến độ dự án từ report của team. |
| **Workflow** | Team gửi report → kiểm field bắt buộc → AI chuẩn hóa/phân loại → AI draft summary và câu hỏi follow-up → người quản lý review → gửi feedback. |
| **Bottleneck** | Tổng hợp thủ công nhiều report rời rạc, không cùng format để biết dự án đang on track, blocked hay late. |
| **Impact** | Review tiến độ chậm, dễ bỏ sót blocker/task trễ, feedback cho team thiếu kịp thời. |
| **Success Metric** | Sau pilot: giảm thời gian tổng hợp report so với baseline; tăng tỷ lệ task có trạng thái rõ; giảm số lần hỏi lại vì report thiếu thông tin. |
| **Boundary** | AI không tự gửi feedback, không đánh giá hiệu suất cá nhân, không bịa status nếu report thiếu nguồn; người quản lý kiểm report gốc trước khi dùng output. |
| **AI intervention point** | Sau khi report được thu thập và trước khi người quản lý viết nhận định tiến độ. |
| **Mức chọn** | Workflow: rule/template cho input, AI draft summary, người quản lý review. |
| **Rủi ro & người thật kiểm tra** | Risk: AI tóm tắt sai, bỏ sót blocker, suy luận quá mức. Người kiểm tra: người quản lý/mentor review trước khi gửi feedback hoặc quyết định follow-up. |

## Final decision

Decision:

```text
Not Yet — cần validate trước khi Go.
```

Pilot nhỏ nhất nếu đủ validation:

- Chọn 1 team hoặc 1 project nhỏ.
- Dùng 1 tuần report gần nhất.
- Người quản lý đo thời gian tổng hợp thủ công làm baseline.
- Chạy workflow bán thủ công: paste report vào prompt/template chuẩn.
- AI tạo summary theo format: health, done, in progress, blocked, risk, next step.
- Người quản lý đo thời gian review và số lỗi phải sửa.

Exit / rollback:

- Nếu AI bỏ sót blocker quan trọng hoặc bịa trạng thái task, không dùng output trực tiếp.
- Nếu người quản lý vẫn phải viết lại phần lớn summary, hạ xuống template report + dashboard.
- Nếu vấn đề chính là team không cập nhật report đầy đủ, ưu tiên process/template trước AI.

Decision rationale:

- Problem rõ và workflow rõ.
- Metric đã có hướng đo nhưng chưa có baseline thật.
- Có non-AI components quan trọng.
- AI nằm ở một bước cụ thể, không ôm toàn bộ workflow.
- Human review rõ nên rủi ro chấp nhận được cho pilot nhỏ.
