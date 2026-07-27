# Individual Problem Scan — Nguyễn Tấn Hoàng

> Phạm vi quan sát: quá trình nhận đề, clone repo và chuẩn bị bài Day 02 trong phiên làm bài hiện tại.
> Lưu ý về bằng chứng: các số đếm file/dòng bên dưới được kiểm tra trực tiếp trong repo. Những mốc thời gian mang nhãn **cần đo** là baseline dự kiến, chưa được coi là dữ liệu đã kiểm chứng.

## Phase 1 — Scan rộng

Tôi bắt đầu từ các thao tác và điểm vướng có thể quan sát trong chính workflow làm bài, thay vì bắt đầu từ một ý tưởng chatbot/agent.

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? (actor) | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi bắt đầu bài lab, học viên phải đối chiếu nhiều tài liệu để biết chính xác cần đọc gì, làm theo thứ tự nào và nộp file nào. | Học viên lần đầu làm Day 02 | Repo có 3 tài liệu chính với tổng cộng 1.305 dòng: `README.md` 112 dòng, `01-worksheet.md` 835 dòng và `02-deliverable-example.md` 358 dòng. |
| 2 | Lặp lại | Sau khi đọc worksheet, học viên phải chép lại từng heading/template cần thiết sang file báo cáo cá nhân trước khi có thể điền nội dung. | Học viên làm bài cá nhân | `01-individual-problem-scan/individual-report.md` ban đầu có kích thước 0 byte, trong khi template nằm rải trong worksheet. |
| 3 | Tốn thời gian + lặp lại | Trước khi commit, học viên phải tự rà xem bài đã đủ scan, top 3 cards và ba workflow trước/sau hay chưa. | Học viên chuẩn bị nộp bài | README yêu cầu 3 nhóm output trong phần cá nhân; repo chưa có checklist tự động kiểm tra các mục bắt buộc. Việc kiểm tra hiện là đọc lại thủ công. |
| 4 | AI có thể hỗ trợ tốt hơn | Khi ghi một candidate, học viên dễ dùng từ chung chung hoặc nhảy thẳng sang giải pháp, nhưng không có phản hồi tức thời về actor, workflow, bottleneck và metric còn thiếu. | Học viên đang viết Problem Card | Worksheet phải dành riêng checklist và prompt phản biện cho các lỗi này; mỗi card có 10 trường cần tự kiểm. |
| 5 | Lặp lại | Khi chuyển từ scan → card → workflow, cùng một actor, bottleneck và metric phải được nhập lại ở nhiều chỗ, dễ lệch số hoặc đổi phạm vi ngoài ý muốn. | Học viên làm Phase 1–2 | Một top problem xuất hiện trong bảng xếp hạng, Problem Card, current workflow và future workflow; top 3 tạo ít nhất 12 điểm thể hiện cần giữ nhất quán. |
| 6 | Khó khăn đến từ người khác | Bản nhóm do 3–4 người cùng làm nhưng cuối cùng mỗi người phải copy một bản vào repo cá nhân, dễ xảy ra tình trạng mỗi repo giữ một phiên bản khác nhau. | Thành viên nhóm và người tổng hợp bài | README quy định một bản nhóm rồi copy vào từng repo cá nhân; file `group-report.md` hiện chỉ có bảng thành viên trống và chưa chỉ ra nguồn bản cuối/version nào là chuẩn. |
| 7 | Tốn thời gian + AI có thể hỗ trợ tốt hơn | Ở phase research, học viên phải mở từng nguồn, tách claim hữu ích, ghi link và phân biệt dữ kiện đã xác minh với giả định; làm thủ công dễ bỏ provenance. | Thành viên phụ trách validation/research | Worksheet yêu cầu kiểm link và không dùng số liệu không có nguồn; mẫu deliverable dùng bảng 6 cột cho từng nguồn/tool. |
| 8 | Khó khăn đến từ người khác + lặp lại | Quyết định và challenge của nhóm có thể nằm rải trong trao đổi miệng/chat, khiến người viết báo cáo phải hỏi lại “vì sao chọn/loại candidate này?”. | Người tổng hợp báo cáo nhóm và các thành viên | Group deliverable bắt buộc có convergence log, lý do chọn/không chọn và tín hiệu phản bác; repo ban đầu chưa có nơi ghi quyết định theo thời điểm. Baseline số lần hỏi lại: **cần đo trong buổi nhóm**. |

