# Group Report — Day 02

Case nhóm chọn: **Đọc report team dự án trước và sau AI**

Nhóm đang phân tích bài toán người quản lý/mentor phải đọc nhiều report của team dự án để đánh giá tiến độ làm việc và mức độ hoàn thành. Mục tiêu của bản này là đi từ candidates ban đầu → chọn candidate problem → kiểm chứng nhanh → research giải pháp → workflow trước/sau → Problem Statement v0/v1 → quyết định Rule / Workflow / Agent.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|-----|-----------|-------------|--------------------|
| 1 | Nguyễn Tấn Hoàng | 2A202601198 | Thành viên |
| 2 | Bùi Công Hậu | 2A202601877 | Thành viên |
| 3 | Nguyễn Minh Hiếu | 2A202601154 | Thành viên |
| 4 | Nguyễn Trương Ngọc Mai | 2A202601652 | Thành viên |
| 5 | Nguyễn Trần Gia Phụng | 2A202601286 | Thành viên |

---

# Phase 3 — Group convergence

## Trình bày candidates

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
|---:|---|---|---|---|---|
| 1 | Nguyễn Tấn Hoàng | Tốn nhiều thời gian đọc report của team dự án để đánh giá tiến độ làm việc và hoàn thành của team | Người quản lý/mentor/team lead | Đọc nhiều report rời rạc, không cùng format, phải tự tổng hợp trạng thái task | Workflow rõ, impact có thể đo |
| 2 | Nguyễn Tấn Hoàng | Chưa hiểu và không theo kịp chương trình training | Học viên tham gia training | Tự hệ thống lại kiến thức sau buổi học, không biết mình đang thiếu phần nào | Pain thật nhưng scope rộng |
| 3 | Nguyễn Tấn Hoàng | Quên các lịch workshop, sự kiện của chương trình học tập K20 | Học viên K20 | Lịch nằm rải rác ở nhiều kênh, không tự chuyển thành reminder cá nhân | Dễ giải bằng rule/calendar |
| 4 | Bùi Công Hậu | Giải mã tài liệu kỹ thuật | Người học/nghiên cứu đọc paper kỹ thuật | Tài liệu nhảy bước toán học, phải tự suy diễn hoặc tra thêm nguồn | Workflow rõ; AI giải thích/verify derivation có thể hỗ trợ mạnh |
| 5 | Bùi Công Hậu | Chuẩn bị hồ sơ ứng tuyển CV/email | Người ứng tuyển/học viên | Viết bản nháp đầu dễ generic, phải đối chiếu JD với kinh nghiệm cá nhân | Có deadline và impact trực tiếp nhưng metric kết quả chậm |
| 6 | Bùi Công Hậu | Format báo cáo/slide học thuật | Sinh viên làm báo cáo/slide | Vòng lặp compile/sửa format/căn chỉnh chiếm nhiều thời gian | Rule/Workflow phù hợp, automation cao |
| 7 | Nguyễn Minh Hiếu | Giải mã tài liệu kỹ thuật | Sinh viên, researcher, developer | Đọc chậm, khó hiểu bản chất toán/thuật toán phức tạp | Use-case AI mạnh nhưng cần tránh "hiểu giả" |
| 8 | Nguyễn Minh Hiếu | Tối ưu CV và email ứng tuyển theo job | Người đi thực tập/ứng tuyển | Phải sửa thủ công từng CV/email cho mỗi công ty | Pain rõ, có deadline, dễ bị generic nếu thiếu context |
| 9 | Nguyễn Minh Hiếu | Định dạng báo cáo và slide học thuật | Sinh viên, nghiên cứu sinh | Tốn thời gian chỉnh căn lề, font, citation thay vì nội dung | Tự động hóa cao nhưng cần giữ ranh giới không làm hộ nội dung |
| 10 | Nguyễn Trương Ngọc Mai | Mất thời gian truy vết hành trình đối tượng qua nhiều camera | Bảo vệ, vận hành camera, ban quản lý | Tua thủ công từng video, ghép nối rời rạc giữa nhiều góc quay | Workflow rõ, pain lớn, đo được bằng thời gian xử lý |
| 11 | Nguyễn Trương Ngọc Mai | Tìm kiếm đối tượng bằng câu lệnh mô tả tự nhiên quá chậm | Đội điều tra, nhân viên trích xuất camera | Nhìn bằng mắt thường từng khung hình để xem có khớp mô tả hay không | Multimodal AI phù hợp nhưng cần đo độ chính xác matching |
| 12 | Nguyễn Trương Ngọc Mai | Bỏ sót sự cố do phải soi màn hình 24/7 chờ hành vi bất thường | Bảo vệ ca trực, đội trưởng an ninh | Mỏi mắt, giảm tập trung khi phải chờ sự cố hiếm | Impact lớn nhưng vướng hạ tầng real-time và cảnh báo giả |
| 13 | Nguyễn Trần Gia Phụng | Khó chọn trang phục phù hợp với thời tiết, địa điểm và tủ đồ | Người chuẩn bị đi làm, đi chơi, dự sự kiện | Khó nhớ toàn bộ tủ đồ và cân nhắc thời tiết, màu sắc, hoàn cảnh | Workflow rõ nhưng taste cá nhân khó đo |
| 14 | Nguyễn Trần Gia Phụng | Trước kỳ thi không biết nên ôn phần nào vì thông tin rải rác nhiều nguồn | Sinh viên chuẩn bị thi | Phải đọc/so sánh slide, giáo trình, bài tập; thông tin trùng hoặc mâu thuẫn | Workflow rõ, mất 2-4 giờ/môn, input tài liệu đa dạng |
| 15 | Nguyễn Trần Gia Phụng | Kiểm tra báo cáo thủ công nhiều lần trước khi nộp | Sinh viên viết báo cáo, đồ án, paper | Lỗi chính tả, đánh số, mâu thuẫn nằm rải rác; sửa một chỗ có thể sai chỗ khác | Rule + Workflow phù hợp, có thể đo giảm thời gian kiểm tra |

