# Individual Problem Scan — Nguyễn Tấn Hoàng

> Phạm vi quan sát: quá trình nhận đề, clone repo và chuẩn bị bài Day 02 trong phiên làm bài hiện tại.
> Lưu ý về bằng chứng: các số đếm file/dòng bên dưới được kiểm tra trực tiếp trong repo. Những mốc thời gian mang nhãn **cần đo** là baseline dự kiến, chưa được coi là dữ liệu đã kiểm chứng.

## Phase 1 — Tìm 5+ problems

Tôi bắt đầu từ các thao tác và điểm vướng có thể quan sát trong workflow làm bài, thay vì bắt đầu từ một ý tưởng chatbot/agent.

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? (actor) | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi bắt đầu bài lab, học viên phải đối chiếu nhiều tài liệu để biết chính xác cần đọc gì, làm theo thứ tự nào và nộp file nào. | Học viên lần đầu làm Day 02 | Repo có 3 tài liệu chính với tổng cộng 1.305 dòng: `README.md` 112 dòng, `01-worksheet.md` 835 dòng và `02-deliverable-example.md` 358 dòng. |
| 2 | Lặp lại | Sau khi đọc worksheet, học viên phải chép lại từng heading/template cần thiết sang file báo cáo cá nhân trước khi có thể điền nội dung. | Học viên làm bài cá nhân | `01-individual-problem-scan/individual-report.md` ban đầu có kích thước 0 byte, trong khi template nằm rải trong worksheet. |
| 3 | Tốn thời gian + lặp lại | Trước khi commit, học viên phải tự rà xem bài đã đủ scan, top 3 cards và ba workflow trước/sau hay chưa. | Học viên chuẩn bị nộp bài | README yêu cầu 3 nhóm output trong phần cá nhân; repo chưa có checklist tự động kiểm tra các mục bắt buộc. Việc kiểm tra hiện là đọc lại thủ công. |
| 4 | AI có thể hỗ trợ tốt hơn | Khi ghi một candidate, học viên dễ dùng từ chung chung hoặc nhảy thẳng sang giải pháp, nhưng không có phản hồi tức thời về actor, workflow, bottleneck và metric còn thiếu. | Học viên đang viết Problem Card | Worksheet phải dành riêng checklist và prompt phản biện cho các lỗi này; mỗi card có 10 trường cần tự kiểm. |
| 5 | Lặp lại | Khi chuyển từ scan → card → workflow, cùng một actor, bottleneck và metric phải được nhập lại ở nhiều chỗ, dễ lệch số hoặc đổi phạm vi ngoài ý muốn. | Học viên làm Phase 1–2 | Một top problem xuất hiện trong bảng xếp hạng, Problem Card, current workflow và future workflow; top 3 tạo ít nhất 12 điểm thể hiện cần giữ nhất quán. |
| 6 | Khó khăn đến từ người khác | Bản nhóm do 3–4 người cùng làm nhưng cuối cùng mỗi người phải copy một bản vào repo cá nhân, dễ xảy ra tình trạng mỗi repo giữ một phiên bản khác nhau. | Thành viên nhóm và người tổng hợp bài | README quy định một bản nhóm rồi copy vào từng repo cá nhân; file `group-report.md` hiện chỉ có bảng thành viên trống và chưa chỉ ra nguồn bản cuối/version nào là chuẩn. |
| 7 | Tốn thời gian + AI có thể hỗ trợ tốt hơn | Ở phase research, học viên phải mở từng nguồn, tách claim hữu ích, ghi link và phân biệt dữ kiện đã xác minh với giả định; làm thủ công dễ bỏ nguồn tham chiếu. | Thành viên phụ trách validation/research | Worksheet yêu cầu kiểm link và không dùng số liệu không có nguồn; mẫu deliverable dùng bảng 6 cột cho từng nguồn/tool. |
| 8 | Khó khăn đến từ người khác + lặp lại | Quyết định và challenge của nhóm có thể nằm rải trong trao đổi miệng/chat, khiến người viết báo cáo phải hỏi lại “vì sao chọn/loại candidate này?”. | Người tổng hợp báo cáo nhóm và các thành viên | Group deliverable bắt buộc có convergence log, lý do chọn/không chọn và tín hiệu phản bác; repo ban đầu chưa có nơi ghi quyết định theo thời điểm. Baseline số lần hỏi lại: **cần đo trong buổi nhóm**. |

## Ghi chú bằng chứng

- Các problem trên phát sinh từ workflow của bài lab hiện tại và đều có actor cụ thể.
- #1, #2 và #3 có bằng chứng trực tiếp từ cấu trúc repo.
- #6 và #8 cần được xác nhận thêm khi bắt đầu làm việc nhóm.
- Chưa sử dụng số liệu thời gian chưa được đo như một dữ kiện thật.