### Nhận xét sau scan

- Các pain trên đều phát sinh từ workflow thật của bài lab hiện tại và có actor cụ thể.
- #1, #2 và #3 có bằng chứng trực tiếp mạnh nhất vì có thể kiểm tra ngay từ cấu trúc repo.
- #6 và #8 có khả năng ảnh hưởng nhiều người hơn, nhưng chỉ nên giữ là candidate cho đến khi quan sát buổi làm nhóm.
- Tôi chưa dùng các con số về “phút tiết kiệm” như dữ kiện thật. Baseline thời gian cần được bấm giờ trong lần thực hiện tiếp theo.

## Phase 2 — Chọn top 3 candidate problems

Đây mới là bước chọn **candidate problem** để pitch. Chưa candidate nào được xem là Problem Statement.

| Rank | Candidate problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Rà soát độ đầy đủ và nhất quán của bài nộp cá nhân | Actor rõ; workflow xảy ra với mọi học viên; input là Markdown nên dễ đo số lỗi thiếu/sai; scope vừa một buổi lab. | Baseline hiện có bao nhiêu lỗi thiếu hoặc lệch sau lần viết đầu tiên. |
| 2 | Giữ một phiên bản chuẩn của báo cáo nhóm khi copy sang repo cá nhân | Tác động tới 3–4 người; handoff và rủi ro version rõ; có thể so sánh process fix, rule và workflow. | Nhóm thực tế dùng GitHub, Google Docs hay chat làm nơi cộng tác. |
| 3 | Ghi lại convergence decision và challenge của nhóm | Giúp giải thích quyết định cuối bằng evidence; tránh hỏi lại; có thể đo mức đầy đủ của decision log. | Tần suất bỏ sót quyết định trong buổi nhóm và liệu template đơn giản đã đủ hay chưa. |

## Problem Card #1 — Rà soát bài nộp cá nhân

**Problem 1 câu:**
Khi chuẩn bị commit bài Day 02, học viên phải đọc lại nhiều tài liệu và đối chiếu thủ công để phát hiện phần còn thiếu hoặc thông tin không nhất quán giữa scan, cards và workflows.

**Actor:**
Học viên chịu trách nhiệm hoàn thiện và nộp repo cá nhân Day 02.

**Thời điểm / bối cảnh:**
Sau khi viết bản nháp và trước mỗi lần commit/push bài.

**Current workflow:**

1. Mở README để nhớ cấu trúc nộp.
2. Mở worksheet để tìm các field bắt buộc.
3. Mở bài mẫu để so hình thức đầu ra.
4. Đọc lại báo cáo cá nhân từ đầu đến cuối.
5. So actor, bottleneck và metric giữa card với workflow.
6. Bổ sung phần thiếu rồi kiểm tra lại.

**Bottleneck:**
Bước 4–5: đối chiếu bằng mắt giữa nhiều đoạn và nhiều file; thời gian mỗi lần **cần bấm giờ xác nhận**.

**Impact:**
Tốn công lặp lại trước mỗi lần nộp; một field bị thiếu hoặc một metric lệch có thể làm lập luận không nhất quán và mất điểm rubric.

**Success metric:**
Trong 3 lần kiểm tra thử, phát hiện 100% field bắt buộc bị thiếu trong bộ test; giảm số lỗi thiếu/không nhất quán còn 0 trước khi push. Chỉ đặt mục tiêu thời gian sau khi đo baseline thủ công.

**Non-AI alternative:**
Checklist Markdown hoặc script rule-based kiểm tra heading/field bắt buộc.