## Gom trùng / cluster

| Cluster | Candidate examples | Pattern chung |
|---|---|---|
| Báo cáo / tổng hợp / kiểm tra tài liệu | Đọc report team dự án; format báo cáo/slide; kiểm tra báo cáo trước khi nộp | Gom, chuẩn hóa hoặc kiểm tra nhiều nội dung rời rạc để tạo output đủ dùng |
| Học tập / nghiên cứu | Không theo kịp training; giải mã tài liệu kỹ thuật; ôn thi từ nhiều nguồn | Người học phải tự hệ thống kiến thức từ nhiều tài liệu, dễ thiếu hoặc hiểu sai |
| Reminder / cá nhân hóa quyết định | Quên lịch workshop; chọn trang phục; chuẩn bị CV/email | Cần nhắc đúng lúc hoặc cá nhân hóa theo ngữ cảnh |
| Camera / an ninh / truy vết | Truy vết hành trình qua nhiều camera; tìm đối tượng bằng mô tả; phát hiện sự cố 24/7 | Dữ liệu hình ảnh/video lớn, cần tìm kiếm hoặc phát hiện nhanh |

## Shortlist và score

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Đọc report team dự án | 5 | 5 | 4 | 5 | 4 | 5 | 5 | 33 |
| Kiểm tra báo cáo trước khi nộp | 5 | 5 | 3 | 4 | 5 | 5 | 4 | 31 |
| Trước kỳ thi không biết nên ôn phần nào | 5 | 4 | 3 | 4 | 4 | 5 | 4 | 29 |
| Truy vết hành trình qua nhiều camera | 5 | 5 | 3 | 5 | 2 | 5 | 3 | 28 |
| Quên lịch workshop/sự kiện K20 | 5 | 4 | 3 | 3 | 5 | 3 | 5 | 28 |

Nhóm chọn: **Đọc report team dự án**.

Vì sao chọn:

- Actor cụ thể: người quản lý/mentor/team lead.
- Workflow hiện tại nhìn thấy rõ: nhận report → đọc từng report → tìm trạng thái → so với kế hoạch → hỏi lại nếu thiếu.
- Bottleneck rõ: đọc và tổng hợp report rời rạc, không cùng format.
- Impact có thể đo bằng thời gian tổng hợp, số lần phải hỏi lại, số task bị thiếu trạng thái.
- Có thể so sánh Rule / Workflow / Agent mà không bị quá rộng.

