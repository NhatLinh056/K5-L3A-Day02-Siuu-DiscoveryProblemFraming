# Báo cáo cá nhân — 2A202603514_LeNhatLinh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Lê Nhật Linh
- MSSV: 2A202603514
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Siuu
- Link repo nhóm: https://github.com/NhatLinh056/K5-L3A-Day02-Siuu-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

|   # | Lăng kính                         | Job Story: Khi… tôi muốn… để…                                                                                                                                                                     | Ai chịu ảnh hưởng?              | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng)                                                                                      |
| --: | --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
|   1 | Lặp lại                           | Khi đến cuối tuần cần báo cáo tiến độ công việc, tôi muốn tổng hợp các nhiệm vụ đã hoàn thành và đang thực hiện, để cập nhật tiến độ đầy đủ, chính xác và đúng hạn.                               | Nhóm trưởng, thành viên nhóm    | Mất 70 phút mỗi chiều Chủ nhật; 4 lần/tháng; phải lục tin nhắn Zalo và board task của nhóm 4 người; 2/4 tuần gần nhất gửi báo cáo trễ sau 22h. |
|   2 | Tốn thời gian                     | Khi tiếp nhận một dự án phần mềm mới, tôi muốn hiểu cấu trúc mã nguồn và luồng xử lý chính, để bắt đầu thực hiện công việc được giao một cách chính xác.                                          | Developer mới, thực tập sinh IT | Mất 180 phút (3 tiếng) trong 2 ngày đầu nhận repo; phải ping hỏi mentor 3–4 lần để hiểu luồng chạy; tự bấm giờ ở đồ án kỳ trước.               |
|   3 | Cần đọc, tổng hợp nhiều thông tin | Khi cần sử dụng lại tài liệu kỹ thuật hoặc đường link đã lưu, tôi muốn tìm đúng thông tin cần thiết, để tiếp tục công việc mà không phải tìm kiếm lại từ đầu.                                     | Sinh viên IT, Developer         | Mất 20–30 phút/lần tìm lại link Notion/docs cũ; xảy ra 3–4 lần/tuần; có hơn 50+ bookmark link rời rạc trong trình duyệt và chat nhóm.          |
|   4 | Pain từ người khác                | Khi tham gia dự án có nhiều nhiệm vụ với thời hạn khác nhau, tôi muốn nắm rõ deadline và mức độ ưu tiên của từng nhiệm vụ, để hoàn thành công việc đúng hạn và không ảnh hưởng đến tiến độ chung. | Thành viên nhóm, trưởng nhóm    | 1–2 lần/sprint có thành viên nộp trễ hoặc hỏi lại thứ tự ưu tiên sát giờ; nhóm 4 người có 10+ task song song; đợt sprint 2 trễ hạn nộp 1 ngày. |
|   5 | Pain từ người khác                | Khi nhận một task có mô tả chưa rõ ràng, tôi muốn hiểu chính xác yêu cầu và tiêu chí hoàn thành, để thực hiện đúng ngay từ đầu và hạn chế phải chỉnh sửa lại.                                     | Developer, thành viên nhóm      | Mất 60 phút chờ phản hồi giải thích task; 3/10 task thiếu Acceptance Criteria; trung bình 2 task/sprint phải sửa lại, mất 4–6h làm lại.        |

**Nếu có dùng AI để gợi ý thêm:**