**AI hypothesis:**
AI có thể đọc ngữ nghĩa để cảnh báo actor, bottleneck hoặc metric mâu thuẫn dù heading vẫn đầy đủ; học viên quyết định sửa nội dung.

**Quick gut:**
- [ ] No AI / process fix
- [ ] Rule
- [x] Workflow
- [ ] Agent
- [ ] Chưa biết

### Draft workflow #1

```text
CURRENT STATE

[Mở 3 tài liệu hướng dẫn]
→ [Lập danh sách field]
→ [Đọc lại report]
→ [Đối chiếu card/workflow bằng mắt]  <-- bottleneck
→ [Sửa]
→ [Đọc lại lần nữa]

FUTURE STATE (giả thuyết cần kiểm chứng)

[Chạy checklist rule-based]
→ [Báo heading/field thiếu]
→ [AI review tính nhất quán ngữ nghĩa]
→ [Học viên xem từng cảnh báo]         <-- human boundary
→ [Học viên tự sửa và approve]

Fallback: AI nhận xét sai → bỏ cảnh báo; checklist rule-based vẫn hoạt động.
Không tự sửa nội dung và không tự push.
```

## Problem Card #2 — Đồng bộ bản báo cáo nhóm

**Problem 1 câu:**
Khi nhiều thành viên cùng hoàn thiện báo cáo nhóm rồi copy sang repo cá nhân, họ có thể nộp các phiên bản khác nhau mà không biết file nào là bản cuối.

**Actor:**
Nhóm 3–4 học viên; đặc biệt là người tổng hợp và người copy bản cuối.

**Thời điểm / bối cảnh:**
Sau Phase 3–6 và trước khi từng thành viên nộp repo cá nhân.

**Current workflow:**

1. Thành viên trao đổi và sửa nội dung ở công cụ chung.
2. Một người thông báo đã có “bản cuối”.
3. Mỗi người tải/copy file về repo riêng.
4. Có sửa muộn thì thông báo lại qua chat.
5. Từng người tự kiểm tra mình đã copy bản mới nhất hay chưa.

**Bottleneck:**
Bước 4–5: handoff phụ thuộc vào thông báo và kiểm tra thủ công.

**Impact:**
Cùng một nhóm có thể có các bản khác nhau về metric, boundary hoặc quyết định Go/Not Yet/No-Go; người chấm khó xác định bản chuẩn.

**Success metric:**
Hash của `group-report.md` giống nhau ở 100% repo thành viên tại thời điểm nộp; mọi bản có cùng version ID và thời gian chốt.

**Non-AI alternative:**
Chỉ định một source of truth, gắn version/tag, công bố checksum và checklist copy.

**AI hypothesis:**
AI không cần thiết cho việc đồng bộ file; nếu dùng, chỉ nên tóm tắt diff để người thật quyết định có đồng bộ hay không.

**Quick gut:**
- [ ] No AI / process fix
- [x] Rule
- [ ] Workflow
- [ ] Agent
- [ ] Chưa biết

### Draft workflow #2

```text
CURRENT STATE

[Cùng sửa bản nhóm]
→ [Nhắn "bản cuối"]
→ [Mỗi người copy thủ công]
→ [Có sửa muộn]
→ [Hỏi lại bản nào mới nhất]          <-- bottleneck
→ [Nộp]

FUTURE STATE (giả thuyết cần kiểm chứng)

[Một source of truth]
→ [Người phụ trách chốt version + hash]
→ [Thành viên copy/pull]
→ [Script so hash]
→ <Khớp?> -- Có --> [Nộp]
          -- Không --> [Đồng bộ lại]   <-- human action

Fallback: script lỗi → so commit SHA hoặc diff thủ công.
```

## Problem Card #3 — Decision log cho hội tụ nhóm

**Problem 1 câu:**
Trong lúc nhóm pitch và challenge nhiều candidate, lý do chọn/loại dễ bị thất lạc, khiến người viết báo cáo phải hỏi lại hoặc suy đoán sau buổi thảo luận.