Vì sao không chọn các bài còn lại:

- **Camera/an ninh:** impact lớn nhưng scope kỹ thuật rộng, cần dữ liệu video, hạ tầng real-time và metric độ chính xác phức tạp hơn thời lượng lab.
- **Học tập/nghiên cứu:** pain thật nhưng quality metric khó hơn, dễ tạo cảm giác "hiểu giả" nếu chưa có bài test/verification rõ.
- **Format/kiểm tra báo cáo:** workflow rõ và gần với bài được chọn, nhưng thiên về rule/template hơn; nhóm muốn đào sâu bài có yếu tố tổng hợp nhận định và feedback.
- **Reminder/cá nhân hóa:** một số bài có thể xử lý bằng calendar, checklist hoặc rule đơn giản trước khi cần AI.

Nếu có disagreement:

```text
Nhóm dùng score để ép mỗi người nói rõ lý do. Candidate nào có actor, workflow, bottleneck và metric rõ hơn sẽ được ưu tiên, không chọn chỉ vì nghe "AI" hơn.
```

---

# Phase 4 — Quick validation + research giải pháp

## Quick validation

Nhóm dùng **Option A — Quick interviews** và hỏi nhanh 3 người từng phải đọc/tổng hợp report trong dự án hoặc bài tập lớn nhóm.

| Người trả lời | Lần gần nhất gặp vấn đề | Workflow hiện tại | Bước đau nhất | Thời gian | Mong muốn nếu tốt hơn |
|---|---|---|---|---|---|
| Nguyễn Minh Hiếu | Đọc report BTL restaurant management | Mở raw report của từng thành viên → đọc, phân tích và nhận xét từng report → tổng hợp ưu/nhược điểm report từng thành viên → ghi feedback → trao đổi với team | Đọc, phân tích và nhận xét từng report | 4-6 tiếng | AI tổng hợp report theo một format chung cố định để rút ngắn thời gian khoảng 4-5 lần |
| Hậu | Dự án môn học nhóm gồm 5 thành viên | Tạo 1 file chung để mọi người viết báo cáo → cho chatbot review → đọc và nhận xét báo cáo từng người → chỉnh sửa nội dung chưa hợp lý → hỏi lại lỗi sai | Đọc nội dung báo cáo của từng người | 2-3 tiếng | Thay đổi cách đọc báo cáo từng người vì rất mất thời gian |
| Ngọc Mai | Đọc báo cáo BTL môn học trên trường | Đọc thủ công nhiều báo cáo không đồng format → đối chiếu deadline → tự tổng hợp nhận định → ghi chú và hỏi lại team | Đọc và tổng hợp thủ công từng báo cáo | Vài ngày | Giảm thời gian tổng hợp và hệ thống tự gợi ý câu hỏi |

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Quick interview | 3 người | Cả 3 đều gặp pain khi đọc/tổng hợp report thủ công; thời gian dao động từ 2-3 tiếng, 4-6 tiếng đến vài ngày; bước đau nhất đều là đọc/phân tích/tổng hợp report | Chưa có phản bác mạnh; Hậu đã thử dùng chatbot review nhưng vẫn phải đọc và sửa nhiều | Thu hẹp problem vào "đọc và tổng hợp nhiều report không đồng format để tạo nhận định/feedback nhanh hơn" |
| Micro survey / poll | Chưa làm | Có thể dùng thêm nếu cần kiểm tra pain trên nhiều người hơn | Chưa có dữ liệu | Không dùng để chốt số liệu hiện tại |
| Log / review / ticket | Chưa thu report thật | Interview cho thấy report thường không đồng format và cần đối chiếu deadline/feedback | Chưa có mẫu report để kiểm tra lỗi cụ thể | Cần thu 1-2 report thật trước pilot để kiểm prompt và format output |

Insight sau validation:

```text
Pain thật và lặp lại ở nhiều bối cảnh bài tập lớn/dự án nhóm. Pain không chỉ là "đọc cho xong report", mà là đọc nhiều report không đồng format, phân tích từng phần, tổng hợp nhận định/feedback và hỏi lại khi thiếu thông tin. Baseline hiện có khá nặng: nhanh nhất 2-3 tiếng, có case 4-6 tiếng, và có case mất vài ngày.
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
CURRENT STATE — 8 bước, baseline interview: 2-3 tiếng đến vài ngày

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
| Tổng thời gian | 2-3 tiếng, 4-6 tiếng, có case vài ngày | Giảm 4-5 lần hoặc về dưới 1 giờ cho vòng review đầu | Dựa trên 3 quick interviews |
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
| **Impact** | Review tiến độ mất từ 2-3 tiếng đến 4-6 tiếng, có case kéo dài vài ngày; dễ bỏ sót blocker/task trễ; feedback cho team thiếu kịp thời. |
| **Success Metric** | Giảm thời gian tổng hợp report 4-5 lần hoặc về dưới 1 giờ cho vòng review đầu; giảm số lần phải hỏi lại vì thiếu status/blocker; tăng tỷ lệ task có trạng thái rõ sau review. |
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
- Chưa cần Agent ngay vì đã có tín hiệu pain và baseline từ interview, nhưng chưa có report mẫu, quyền truy cập nguồn dữ liệu và boundary vận hành đủ rõ.

## Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Người quản lý/mentor/team lead cần theo dõi tiến độ dự án từ report của team. |
| **Workflow** | Team gửi report → kiểm field bắt buộc → AI chuẩn hóa/phân loại → AI draft summary và câu hỏi follow-up → người quản lý review → gửi feedback. |
| **Bottleneck** | Tổng hợp thủ công nhiều report rời rạc, không cùng format để biết dự án đang on track, blocked hay late. |
| **Impact** | Review tiến độ tốn 2-3 tiếng đến 4-6 tiếng, có trường hợp kéo dài vài ngày; dễ bỏ sót blocker/task trễ, feedback cho team thiếu kịp thời. |
| **Success Metric** | Sau pilot: giảm thời gian tổng hợp 4-5 lần hoặc về dưới 1 giờ cho vòng review đầu; tăng tỷ lệ task có trạng thái rõ; giảm số lần hỏi lại vì report thiếu thông tin. |
| **Boundary** | AI không tự gửi feedback, không đánh giá hiệu suất cá nhân, không bịa status nếu report thiếu nguồn; người quản lý kiểm report gốc trước khi dùng output. |
| **AI intervention point** | Sau khi report được thu thập và trước khi người quản lý viết nhận định tiến độ. |
| **Mức chọn** | Workflow: rule/template cho input, AI draft summary, người quản lý review. |
| **Rủi ro & người thật kiểm tra** | Risk: AI tóm tắt sai, bỏ sót blocker, suy luận quá mức. Người kiểm tra: người quản lý/mentor review trước khi gửi feedback hoặc quyết định follow-up. |

## Final decision

Decision:

```text
Go với scope nhỏ.
```

Pilot nhỏ nhất:

- Chọn 1 team hoặc 1 project nhỏ.
- Dùng report của một bài tập lớn/dự án nhóm gần nhất.
- Dùng baseline từ interview: 2-3 tiếng, 4-6 tiếng, vài ngày; đo thêm thời gian thực tế khi chạy pilot.
- Chạy workflow bán thủ công: paste report vào prompt/template chuẩn.
- AI tạo summary theo format: health, done, in progress, blocked, risk, next step.
- Người quản lý đo thời gian review và số lỗi phải sửa.

Exit / rollback:

- Nếu AI bỏ sót blocker quan trọng hoặc bịa trạng thái task, không dùng output trực tiếp.
- Nếu người quản lý vẫn phải viết lại phần lớn summary, hạ xuống template report + dashboard.
- Nếu vấn đề chính là team không cập nhật report đầy đủ, ưu tiên process/template trước AI.

Decision rationale:

- Problem rõ và workflow rõ.
- Đã có quick interviews xác nhận pain với baseline thời gian cụ thể.
- Có non-AI components quan trọng.
- AI nằm ở một bước cụ thể, không ôm toàn bộ workflow.
- Human review rõ nên rủi ro chấp nhận được cho pilot nhỏ.