- **Công cụ:** ChatGPT.
- **Ý giữ lại:** Gợi ý lăng kính tổng hợp tài liệu và làm rõ yêu cầu task (viết lại thành #3, #5 theo số liệu thật).
- **Ý loại bỏ:** Debug microservices, cấu hình CI/CD, phân loại ticket hạ tầng server.
- **Lý do loại bỏ:** Vĩ mô, xa vời trải nghiệm thực tế học tập và làm việc nhóm.

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem                                                                | Vì sao chọn                                                                                                                                                    | Điều còn chưa chắc                                                                                                                                      |
| ---: | :--------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
|    1 | **Tìm hiểu cấu trúc và luồng xử lý codebase dự án mới**                | Tốn nhiều thời gian nhất (180 phút/lần onboard), là rào cản lớn nhất khi tiếp nhận dự án mới; quy trình 7 bước rõ ràng, dễ đo lường bằng việc bấm giờ thực tế. | Liệu việc bổ sung tài liệu kiến trúc chuẩn (README/Mermaid) đã đủ giải quyết chưa, hay thật sự cần AI hỗ trợ tương tác trace code theo use-case cụ thể? |
|    2 | **Task được giao không rõ yêu cầu và thiếu tiêu chí hoàn thành**       | Pain lớn từ người khác, gây lãng phí 4–6 giờ làm lại cho cả nhóm, quy trình giao việc có các bước cụ thể.                                                      | Liệu chỉ cần bắt buộc áp dụng mẫu form template (Rule) là đủ, hay vẫn cần AI để rà soát ngữ cảnh mô tả task?                                            |
|    3 | **Mất thời gian tổng hợp báo cáo tiến độ tuần từ nhiều nguồn rải rác** | Lặp lại đều đặn mỗi tuần (70 phút/lần), có bằng chứng trễ hạn thực tế (2/4 tuần gần nhất), dễ so sánh phương án Rule vs Workflow.                              | Dữ liệu commit Git và task board có đủ ngữ cảnh để sinh báo cáo mạch lạc không, hay vẫn cần con người tổng hợp thủ công các blocker?                    |

### Problem Card #1 – Tìm hiểu codebase mới

| Trường                                    | Nội dung                                                                                                                                                                                                                                                                                                                 |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Job Story                                 | Khi tiếp nhận một dự án phần mềm mới (khoảng 30–50 files mã nguồn), tôi muốn hiểu nhanh cấu trúc thư mục và luồng dữ liệu chính, để bắt đầu code đúng task được giao mà không làm sai lệch kiến trúc.                                                                                                                    |
| Actor                                     | Sinh viên ngành CNTT / Developer mới gia nhập nhóm dự án đồ án môn học hoặc dự án thực tập (chưa nắm kiến trúc hệ thống).                                                                                                                                                                                                |
| Thời điểm / bối cảnh                      | Buổi đầu tiên nhận repository Git và task tính năng đầu tiên từ trưởng nhóm / mentor.                                                                                                                                                                                                                                    |
| Quy trình hiện tại (3–7 bước)             | 1. Nhận repo Git và mô tả task (5') → 2. Đọc README & tài liệu cài đặt (15') → 3. Duyệt cấu trúc thư mục & file config (20') → 4. Tìm module liên quan đến task (30') → 5. Đọc code & lần theo luồng hàm giữa các tầng (60') → 6. Chạy thử project local & debug (30') → 7. Nhắn tin hỏi bạn lead để xác nhận lại (20'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5 (Đọc code chi tiết và lần theo luồng gọi hàm giữa các tầng Controller → Service → Repository): mất **60 phút** (chiếm 33% tổng thời gian 180 phút). Nghẽn do không có sơ đồ call-graph, người mới phải đọc lần mò qua lại giữa hàng chục file code để trace luồng thủ công.                                       |
| Impact (nếu không giải thì sao)           | Mất **180 phút** (3 tiếng) cho mỗi lần onboard task mới. Trung bình mỗi đồ án có 2–3 thành viên mới; nếu hiểu sai luồng logic dẫn đến viết code sai kiến trúc, phát sinh 2–3 bug khi merge PR và nhóm mất thêm 2–4 giờ refactor lại code.                                                                                |
| Success metric (baseline → target)        | Thời gian đọc code và hiểu luồng xử lý chính giảm từ **60 phút xuống ≤ 25 phút**; tổng thời gian onboarding từ lúc nhận repo đến khi chạy thử xong task đầu tiên giảm từ **180 phút xuống ≤ 90 phút** (giảm 50%); số lần phải gọi hỏi mentor/lead giảm từ **3–4 lần xuống ≤ 1 lần/task**. Đo bằng bấm giờ thực tế.       |
| Phương án không dùng AI                   | Chuẩn hóa tài liệu dự án: Bắt buộc README có hướng dẫn cài đặt, sơ đồ kiến trúc module C4 Model cấp độ 2 và luồng dữ liệu chính vẽ bằng Mermaid; quy định 20 phút pair walkthrough 1-on-1 giữa mentor và thành viên mới.                                                                                                 |
| Giả thuyết về AI (nếu có)                 | AI phân tích mã nguồn (code-aware LLM) tự động quét repo, tóm tắt vai trò từng module và tự sinh sơ đồ call-graph mô tả luồng gọi hàm từ API endpoint đến database cho use-case cụ thể.                                                                                                                                  |
| Cảm nhận nhanh                            | **Workflow** (Cần kết hợp phân tích cú pháp code tĩnh với LLM tóm tắt logic; con người vẫn phải tự chạy debug đặt breakpoint trên máy để kiểm chứng).                                                                                                                                                                    |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 180 phút

[1 Nhận repo + task: 5'] → [2 Đọc README: 15']
→ [3 Xem cấu trúc thư mục: 20'] → [4 Tìm module: 30']
→ [5 Đọc code + lần theo luồng: 60'] ← BOTTLENECK (lạc giữa các tầng file code)
→ [6 Chạy thử & debug: 30'] → [7 Hỏi lead xác nhận: 20']
```

### Problem Card #2 – Task không rõ yêu cầu

| Trường                                    | Nội dung                                                                                                                                                                                                                                                                                                         |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi nhận một task phát triển tính năng có mô tả chưa rõ ràng, tôi muốn nắm chắc yêu cầu đầu vào, đầu ra và tiêu chí hoàn thành (Acceptance Criteria), để triển khai đúng ngay từ đầu và không bị reject khi review code.                                                                                         |
| Actor                                     | Developer / Thành viên nhóm thực hiện task trong dự án phần mềm khi nhận việc từ Trưởng nhóm hoặc Product Owner.                                                                                                                                                                                                 |
| Thời điểm / bối cảnh                      | Buổi phân chia công việc đầu sprint hoặc khi nhận task mới trên board Trello/Jira/GitHub Projects.                                                                                                                                                                                                               |
| Quy trình hiện tại (3–7 bước)             | 1. Nhận task trên board (5') → 2. Đọc mô tả task (10') → 3. Tự tìm kiếm thông tin nghiệp vụ còn thiếu (15') → 4. Soạn tin nhắn hỏi lại người giao task (10') → 5. Chờ người giao task phản hồi giải thích (60') → 6. Bắt tay code tính năng (90') → 7. Tạo Pull Request & giải trình nghiệp vụ khi review (20'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5 (Chờ người giao task phản hồi giải thích): mất **60 phút** (chiếm gần 30% tổng thời gian 210 phút quy trình). Nghẽn do người giao bận học hoặc họp không trả lời ngay, gây đứt gãy mạch làm việc (context switching), khiến developer rơi vào trạng thái nhàn rỗi thụ động.                               |
| Impact (nếu không giải thì sao)           | **3/10 task** trong sprint bị thiếu Acceptance Criteria; dẫn đến trung bình **2 lần hiểu sai yêu cầu** trong mỗi sprint, khiến dev phải đập đi xây lại code sau khi bị review reject, gây lãng phí **4–6 giờ làm lại** và trễ hạn nộp đồ án của cả nhóm 1 ngày.                                                  |
| Success metric (baseline → target)        | Thời gian chờ phản hồi làm rõ task giảm từ **60 phút xuống ≤ 15 phút**; tỷ lệ task thiếu tiêu chí nghiệm thu (Acceptance Criteria) giảm từ **30% xuống ≤ 5%**; số lần task bị từ chối lúc review PR do hiểu sai yêu cầu giảm từ **2 lần/sprint về 0**. Đo qua log chat và Jira.                                  |
| Phương án không dùng AI                   | Quy định bắt buộc Task Template trên GitHub Issues/Jira với 3 mục chuẩn: Bối cảnh, User Story, và Acceptance Criteria dạng Gherkin (Given-When-Then); áp dụng quy tắc "Definition of Ready" (Rule): task chưa đủ tiêu chí thì cấm kéo sang cột In Progress.                                                      |
| Giả thuyết về AI (nếu có)                 | AI Linter tự động quét mô tả task ngay khi tạo: phát hiện các câu từ mơ hồ (ví dụ "tối ưu tốc độ", "làm giao diện trực quan") và gợi ý người giao task bổ sung checklist Acceptance Criteria định lượng trước khi bấm Assign.                                                                                    |
| Cảm nhận nhanh                            | **Rule / Workflow** (Chỉ cần Rule template chuẩn đã giải quyết được 70% vấn đề; Workflow AI linter chỉ đóng vai trò hỗ trợ gợi ý checklist biên).                                                                                                                                                                |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 210 phút

[1 Nhận task: 5'] → [2 Đọc mô tả: 10']
→ [3 Tìm kiếm thông tin: 15'] → [4 Soạn câu hỏi: 10']
→ [5 Chờ phản hồi làm rõ: 60'] ← BOTTLENECK (ngắt quãng luồng công việc)
→ [6 Code tính năng: 90'] → [7 Review & giải trình: 20']
```

### Problem Card #3 – Báo cáo tiến độ hằng tuần

| Trường                                    | Nội dung                                                                                                                                                                                                                                                                                        |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi đến kỳ báo cáo tuần vào tối Chủ nhật, tôi muốn tổng hợp nhanh tiến độ công việc và các vướng mắc của toàn bộ thành viên, để nộp báo cáo đúng hạn trước 22h cho giảng viên mà không bỏ sót blocker nào.                                                                                      |
| Actor                                     | Trưởng nhóm (Team Leader) hoặc thành viên luân phiên chịu trách nhiệm tổng hợp tiến độ tuần của nhóm đồ án 4–5 người.                                                                                                                                                                           |
| Thời điểm / bối cảnh                      | Tối Chủ nhật hằng tuần, khoảng 20h–22h, trước hạn chót nộp báo cáo sprint môn học.                                                                                                                                                                                                              |
| Quy trình hiện tại (3–7 bước)             | 1. Mở task board & GitHub repo (5') → 2. Kiểm tra task và commit cá nhân (10') → 3. Nhắn tin nhóm chat & ping từng thành viên nhắc nộp cập nhật (20') → 4. Đọc gom thông tin & lọc blocker (15') → 5. Viết báo cáo tiến độ hoàn chỉnh vào Docs (15') → 6. Rà soát định dạng & gửi báo cáo (5'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (Nhắn tin nhóm chat và ping từng bạn nhắc nộp tiến độ): mất **20 phút** (chiếm gần 30% tổng thời gian 70 phút). Nghẽn vì các thành viên trả lời rải rác, không đúng cấu trúc yêu cầu, người tổng hợp phải chờ đợi và nhắn tin nhắc lại 2–3 lần.                                          |
| Impact (nếu không giải thì sao)           | Mất **70 phút/tuần** cho một công việc thuần túy hành chính; **2/4 tuần gần nhất** gửi báo cáo trễ sau 22h; từng bỏ sót 1 blocker cấu hình DB của bạn backend khiến cả nhóm bị trừ điểm chuyên cần ở buổi review.                                                                               |
| Success metric (baseline → target)        | Tổng thời gian lập báo cáo tuần giảm từ **70 phút xuống ≤ 25 phút**; **100% báo cáo** được gửi đúng hạn trước 21h Chủ nhật; **0 blocker kỹ thuật** bị bỏ sót trong báo cáo. Đo từ lúc bắt đầu tổng hợp đến lúc gửi báo cáo.                                                                     |
| Phương án không dùng AI                   | Mẫu Google Form cố định hoặc Discord Standup bot tự động nhắc định kỳ; quy định thành viên điền 3 mục (Đã làm, Đang làm, Vướng mắc) trước 18h Chủ nhật; dùng dashboard tiến độ có sẵn của GitHub Projects.                                                                                      |
| Giả thuyết về AI (nếu có)                 | AI tự động đọc Git commit log và PR đã merge trong tuần từ GitHub API, soạn bản nháp báo cáo theo mẫu chuẩn (tiến độ, rủi ro) để nhóm trưởng chỉ cần review và bổ sung nhận định trong 5 phút.                                                                                                  |
| Cảm nhận nhanh                            | **Rule / Workflow** (Rule tự động nhắc và gom log Git đã giải quyết phần lấy số liệu; AI hỗ trợ tóm tắt thành văn bản báo cáo mạch lạc cho GV).                                                                                                                                                 |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 70 phút

[1 Mở Git & task board: 5'] → [2 Kiểm tra task cá nhân: 10']
→ [3 Thu thập cập nhật & ping nhắc: 20'] ← BOTTLENECK (chờ đợi thông tin rải rác)
→ [4 Gom thông tin & lọc blocker: 15'] → [5 Soạn văn bản báo cáo: 15']
→ [6 Rà soát format & gửi: 5']
```

### Card muốn pitch nhất

- **Card số:** 1 – Tìm hiểu cấu trúc và luồng xử lý codebase dự án mới.
- **Vì sao:** Đây là nỗi đau thực tế lớn nhất của sinh viên và developer khi tham gia dự án (mất tới 180 phút/lần onboard), quy trình kỹ thuật gồm 7 bước rõ ràng, bottleneck cụ thể (bước 5 đọc code trace luồng mất 60 phút) và có thể định lượng chính xác thời gian tiết kiệm được. Đồng thời bài toán này giúp nhóm dễ dàng phân định ranh giới giữa giải pháp No AI (chuẩn hóa tài liệu), Rule (linter/call graph tĩnh) và AI Workflow.
- **Câu hỏi muốn nhóm phản biện:** "Liệu việc chuẩn hóa tài liệu dự án bằng sơ đồ kiến trúc Mermaid (giải pháp No AI) đã đủ để giảm 50% thời gian onboard chưa, hay nhóm thật sự cần giải pháp AI để giải thích luồng xử lý tương tác cho từng use-case cụ thể?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra                                                                                                            | Đồng ý? | Đã sửa gì                                                                                                                                          |
| ----------------------------------------------------------------------------------------------------------------------------- | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Card #1 (Codebase):** Nghi ngờ số liệu 180'; chưa ưu tiên giải pháp No AI (docs/sơ đồ kiến trúc); rủi ro AI bịa luồng code. | Đồng ý  | Bổ sung số liệu bấm giờ thật; ưu tiên làm README chuẩn + sơ đồ C4 trước; thêm boundary: AI chỉ vẽ nháp call-graph, dev tự đặt breakpoint xác minh. |
| **Card #2 (Task mơ hồ):** Chỉ cần form mẫu bắt buộc (Rule), dùng AI là thừa; metric giảm 30% mơ hồ.                           | Đồng ý  | Đưa giải pháp Rule lên đầu (Template Issue + Acceptance Criteria bắt buộc); đổi metric: chờ phản hồi ≤ 15', task thiếu AC ≤ 5%.                    |
| **Card #3 (Báo cáo tuần):** Chậm do thành viên nộp muộn (kỷ luật), AI không sửa được tính ỳ; công cụ sẵn có đã hỗ trợ.        | Đồng ý  | Dùng Rule (bot nhắc giờ + form chuẩn); giới hạn AI chỉ tóm tắt log Git thành bản nháp narrative; rút thời gian từ 70' xuống ≤ 25'.                 |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Problem Card #1 (Tìm hiểu codebase dự án mới, baseline 180' → target 90'). | Nhóm nhận thấy đây là bài toán kỹ thuật có số liệu đo lường rõ ràng nhất và chọn làm candidate #1. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: • Hỏi Hải (#5 - Review blog): "Tại sao không bắt agency tự chạy checklist format/chính tả trước khi nộp mà Lead phải tốn 60' sửa thay? Lỗi do quy trình hay cần AI?" • Hỏi Khiêm (#8 - Biên bản họp): "Ghi âm cuộc họp đưa lên AI có vi phạm bảo mật thông tin nội bộ của nhóm không?" • Hỏi Việt (#10 - Hạn nộp bài): "Google Calendar và tính năng nhắc hẹn của LMS đã giải quyết tự động việc này rồi, sao cần AI?" | Hải đồng ý bổ sung quy trình nghiệm thu bằng Rule checklist; Khiêm thêm ranh giới bảo mật ẩn danh text; Việt rút card #10 khỏi shortlist vì Rule/LMS đã đủ giải quyết. |
| Nhận phản biện | Câu hỏi tôi nhận được: • Khiêm (#1 - Codebase): "AI chỉ giảm bước 5 được 35', vậy 55' còn lại để đạt 180' → 90' giảm ở đâu?" • Hải (#2 - Task không rõ): "Vấn đề này do người giao thiếu template hay do dev chưa chủ động research?" • Việt (#3 - Báo cáo tuần): "Jira và GitHub Projects đã có dashboard số liệu, tại sao khâu này vẫn mất 70 phút?" | Tôi đã sửa: Với #1: Làm rõ 55' còn lại giảm nhờ dây chuyền (định vị file nhanh hơn 30', giảm hỏi lead 15', giảm thử sai 10'); Với #2: Đưa Rule Issue template lên đầu; Với #3: Rút gọn quy trình bằng bot nhắc giờ tự động. |
| Gom cluster / cây OST | Chủ trì tổng hợp 12 candidate problems của 4 thành viên, gom thành 3 cluster A, B, C; dựng khung cây OST nối từ Outcome (180' → 90') sang 3 nhánh cơ hội (Opportunity). | Nhóm thống nhất được cấu trúc cây OST, phân định rạch ròi giữa mục tiêu, cơ hội và giải pháp (gạch bỏ các giải pháp sớm). |
| Chọn candidate problem | Dẫn dắt nhóm lập bảng chấm điểm 7 tiêu chí cho 3 candidate shortlist; giải thích lý do chọn Card #1 (35/35 điểm) và loại Card #2, #3. | Cả 4 thành viên đồng thuận 100% chọn bài toán Onboarding Codebase; có lý do loại trừ rõ ràng theo chuẩn rubric C6. |
| Kiểm chứng / research | Rà soát bảng Assumption Map 5 giả định; hỗ trợ định hướng các câu hỏi phỏng vấn Mom Test tập trung vào hành vi trace code thực tế trong quá khứ của sinh viên. | Tránh cho nhóm câu hỏi khảo sát vi phạm Mom Test; hỗ trợ phân tích kết quả phỏng vấn và khảo sát. |
| Quy trình nhóm | Phản biện sơ đồ quy trình tương lai; yêu cầu bổ sung bắt buộc bước HITL đặt breakpoint và nhánh Fallback (Call Hierarchy IDE + 10' pair mentor) khi AI hallucinate. | Quy trình tương lai hoàn thiện, có đường lui an toàn khi AI gợi ý sai, đạt trọn vẹn điểm tiêu chí C8. |
| Problem Statement | Trực tiếp soạn thảo Problem Statement v0 và v1; chuẩn hóa 9 trường thông tin; định lượng Success Metric (180' → 90', hỏi mentor ≤ 1 lần) và ranh giới Boundary cấm AI tự ý sinh code. | Định hình bài toán sắc nét, có rào chắn AI rõ ràng và tiêu chí đo lường định lượng cụ thể. |
| Mức can thiệp AI | Thảo luận và đề xuất mức can thiệp AI Workflow (kết hợp Rule AST lọc file) thay vì Agent tự hành; xây dựng bảng AI Canvas và phân tích rủi ro Báo nhầm theo Google PAIR. | Giúp nhóm chọn mức can thiệp thực tế, vừa sức lab, tránh rơi vào bẫy ảo tưởng công nghệ (Agent). |
| Quyết định | Thống nhất chốt quyết định Go với pilot 2 repository mẫu trong 1 tuần; ấn định ngưỡng dừng Kill Switch đo được (> 15% hallucination hoặc giảm < 40' thì dừng). | Nhóm có quyết định dứt khoát kèm ngưỡng dừng đo lường thực tế, đạt chuẩn rubric C11. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm problem sau khi đã tự scan trước. | Mở rộng góc nhìn về việc đọc tài liệu kỹ thuật và khó khăn khi làm rõ yêu cầu task. | Gợi ý các bài toán quá nặng về hạ tầng (debug microservices, CI/CD) không phù hợp phạm vi thực tế của học viên. | Lọc bỏ các bài toán hạ tầng viển vông, chỉ giữ lại các vấn đề sát sườn với dev hàng ngày có thể đo lường được. |
| CP2 Problem Card | Đóng vai "PM hoài nghi" để tìm lỗ hổng trong 3 card. | Chỉ ra card thiếu số liệu thực tế, chưa đo thời gian và chưa thử phương án không AI. | Gợi ý nhảy ngay vào làm agent phân tích toàn bộ repo mà không tính đến chi phí, độ phức tạp và rủi ro hallucination. | Bổ sung số phút cụ thể từng bước, đặt baseline/target rõ ràng và ưu tiên giải pháp tài liệu onboarding/workflow trước. |
| CP4 Research | Rà soát 5 giả định trong bảng Assumption Map. | Gợi ý thêm các khía cạnh rủi ro về Usability (độ tin tưởng của dev vào sơ đồ). | Đưa ra các giả định chung chung về cảm xúc ("người dùng thích giao diện trực quan") không thể kiểm chứng được. | Đổi thành giả định kỹ thuật đo được: dev có chịu dùng sơ đồ call-graph thay vì lội code thủ công không và AI có bịa hàm ảo khi trace code không. |
| CP5 Quy trình | Sinh cú pháp Mermaid cho sơ đồ quy trình tương lai. | Dựng nhanh khung sơ đồ trực quan với cú pháp chuẩn xác. | AI tự động hóa hoàn toàn 100% (bỏ qua dev, để AI tự đọc và tự code luôn), không hề có bước con người kiểm tra (HITL). | Bắt buộc AI phải đưa con người vào giữa quy trình (bước 5: dev đặt breakpoint kiểm chứng) và vẽ thêm nhánh Fallback Call Hierarchy nếu AI gợi ý sai. |
| CP5–6 Problem Statement | Đóng vai "PM hoài nghi" để phản biện Problem Statement v0. | Chỉ ra điểm yếu chí mạng: giảm từ 180' xuống 90' là quá lớn nếu chỉ dựa vào một mình AI ở bước trace code. | Khuyên hạ target xuống 150' hoặc thêm tính năng tự động sinh code để bù thời gian. | Giữ nguyên target 90' nhưng làm rõ hiệu ứng dây chuyền trong bảng Before/After: giảm ở định vị file (30'), trace code (45') và giảm hỏi mentor (15'). |
| CP6 Mức can thiệp / quyết định | So sánh AI Workflow vs AI Agent và gợi ý ngưỡng dừng Kill Switch. | Phân tích được trade-off giữa độ phức tạp và khả năng kiểm soát chất lượng. | Khuyên làm Autonomous Agent với lý do xu hướng công nghệ, và đưa ngưỡng dừng cảm tính ("dừng khi người dùng không hài lòng"). | Bác bỏ hoàn toàn Agent, kiên quyết chọn AI Workflow; đưa ra ngưỡng dừng bằng số cứng: tỷ lệ hallucinate > 15% hoặc không giảm được ≥ 40' sau 1 tuần. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Khi nghe pitch top 3 của các bạn trong nhóm (bạn Hải về review bài viết blog agency, bạn Khiêm về giải đáp thắc mắc trùng lặp, bạn Việt về gỡ lỗi lập trình sinh viên), tôi nhận ra vấn đề của bạn Hải rất thực tế trong mảng vận hành nội dung nhưng phạm vi giải quyết lại phụ thuộc nhiều vào quy trình nghiệm thu với bên thứ ba (agency). Bài của bạn Khiêm và Việt rất gần gũi với môi trường học tập nhưng phần lớn có thể giải quyết được bằng Rule hoặc chuẩn hóa tài liệu (No AI) mà chưa nhất thiết phải cần đến AI. Việc lắng nghe giúp tôi học được cách phân biệt giữa một vấn đề gây khó chịu đơn thuần (annoyance) và một điểm nghẽn thực sự (bottleneck) làm tiêu tốn hàng giờ lặp đi lặp lại có thể đo lường định lượng được.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Nhóm bị "solution-first" rõ rệt nhất ở đầu giai đoạn CP3 và CP5. Khi vừa thống nhất chọn bài toán Codebase, các thành viên lập tức hào hứng bàn về việc "xây dựng một AI Agent tự động đọc hiểu toàn bộ repo rồi tự code và chạy test luôn", xem AI như một giải pháp vạn năng. Nhóm chỉ giật mình nhận ra sai lầm khi bắt tay vào vẽ cây OST và phân tích quy trình Before/After: nếu để AI tự động làm hết, developer mới sẽ hoàn toàn mất quyền kiểm soát, không hiểu bản chất kiến trúc và rủi ro sinh bug tiềm ẩn là cực kỳ lớn. Nhóm đã kịp thời xử lý bằng cách bóc tách cơ hội cốt lõi là "developer cần một bản đồ dẫn đường trực quan" chứ không phải "cần AI làm thay", từ đó kéo mức can thiệp từ Agent tự hành xuống AI Workflow hỗ trợ trích xuất luồng hàm.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi đã đổi ý hoàn toàn sau khi nhận được câu hỏi phản biện rất sắc bén từ bạn Hoàng Gia Khiêm: *"AI ở bước 5 chỉ giảm được 35 phút, vậy làm sao toàn bộ quy trình đạt được mục tiêu giảm từ 180 phút xuống 90 phút?"*. Ban đầu, tôi giả định khá chủ quan rằng khi có AI thì các bước khác cũng sẽ tự khắc nhanh hơn. Lời phản biện của Khiêm buộc tôi phải ngồi tính toán chi tiết sự tương tác giữa các bước: giảm 90 phút thực chất là hiệu ứng dây chuyền – nhờ có sơ đồ call-graph dẫn đường nên bước 3–4 định vị file nhanh hơn 30 phút, bước 5 trace code giảm 45 phút, bước 6 giảm thử sai 10 phút và bước 7 giảm làm phiền mentor 15 phút. Sự thay đổi này giúp bảng Before/After của nhóm trở nên thực tế và có sức thuyết phục cao.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ nhất là tín hiệu phản bác thu được từ cuộc phỏng vấn sâu bạn sinh viên làm đồ án (Interview Snapshot #2 do bạn Hải thực hiện). Trước đó, tôi đinh ninh rằng developer nào cũng thích AI sinh ra càng nhiều gợi ý càng tốt. Nhưng bạn sinh viên lại chia sẻ trải nghiệm bực bội: mất thêm 45 phút mò mẫm debug chỉ vì tin vào một hàm helper ảo do ChatGPT tự bịa ra. Tín hiệu phản bác này khiến cả nhóm thức tỉnh và lập tức điều chỉnh Boundary: kiên quyết cấm AI tự ý sinh code, chỉ cho phép trích xuất sơ đồ tương tác hàm và bắt buộc phải dẫn nguồn chính xác số dòng code thật (`filepath:linenumber`) để developer tự kiểm chứng.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Điều khó nhất là xác định ranh giới (Boundary) và chỉ số thành công (Success Metric) sao cho đo lường được. Rất dễ rơi vào cái bẫy viết văn hoa sáo rỗng như "giúp lập trình viên hiểu code sâu sắc hơn và tăng năng suất". Để ép được mục tiêu về con số định lượng thực tế (180' → 90', giảm hỏi mentor từ 3–4 lần xuống ≤ 1 lần/task) và vạch rõ giới hạn AI không được can thiệp vào khâu viết code đòi hỏi nhóm phải tranh luận rất nhiều lần qua từng phiên bản v0 và v1.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu được làm lại từ đầu, tôi sẽ phản biện nhóm quyết liệt hơn ngay từ CP1 để gạt bỏ sớm các bài toán thiên về giải pháp trá hình (dạng "cần một công cụ AI để..."). Ngoài ra, ở khâu kiểm chứng CP4, tôi sẽ chuẩn bị sẵn một repository mã nguồn mở cụ thể ngay tại lớp và cùng nhóm chạy thử nghiệm trực tiếp một prompt trích xuất luồng hàm, thay vì chỉ phỏng vấn hỏi lại trải nghiệm quá khứ, để đo đạc được ngay tỷ lệ hallucination thực tế của mô hình.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi _problem → quy trình → metric → boundary → mức can thiệp AI → quyết định_ của bài nhóm mình.

Bài toán của nhóm xuất phát từ nỗi đau thực tế của developer mới khi tiếp nhận repository lớn: mất trung bình 180 phút để hoàn thành task đầu tiên, trong đó điểm nghẽn lớn nhất là bước 5 lần theo luồng gọi hàm giữa các tầng file tốn tới 60 phút thủ công do không có sơ đồ dẫn đường. Quy trình mới tái cấu trúc 7 bước: dùng Rule AST lọc nhanh các file liên quan ở bước 3, AI Workflow trích xuất sơ đồ Call-Graph use-case ở bước 4, và bắt buộc developer (HITL) đặt breakpoint kiểm chứng trên IDE ở bước 5 kèm nhánh Fallback quay về Call Hierarchy nếu sơ đồ sai. Thành công được đo lường định lượng bằng việc rút ngắn thời gian trace code từ 60' xuống ≤ 25', tổng thời gian onboarding giảm từ 180' xuống ≤ 90' (giảm 50%) và số lần ngắt quãng mentor giảm từ 3–4 lần xuống ≤ 1 lần/task. Ranh giới an toàn (Boundary) quy định AI tuyệt đối không tự viết code, chỉ vẽ sơ đồ kèm trích dẫn chính xác đường dẫn file và số dòng code thật (`filepath:linenumber`). Mức can thiệp được chọn là AI Workflow (hướng tiếp cận Augment hỗ trợ con người hiểu bản chất) vì Rule không hiểu được luồng nghiệp vụ động, còn Agent thì quá phức tạp và rủi ro hallucination cao. Cuối cùng, nhóm đưa ra quyết định Go với phạm vi pilot nhỏ trên 2 repo mẫu trong 1 tuần, gắn liền với ngưỡng dừng Kill Switch đo được: nếu tỷ lệ hallucinate > 15% hoặc không giảm được ít nhất 40 phút thì lập tức dừng dự án và quay về dùng tài liệu tĩnh C4 vẽ tay kết hợp pair 10 phút với mentor.

---

## 7. Tài liệu tham khảo

1. Google PAIR (People + AI Research), *People + AI Guidebook: Designing human-centered AI products*, [pair.withgoogle.com](https://pair.withgoogle.com).
2. Rob Fitzpatrick (2013), *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*.
3. Simon Brown, *The C4 model for visualising software architecture*, [c4model.com](https://c4model.com).
4. Cursor Team, *Codebase Indexing & Semantic Search Architecture*, [docs.cursor.com](https://docs.cursor.com).
5. GitHub Copilot Documentation, *Using GitHub Copilot Chat in your IDE*, [docs.github.com/copilot](https://docs.github.com/copilot).
