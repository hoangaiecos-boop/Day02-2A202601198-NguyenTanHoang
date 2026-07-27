# Individual Reflection — Nguyễn Tấn Hoàng

## Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Scan 5 problems từ trải nghiệm học tập, dự án và theo dõi thông tin chương trình. | Có danh sách problem ban đầu với actor và dấu hiệu thật để chọn top 3. |
| Pitch Problem Card | Chọn và mô tả top 3 problems: đọc report team dự án, không theo kịp training, quên lịch workshop K20. | Nhóm có candidates đủ rõ để so sánh theo workflow, bottleneck và impact. |
| Challenge bài của bạn khác | Tự challenge các candidates bằng câu hỏi: actor có rõ không, workflow có vẽ được không, impact có đo được không. | Loại bớt hướng quá rộng hoặc có thể giải bằng rule đơn giản. |
| Gom trùng / cluster | Gom candidates thành các nhóm: báo cáo/tổng hợp thông tin, học tập/training, reminder/follow-up. | Nhóm nhìn ra pattern chung và dễ chọn candidate có workflow rõ nhất. |
| Chọn candidate problem | Đề xuất chọn problem đọc report team dự án. | Candidate được chọn vì có actor rõ, bottleneck cụ thể và có dữ liệu interview xác nhận pain. |
| Validation / research | Thực hiện quick interviews với Nguyễn Minh Hiếu, Hậu và Ngọc Mai; research Jira, Asana, ClickUp. | Có baseline thời gian 2-3 tiếng, 4-6 tiếng, có case vài ngày; nhóm sửa decision thành Go với scope nhỏ. |
| Workflow nhóm | Vẽ current workflow và future workflow theo hướng rule/template + AI draft + human review. | Nhóm thấy AI nên nằm ở bước tóm tắt/phân loại, không ôm toàn bộ quyết định. |
| Problem Statement | Viết Problem Statement v0/v1 với actor, workflow, bottleneck, impact, metric và boundary. | Problem Statement rõ hơn sau validation vì có baseline thời gian và success metric cụ thể. |
| Rule / Workflow / Agent | So sánh Rule, Workflow và Agent cho bài toán đọc report. | Nhóm chọn Workflow cho pilot vì đủ kiểm soát rủi ro và chưa cần Agent ngay. |
| Decision | Chốt Go với scope nhỏ, có pilot và rollback. | Quyết định dựa trên interview, research và boundary human review. |

## Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Nhờ AI hỗ trợ format bảng và làm rõ actor/dấu hiệu thật. | Giúp trình bày problem gọn và đúng template. | Ban đầu dễ viết hơi chung hoặc quá theo cấu trúc bài lab. | Giữ lại 5 problems xuất phát từ trải nghiệm thật của mình. |
| Problem Card | Dùng AI để chuyển top 3 thành Problem Cards đủ field. | Giúp không bỏ sót current workflow, bottleneck, metric, non-AI alternative. | AI có xu hướng chọn Agent hơi sớm cho problem đọc report. | Sau khi tham khảo example, hạ hướng nhóm về Workflow cho pilot. |
| Workflow | Dùng AI để vẽ draft workflow trước/sau bằng Mermaid/text. | Nhìn rõ bước nghẽn và human boundary. | Một số workflow ban đầu còn giống solution hơn là mô tả pain. | Tách rõ current workflow và future workflow, thêm fallback nếu AI sai. |
| Research | Dùng AI/search để tìm hướng Jira, Asana, ClickUp. | Có nguồn tham khảo và thấy các pattern đã có. | Không dùng số liệu tiết kiệm thời gian nếu không có nguồn hoặc validation thật. | Chỉ giữ nguồn/link và bài học liên quan trực tiếp đến problem nhóm. |
| Problem Statement | Dùng AI hỗ trợ kiểm field mơ hồ và viết lại v0/v1 theo template. | Giúp metric, boundary, AI intervention point rõ hơn. | Nếu thiếu dữ liệu thật, AI dễ viết metric chung chung. | Bổ sung baseline interview: 2-3 tiếng, 4-6 tiếng, vài ngày. |
| Rule / Workflow / Agent | Dùng AI hỗ trợ so sánh các mức giải pháp. | Giúp thấy Rule/Workflow/Agent khác nhau ở rủi ro và scope. | Ban đầu có xu hướng chọn Agent vì nghe mạnh hơn. | Chọn Workflow vì phù hợp pilot nhỏ và có human review. |
| Decision | Dùng AI hỗ trợ trình bày Go/Not Yet/No-Go, pilot và rollback. | Giúp decision rõ điều kiện, scope và rủi ro. | Khi chưa nhập interview, decision từng là Not Yet. | Sau validation thật, đổi thành Go với scope nhỏ. |

## Reflection câu hỏi mở

Reflection:

```text
Tôi học được rằng một problem tốt không phải là problem nghe có vẻ "AI" nhất, mà là problem có actor rõ, workflow vẽ được, bottleneck cụ thể và metric đo được. Ban đầu tôi có xu hướng nghĩ bài đọc report team dự án nên dùng Agent vì có nhiều report và cần phân tích. Sau khi xem lại worksheet và deliverable example, tôi thấy hướng Workflow hợp lý hơn cho pilot: chuẩn hóa input bằng rule/template, dùng AI để tóm tắt và phân loại, sau đó người quản lý vẫn review.

Phần validation làm tôi thay đổi cách nhìn bài toán. Trước đó tôi chỉ biết đây là pain cá nhân, nhưng sau khi hỏi Nguyễn Minh Hiếu, Hậu và Ngọc Mai, tôi thấy pain này thật sự lặp lại trong các bài tập lớn/dự án nhóm. Thời gian 2-3 tiếng, 4-6 tiếng, thậm chí vài ngày khiến impact rõ hơn nhiều so với câu "mất thời gian" chung chung.

Điều khó nhất khi viết Problem Statement là giữ nó không trượt sang solution-first. Nếu viết "xây AI đọc report" quá sớm thì dễ bỏ qua workflow thật và non-AI alternative. Tôi đã phải đưa boundary vào rõ hơn: AI không tự đánh giá hiệu suất cá nhân, không tự gửi feedback và không bịa status nếu report thiếu nguồn.

Nếu làm lại, tôi sẽ validate sớm hơn và hỏi thêm câu về format report thật: report thường thiếu field nào, có owner/deadline/blocker không, và người review thường phải hỏi lại bao nhiêu lần. Tôi cũng sẽ challenge nhóm mạnh hơn ở điểm: liệu chỉ cần template/report dashboard đã đủ chưa trước khi dùng AI.
```

## Tự kiểm cuối bài

- [x] [12đ cá nhân] Cá nhân có 5+ problems và top 3 Problem Cards.
- [x] [12đ cá nhân] Tôi đã pitch rõ và challenge nhóm đúng trọng tâm.
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài.
- [x] [15đ nhóm] Nhóm có workflow trước/sau.
- [x] [20đ nhóm] Nhóm có Problem Statement v0/v1 với metric và boundary rõ.
- [x] [15đ nhóm] Nhóm có so sánh No AI / Rule / Workflow / Agent.
- [x] [10đ nhóm] Nhóm có Go / Not Yet / No-Go và lý do rõ.
- [x] [10đ cá nhân] Reflection cá nhân có nói rõ vai trò trong nhóm, cách dùng AI, điều học được và nếu làm lại sẽ đổi gì.
- [x] [6đ cá nhân] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp với AI.
