# Group Report — Day 02

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|-----|-----------|-------------|--------------------|
| 1   |           |             |                    |
| 2   |           |             |                    |
| 3   |           |             |                    |
| 4   |           |             |                    |
| 5   |           |             |                    |

## Candidate problem được nhóm chọn

Đọc report team dự án để đánh giá tiến độ làm việc và mức độ hoàn thành của team.

## Kiểm chứng vấn đề

Mục tiêu kiểm chứng: khó khăn này có thật không, ai gặp, bước nào đau nhất và có đáng giải quyết bằng AI/workflow không.

### Cách kiểm chứng nhanh

1. Hỏi nhanh 2-3 người từng quản lý, mentor hoặc theo dõi tiến độ team dự án.
2. Quan sát 1-2 report/cập nhật dự án gần nhất để xem format có thống nhất không.
3. Ghi lại thời gian ước lượng từ lúc mở report đến lúc có nhận định tiến độ.
4. Đếm số lần phải hỏi lại team vì report thiếu trạng thái, blocker hoặc next step.

### Câu hỏi interview ngắn

1. Lần gần nhất bạn phải đọc report/cập nhật của team để đánh giá tiến độ là khi nào?
2. Bạn đang đọc report theo workflow nào?
3. Bước nào mất thời gian hoặc khó chịu nhất?
4. Mỗi lần tổng hợp tiến độ bạn mất khoảng bao lâu?
5. Report thường thiếu thông tin gì: task done, task đang làm, blocker, deadline hay next step?
6. Nếu có một bản tóm tắt tự động, bạn muốn nó đưa ra những mục nào?

### Bảng ghi kết quả kiểm chứng

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | Dự kiến 3 người | Nếu nhiều người nói mất thời gian đọc nhiều update/report và phải tự tổng hợp trạng thái tiến độ. | Nếu team đã có dashboard/task board rõ ràng và hầu như không cần đọc report rời rạc. | Thu hẹp problem vào bối cảnh "report rời rạc, không cùng format, chưa có dashboard chuẩn". |
| Survey / poll | Dự kiến 5-10 người | Nếu đa số chọn mức độ đáng giải quyết 4-5/5 hoặc nói bước đau nhất là tổng hợp trạng thái/blocker. | Nếu đa số chỉ mất rất ít thời gian hoặc đã có template chung giải quyết được pain. | Điều chỉnh metric từ "giảm thời gian đọc report" sang "giảm số lần hỏi lại vì thiếu thông tin". |
| Log / review / ticket | 1-2 report gần nhất | Có nhiều report thiếu trạng thái rõ ràng, thiếu blocker/next step hoặc dùng format khác nhau. | Report đã đồng nhất, task có owner/status/deadline rõ, ít thông tin cần suy luận. | Nếu log cho thấy vấn đề chủ yếu do format, ưu tiên process/template trước khi dùng AI. |

### Kết luận tạm sau validation plan

Pain có khả năng tồn tại vì workflow hiện tại phụ thuộc nhiều vào việc đọc, hiểu ngữ cảnh và tự tổng hợp từ nhiều report. Tuy nhiên, chưa nên chốt số liệu impact cho đến khi có ít nhất 2-3 interview hoặc một mẫu report thật để đo thời gian.

Problem statement tạm sau kiểm chứng:

Người quản lý/mentor/team lead mất nhiều thời gian đọc và tổng hợp các report dự án rời rạc, không cùng format để biết team đang on track, blocked hay late, dẫn đến đánh giá tiến độ chậm và dễ bỏ sót vấn đề cần follow-up.

## Research giải pháp đã có

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Jira burndown/reporting | [Atlassian burndown charts](https://www.atlassian.com/agile/tutorials/burndown-charts) | Theo dõi work remaining, sprint/epic/release progress và phát hiện risk trong sprint. | Có biểu đồ tiến độ rõ, tốt khi task đã được cập nhật trong Jira và estimation có cấu trúc. | Không tự đọc report dạng văn bản rời rạc; không phản ánh đầy đủ chất lượng, ngữ cảnh hoặc lý do blocker nếu team không cập nhật task tốt. | Nếu team đã có task board chuẩn, nên kéo dữ liệu từ board trước; AI nên hỗ trợ giải thích và tóm tắt, không thay thế source of truth. |
| Asana status report template/status updates | [Asana status report template](https://asana.com/templates/status-report) | Chuẩn hóa báo cáo thành status, summary, accomplishments, blockers và next steps. | Giúp báo cáo dễ scan, giảm việc gom thông tin thủ công nếu team dùng chung một workspace. | Cần team nhập dữ liệu đúng format; nếu report nằm ở chat/doc riêng thì vẫn phải chuyển đổi thủ công. | Nên thiết kế output AI theo cấu trúc quen thuộc: health, done, in progress, blocker, risk, next step. |
| ClickUp AI project updates/summaries | [ClickUp project management](https://clickup.com/teams/project-management) | Tạo action items, tóm tắt discussion và pull updates để giữ team aligned. | Có hướng AI rõ ràng cho việc tóm tắt cập nhật và hành động tiếp theo trong workspace. | Phụ thuộc dữ liệu nằm trong ClickUp; rủi ro AI tóm tắt sai nếu context thiếu hoặc report nhập không đầy đủ. | AI hypothesis hợp lý nhất là agent/workflow có human review: AI draft summary, người quản lý kiểm tra rồi mới gửi feedback. |

### Bài học kéo về bài toán của nhóm

- Giải pháp không nên bắt đầu bằng chatbot chung chung; cần một workflow đọc report và xuất ra format tiến độ cố định.
- Non-AI baseline vẫn quan trọng: chuẩn hóa template report có thể giải quyết một phần lớn pain.
- AI phù hợp khi report là văn bản rời rạc, cần đọc hiểu ngữ cảnh, phân loại trạng thái và gợi ý câu hỏi follow-up.
- Boundary cần rõ: AI chỉ draft summary và highlight risk; người quản lý vẫn quyết định đánh giá cuối cùng.
- Metric nên đo được: thời gian tổng hợp report, số điểm thiếu thông tin được phát hiện, số lần phải hỏi lại team và độ chính xác của trạng thái task sau khi người quản lý review.