**Actor:**
Người điều phối/người ghi chép và các thành viên tham gia hội tụ nhóm.

**Thời điểm / bối cảnh:**
Phase 3 khi nhóm đi từ khoảng 9–12 candidates về một candidate để đào sâu.

**Current workflow:**

1. Mỗi người pitch top 3.
2. Thành viên đặt câu hỏi/challenge.
3. Nhóm gom cluster và shortlist.
4. Nhóm thảo luận rồi chọn candidate.
5. Sau buổi họp, người viết nhớ lại lý do và điền report.
6. Hỏi lại thành viên nếu thiếu thông tin.

**Bottleneck:**
Bước 5–6: reconstruct quyết định sau khi cuộc trao đổi đã kết thúc.

**Impact:**
Mất phản biện quan trọng, báo cáo có thể chỉ ghi “nhóm chọn vì tốt nhất” mà thiếu evidence; số lần hỏi lại hiện **cần đo**.

**Success metric:**
100% candidate trong shortlist có score, lý do chọn/không chọn và ít nhất một challenge được ghi ngay trong buổi; không cần hỏi lại để viết convergence log.

**Non-AI alternative:**
Một decision-log template có người ghi chép, timestamp, owner và trường “evidence/challenge”.

**AI hypothesis:**
Nếu được tất cả thành viên đồng ý và có transcript, AI có thể draft recap; người ghi chép phải kiểm tra trước khi đưa vào báo cáo. Không ghi âm ngầm.

**Quick gut:**
- [x] No AI / process fix
- [ ] Rule
- [ ] Workflow
- [ ] Agent
- [ ] Chưa biết

### Draft workflow #3

```text
CURRENT STATE

[Pitch]
→ [Challenge]
→ [Shortlist]
→ [Chọn candidate]
→ [Nhớ lại sau buổi họp]              <-- bottleneck
→ [Hỏi lại]
→ [Viết convergence log]

FUTURE STATE (giả thuyết cần kiểm chứng)

[Mở decision-log template]
→ [Pitch + ghi candidate/owner]
→ [Ghi challenge/evidence ngay lúc nói]
→ [Score + ghi lý do chọn/loại]
→ [Nhóm đọc lại và xác nhận]           <-- human boundary
→ [Đưa log đã xác nhận vào report]

Fallback: thiếu ghi chép → đánh dấu "chưa xác nhận" và hỏi đúng người,
không để AI tự suy diễn lý do.
```

## Card muốn pitch nhất

**Card:** #1 — Rà soát độ đầy đủ và nhất quán của bài nộp cá nhân.

**Vì sao:**
Pain đã xuất hiện ngay trong phiên làm bài này, input và output đều quan sát được, có thể tạo bộ test lỗi để đo chính xác, và cho phép so sánh rõ ba mức: checklist thủ công, rule-based checker, hoặc workflow có AI review. Scope không cần truy cập dữ liệu nhạy cảm và không cần Agent tự chủ.

**Câu hỏi muốn nhóm challenge:**
“Checklist/rule-based checker có giải quyết đủ phần lớn lỗi không, và lỗi ngữ nghĩa nào thực sự cần AI thay vì chỉ cần rubric rõ hơn?”

## Nhật ký sử dụng AI cho phần này

AI được dùng để:

- đọc và hệ thống hóa yêu cầu từ ba tài liệu trong repo;
- kiểm tra cấu trúc card theo worksheet;
- chuyển mô tả workflow thành dạng text dễ đọc;
- phản biện việc nhảy sang Agent quá sớm.

Giới hạn:

- AI không có quyền truy cập trải nghiệm riêng, chat nhóm hoặc số liệu bấm giờ của tôi;
- vì vậy bài chỉ dùng bằng chứng kiểm tra được từ repo và đánh dấu rõ các baseline cần đo;
- tôi cần tự xác nhận các candidate với trải nghiệm thật và cập nhật số liệu sau buổi làm nhóm.
