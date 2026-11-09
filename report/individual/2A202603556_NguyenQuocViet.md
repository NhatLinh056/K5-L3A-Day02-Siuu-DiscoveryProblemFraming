# Báo cáo cá nhân — 2A202603556_NguyenQuocViet

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Quốc Việt
- MSSV: 2A202603556
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Siuu
- Link repo nhóm: https://github.com/NhatLinh056/K5-L3A-Day02-Siuu-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi ôn bài trước kỳ thi hoặc làm bài tập, tôi muốn tìm nhanh một công thức hay định nghĩa cụ thể, để tiếp tục học hoặc hoàn thành bài. | Sinh viên | Vài lần mỗi tuần; đôi khi mất 10–20 phút tìm trong slide và PDF. |
| 2 | Lặp lại | Khi có nhiều bài tập ở các môn với hạn nộp khác nhau, tôi muốn sắp xếp công việc và hạn nộp, để hoàn thành mọi bài đúng hạn. | Sinh viên học nhiều môn | Xảy ra gần như mỗi tuần; trong 4 tuần gần nhất tôi ước tính quên hoặc nộp trễ khoảng 2 bài nhỏ. Hạn nằm rải rác trong nhóm chat lớp, LMS và ghi chú điện thoại. |
| 3 | Tốn thời gian; pain từ người khác | Khi làm bài nhóm với 3–5 bạn cùng lớp, tôi muốn chia việc và theo dõi tiến độ, để mọi thành viên hiểu trách nhiệm của mình. | Tất cả thành viên nhóm | Hầu hết bài tập nhóm; dành khoảng 15–30 phút thảo luận phân công; đôi khi thành viên hiểu khác nhau về trách nhiệm. |
| 4 | Tốn thời gian | Khi làm bài lập trình bằng Python, Java hoặc ngôn ngữ khác, tôi muốn tìm nguyên nhân và sửa lỗi nhanh, để hoàn thành bài và dành thời gian hiểu nội dung khác. | Sinh viên học lập trình, lập trình viên | Vài lần mỗi tuần; một lỗi cú pháp hoặc logic nhỏ có thể mất 20–60 phút để tìm. |
| 5 | Tốn thời gian | Khi giảng viên trình bày khái niệm nhanh, tôi muốn ghi lại ý chính mà vẫn theo kịp bài giảng, để không bỏ lỡ nội dung quan trọng. | Sinh viên | Khoảng 3 buổi/tuần; ước tính bỏ lỡ 2–3 ý quan trọng mỗi tuần vì còn ghi phần trước, giảng nhanh hoặc chép lại nội dung đã có trên slide. |
| 6 | Tốn thời gian | Khi chuẩn bị thi hoặc làm bài khó, tôi muốn tìm bạn học cùng môn và có lịch phù hợp, để có thể học tập cộng tác. | Sinh viên muốn học cùng người khác | Vài lần mỗi học kỳ; có thể mất vài ngày tìm người có lịch phù hợp. |

**Nếu có dùng AI để gợi ý thêm:** Sáu vấn đề trên do Việt cung cấp. AI hỗ trợ sắp xếp và diễn đạt theo mẫu Job Story; chưa có ý tưởng bổ sung nào được giữ lại hoặc loại bỏ.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Quản lý hạn nộp bài tập (#2 CP1) | Quên hạn nộp gây căng thẳng và có thể ảnh hưởng kết quả học tập. | Chưa có số liệu về số hạn bị quên hoặc nộp trễ; cần xác định lịch nhắc và nơi ghi hạn hiện tại. |
| 2 | Điều phối bài tập nhóm (#3 CP1) | Lịch và cách giao tiếp khác nhau có thể làm việc nhóm kém hiệu quả. | Mức 1–2 giờ là cho khâu nào và mỗi dự án có bao nhiêu thành viên? Mức giảm 50% cần đo trên bao nhiêu dự án? |
| 3 | Gỡ lỗi lập trình (#4 CP1) | Thông báo lỗi khó hiểu khiến việc gỡ lỗi tốn nhiều thời gian. | Mức 20–60 phút áp dụng cho lỗi khó; cần xác định loại lỗi phổ biến và đo thời gian trước khi chọn mục tiêu. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhiều môn giao bài với các hạn khác nhau, tôi muốn tổ chức công việc và theo dõi hạn nộp, để hoàn thành bài đúng hạn. |
| Actor | Sinh viên, nhất là người học nhiều môn cùng lúc. |
| Thời điểm / bối cảnh | Gần như mỗi tuần khi nhận thông báo từ giảng viên qua nhóm chat lớp, LMS và các nguồn khác; hiện ghi thêm vào ghi chú điện thoại nhưng chưa có một nơi quản lý thống nhất. |
| Quy trình hiện tại (3–7 bước) | 1. Nhận thông tin bài tập từ giảng viên. 2. Kiểm tra hạn trên nền tảng học tập hoặc nhóm lớp. 3. Ghi hạn vào ghi chú hoặc lịch. 4. Xếp thứ tự ưu tiên. 5. Làm bài. 6. Kiểm tra và nộp trước hạn. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Tổng hợp và nhớ hạn từ nhiều nền tảng; Việt ước tính mất khoảng 10–15 phút mỗi tuần, chưa tính thời gian/hậu quả khi quên bài. Chưa tách thời gian từng bước. |
| Impact (nếu không giải thì sao) | Có thể nộp trễ, giảm điểm, căng thẳng và quản lý thời gian kém. |
| Success metric (baseline → target) | Baseline ước tính: quên hoặc nộp trễ khoảng 2 bài nhỏ trong 4 tuần gần nhất. Target: 0 bài quên/trễ; 100% bài được ghi nhận và nộp đúng hạn trong 4 tuần theo dõi. Đo bằng cách đối chiếu danh sách trên nhóm chat/LMS/ghi chú với trạng thái và thời điểm nộp. |
| Phương án không dùng AI | Google Calendar, ứng dụng quản lý công việc, nhắc hạn tự động hoặc bảng tính chung để ghi hạn. |
| Giả thuyết về AI (nếu có) | Trợ lý học tập đọc mô tả bài tập, trích hạn nộp, phân loại ưu tiên và gợi ý lịch học theo tuần. |
| Cảm nhận nhanh | Rule / Workflow; cần so sánh với lịch và nhắc hạn thông thường trước khi quyết định có cần AI. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — thời lượng từng bước chưa được đo

[1 Nhận thông tin bài tập] → [2 Kiểm tra nền tảng/nhóm lớp]
→ [3 Ghi hạn vào ghi chú/lịch: một phần của 10–15 phút/tuần] ← BOTTLENECK: tổng hợp và nhớ hạn
→ [4 Xếp ưu tiên] → [5 Làm bài] → [6 Kiểm tra và nộp]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm bài tập nhóm với 3–5 bạn cùng lớp, tôi muốn chia việc và theo dõi tiến độ, để mọi thành viên hiểu trách nhiệm và nhóm hoàn thành bài hiệu quả. |
| Actor | Các thành viên trong nhóm bài tập. |
| Thời điểm / bối cảnh | Khi bắt đầu và thực hiện bài tập nhóm; thành viên có lịch và cách giao tiếp khác nhau. |
| Quy trình hiện tại (3–7 bước) | 1. Tạo nhóm chat. 2. Thảo luận yêu cầu. 3. Chia việc. 4. Đặt hạn cá nhân. 5. Hỏi tiến độ. 6. Ghép các phần. 7. Rà soát và nộp bài. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Thu thập cập nhật tiến độ và ghép các phần; ước tính 1–2 giờ mỗi dự án. Phân công ban đầu mất khoảng 15–30 phút thảo luận. |
| Impact (nếu không giải thì sao) | Khối lượng việc không đều, trễ hạn, chất lượng các phần thiếu nhất quán và có thể phát sinh mâu thuẫn. |
| Success metric (baseline → target) | Baseline ước tính: khoảng 1–2 giờ điều phối mỗi dự án. Target: giảm 50% thời gian điều phối và mọi thành viên hiểu nhiệm vụ. Đo thời gian điều phối và hỏi từng thành viên xác nhận nhiệm vụ ở mỗi dự án; số dự án theo dõi chưa xác định. |
| Phương án không dùng AI | Trello hoặc Notion, Google Docs dùng chung, bảng phân công, hoặc họp cập nhật tiến độ định kỳ. |
| Giả thuyết về AI (nếu có) | Trợ lý dự án gợi ý phân công theo kỹ năng/lịch rảnh, theo dõi tiến độ, tóm tắt trao đổi và nhắc hạn. Nhóm vẫn cần xác nhận cách phân công. |
| Cảm nhận nhanh | Rule / Workflow; cần kiểm tra xem bảng công việc và nhắc hạn đã giải quyết đủ chưa. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — thời gian điều phối ước tính 1–2 giờ/dự án

[1 Tạo nhóm chat] → [2 Thảo luận yêu cầu: 15–30 phút]
→ [3 Chia việc] → [4 Đặt hạn cá nhân]
→ [5 Thu thập cập nhật] → [6 Ghép các phần]
   BOTTLENECK ở bước 5–6: tổng cộng khoảng 1–2 giờ/dự án
→ [7 Rà soát và nộp]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm bài lập trình bằng Python, Java hoặc ngôn ngữ khác, tôi muốn hiểu nguyên nhân lỗi và sửa lỗi, để hoàn thành bài mà vẫn học được cách gỡ lỗi. |
| Actor | Sinh viên học lập trình; vấn đề cũng có thể gặp ở lập trình viên. |
| Thời điểm / bối cảnh | Khi chạy bài tập lập trình và gặp lỗi cú pháp hoặc logic. |
| Quy trình hiện tại (3–7 bước) | 1. Viết chương trình. 2. Chạy mã. 3. Đọc thông báo lỗi. 4. Tìm trên Google hoặc Stack Overflow. 5. Thử cách sửa. 6. Chạy lại. 7. Kiểm tra kết quả. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Hiểu nguyên nhân gốc của lỗi; một lỗi khó có thể mất 20–60 phút để giải quyết. Thời gian riêng từng bước chưa đo. |
| Impact (nếu không giải thì sao) | Bài bị chậm hoặc chưa hoàn thành, gây nản và làm giảm thời gian học các khái niệm lập trình khác. |
| Success metric (baseline → target) | Baseline ước tính: khoảng 20–30 phút cho lỗi tương đối khó; 20–60 phút cho lỗi khó hơn cần trace nhiều phần code. Target: dưới 10 phút cho lỗi phổ biến. Đo thời gian từ lúc gặp lỗi đến khi hiểu nguyên nhân, sửa và xác nhận đầu ra; cần định nghĩa nhóm lỗi phổ biến. |
| Phương án không dùng AI | Công cụ debug tốt hơn, cảnh báo lỗi trong IDE, hướng dẫn gỡ lỗi, tài liệu mã và unit test. |
| Giả thuyết về AI (nếu có) | Trợ lý giải thích thông báo lỗi bằng ngôn ngữ đơn giản, nêu nguyên nhân có thể có, đề xuất cách sửa và đưa mã đã sửa kèm giải thích. Cần giữ trọng tâm vào việc học, không chỉ đưa đáp án để chép. |
| Cảm nhận nhanh | Workflow; cần thiết kế để hỗ trợ hiểu và học, đồng thời kiểm tra xem tài liệu/hướng dẫn và công cụ debug thông thường có đủ không. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 20–60 phút cho một lỗi khó (ước tính)

[1 Viết chương trình] → [2 Chạy mã] → [3 Đọc thông báo lỗi]
→ [4 Tìm Google/Stack Overflow] → [5 Thử cách sửa] ← BOTTLENECK: tìm nguyên nhân
→ [6 Chạy lại] → [7 Kiểm tra kết quả]
```

### Card muốn pitch nhất

- Card số: 3 — Gỡ lỗi lập trình.
- Ý tưởng muốn pitch: Trợ lý AI gỡ lỗi cho sinh viên lập trình. Đây là hướng giải pháp; vấn đề gốc cần mô tả rõ hơn bằng một tình huống lỗi cụ thể, quy trình hiện tại và bằng chứng về thời gian/tần suất.
- Vì sao: Lỗi lập trình thường gặp; việc gỡ lỗi có thể tốn nhiều thời gian, nhất là khi sinh viên chưa hiểu thông báo lỗi phức tạp. Ý tưởng là trợ lý giúp sinh viên hiểu nguyên nhân lỗi thay vì chỉ đưa đáp án, qua đó tiết kiệm thời gian và hỗ trợ học kỹ năng lập trình. Các nhận định về tần suất và thời gian cần được bổ sung bằng trải nghiệm hoặc số liệu thật.
- Câu hỏi muốn nhóm phản biện: “Làm thế nào để thiết kế trợ lý AI gỡ lỗi giúp sinh viên hiểu và học từ lỗi của mình, thay vì khiến họ phụ thuộc hoàn toàn vào AI?”

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Quản lý hạn nộp: lịch và nhắc hạn thông thường có thể đã giải quyết phần lớn vấn đề; cần chứng minh điểm nghẽn còn lại trước khi thêm AI. | Đồng ý. | Ghi nhận cần đo số lần quên/trễ hạn và thử phương án lịch/nhắc hạn trước khi kết luận cần AI. |
| Điều phối nhóm: phân công theo kỹ năng/lịch có thể cần dữ liệu cá nhân và sự đồng thuận; bảng nhiệm vụ/nhắc hạn có thể đủ. | Đồng ý. | Ghi nhận cần xác định rõ bước tốn thời gian và so sánh bảng nhiệm vụ/nhắc hạn trước khi kết luận cần AI. |
| Gỡ lỗi: nếu AI đưa mã đã sửa ngay, sinh viên có thể chép đáp án mà không hiểu nguyên nhân; mục tiêu học tập cần tiêu chí đánh giá. | Đồng ý. | Giữ mục tiêu AI giải thích nguyên nhân và cách sửa; cần tiêu chí để xác nhận sinh viên hiểu thay vì chỉ chép mã. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch ý tưởng trợ lý AI gỡ lỗi cho sinh viên lập trình; đặt câu hỏi làm sao giúp người học hiểu lỗi thay vì phụ thuộc hoàn toàn vào AI. | Nhóm có câu hỏi cụ thể để phản biện giá trị học tập và nguy cơ phụ thuộc AI. |
| Phản biện bài của bạn khác | Hỏi về báo cáo tuần: dashboard Jira/GitHub Projects đã đủ chưa; lịch nội dung: Buffer/Hootsuite đã giải quyết lên lịch chưa; câu hỏi lặp lại: quick reply/snippet đã đủ chưa. | Giúp nhóm so sánh từng pain với No AI/Rule trước khi đề xuất AI. |
| Nhận phản biện | Hoàng Gia Khiêm hỏi làm sao bảo đảm trợ lý gỡ lỗi giúp sinh viên hiểu bản chất lỗi thay vì chỉ chép đáp án; AI cũng lưu ý lịch/nhắc hạn và bảng nhiệm vụ có thể đủ. | Tôi đồng ý; bổ sung yêu cầu so sánh phương án đơn giản trước và giữ mục tiêu học tập trong card gỡ lỗi. |
| Gom cluster / cây OST | Tham gia hội tụ và phản biện 12 candidate; Lê Nhật Linh chủ trì gom 3 cluster và dựng khung OST. | Nhóm tập trung vào outcome onboarding 180 → 90 phút và ba opportunity liên quan đến cấu trúc repo, trace use-case, kiểm chứng luồng. |
| Chọn candidate problem | Tham gia thống nhất chọn onboarding codebase sau khi so sánh candidate của nhóm. | Nhóm chọn vấn đề có quy trình và bottleneck định lượng được, đồng thời có thể so sánh No AI/Rule/Workflow/Agent. |
| Kiểm chứng / research | Chạy quick-poll với 8 sinh viên; 7/8 (87,5%) cho biết gặp khó khăn khi trace luồng code qua nhiều file. | Có tín hiệu định lượng ban đầu ủng hộ vấn đề; mẫu nhỏ, thuận tiện, cần ghi cách hỏi và tránh khái quát cho mọi sinh viên. |
| Quy trình nhóm | Hỗ trợ Hoàng Gia Khiêm vẽ hai sơ đồ Mermaid trước/sau và nhánh fallback. | Quy trình hiện tại 180 phút, tương lai mục tiêu 90 phút; fallback dùng Call Hierarchy IDE và 10 phút mentor pair. |
| Problem Statement | Phần soạn v0/v1 do nhóm trưởng phụ trách; tôi chưa nêu đóng góp trực tiếp. | Bài toán nhóm dùng mục tiêu onboarding 180 → 90 phút, hỏi mentor ≤ 1 lần và boundary không để AI tự viết code. |
| Mức can thiệp AI | Soạn AI Canvas, trả lời hai câu hỏi Google PAIR và viết bốn tiêu chí Eval: Grounding, Accuracy, Latency, Completeness. | Cụ thể hóa cách đánh giá; các ngưỡng và bộ dữ liệu kiểm tra cần được ghi trong báo cáo nhóm. |
| Quyết định | Hỗ trợ Đặng Thanh Hải đánh giá bốn rủi ro và điều kiện pilot; nhóm thống nhất Go pilot trên 2 repo. | Kill switch: hallucination >15% hoặc thời gian tiết kiệm <40 phút thì dừng và quay về giải pháp No AI. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI sắp xếp và diễn đạt sáu vấn đề do tôi tự cung cấp theo mẫu Job Story; không nhờ AI tạo vấn đề cá nhân. | Giúp chuẩn hóa câu chữ và gắn từng vấn đề với actor, bối cảnh và dấu hiệu. | AI không thể xác nhận các trải nghiệm hoặc số liệu của tôi. | Giữ các ví dụ tôi cung cấp; đánh dấu số liệu chưa đo và không bổ sung vấn đề do AI bịa. |
| CP2 Problem Card | Nhờ AI phản biện ba card. | Chỉ ra rằng lịch/nhắc hạn hoặc bảng nhiệm vụ có thể đủ, và trợ lý gỡ lỗi có thể khiến người học chép đáp án. | Các nhận xét là giả thuyết phản biện, không tự chứng minh giải pháp nào hiệu quả. | Tôi đồng ý cả ba; thêm yêu cầu đo baseline, so sánh phương án đơn giản và giữ mục tiêu học tập. |
| CP4 Research | Dùng AI để gợi ý hướng research và các khó khăn phổ biến của sinh viên. | Giúp mở rộng hướng tìm hiểu ban đầu. | Một số thông tin chung chung, chưa gắn với trải nghiệm thật hoặc nguồn cụ thể. | Xem xét lại và tập trung vào vấn đề thực tế; không dùng gợi ý chung làm bằng chứng. |
| CP5 Quy trình | Dùng AI để gợi ý các bước của quy trình hiện tại và sắp xếp thứ tự. | Giúp tạo bản nháp trình tự để nhóm rà soát. | Một số bước chưa khớp cách sinh viên thật sự làm. | Tự chỉnh các bước để phản ánh quy trình thực tế và đóng góp vào hai sơ đồ trước/sau. |
| CP5–6 Problem Statement | Dùng AI để hỗ trợ diễn đạt Problem Statement. | Giúp làm câu chữ rõ và dễ đọc hơn. | Bản đầu quá rộng, chưa rõ actor, vấn đề và kết quả mong muốn. | Thu hẹp đối tượng, vấn đề chính và outcome; nhóm trưởng chịu trách nhiệm soạn bản cuối. |
| CP6 Mức can thiệp / quyết định | Nhờ AI soạn tiêu chí đánh giá đầu ra. | Gợi ý khung tiêu chí để bắt đầu. | Tiêu chí ban đầu chung chung và cảm tính, ví dụ “sơ đồ dễ hiểu”. | Tự đổi thành tiêu chí kỹ thuật đo được: trích dẫn đúng `filepath:linenumber` và độ trễ ≤ 15 giây. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Qua quá trình thực hiện bài tập, tôi nhận ra rằng việc xác định đúng vấn đề quan trọng hơn việc nghĩ ra một ý tưởng công nghệ thật thú vị. Ban đầu, tôi thường nghĩ đến việc sử dụng AI để giải quyết các vấn đề trong học tập. Tuy nhiên, sau khi phân tích các tình huống thực tế, tôi nhận thấy cần hiểu rõ người dùng đang gặp khó khăn gì và tại sao vấn đề đó xảy ra.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Ban đầu, nhóm có xu hướng nghĩ đến việc sử dụng AI để hỗ trợ sinh viên làm quen với codebase vì đây là một ứng dụng có vẻ hữu ích và phù hợp với xu hướng công nghệ. Tuy nhiên, nhóm nhận ra mình đang tập trung vào giải pháp trước khi xác định chính xác vấn đề người dùng gặp phải. Nhóm điều chỉnh bằng cách xem xét quy trình onboarding hiện tại, tìm hiểu những công việc người mới phải thực hiện và xác định bước khiến họ mất nhiều thời gian nhất. Qua đó, nhóm hiểu rằng vấn đề không đơn giản là sinh viên không biết lập trình, mà là họ gặp khó khăn khi hiểu cấu trúc dự án, tìm vị trí các thành phần quan trọng và theo dõi luồng hoạt động của codebase. Điều này giúp nhóm chuyển từ câu hỏi “AI có thể làm gì?” sang “Người dùng đang gặp khó khăn gì và AI có thực sự giải quyết được khó khăn đó không?”.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Ban đầu, tôi nghĩ rằng chỉ cần cung cấp một chatbot AI có khả năng trả lời câu hỏi về codebase là có thể giải quyết phần lớn khó khăn khi onboarding. Tuy nhiên, sau khi nhận phản biện rằng chatbot chỉ trả lời câu hỏi chưa chắc giúp người mới hiểu toàn bộ cấu trúc và luồng hoạt động của dự án, tôi nhận ra ý tưởng ban đầu còn khá chung chung. Người mới có thể không biết phải hỏi câu gì hoặc không biết câu trả lời của AI nằm ở file và thành phần nào trong dự án. Vì vậy, tôi thay đổi suy nghĩ: giải pháp không nên chỉ tập trung vào hỏi đáp, mà cần hướng dẫn người dùng tìm hiểu cấu trúc thư mục, xác định file quan trọng và lần theo luồng thực thi của code. Phản biện này giúp tôi hiểu rằng giải pháp AI cần gắn với quy trình thực tế của người dùng thay vì chỉ có nhiều tính năng.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Kết quả khiến tôi bất ngờ là 7/8 sinh viên được khảo sát gặp khó khăn khi trace code. Trước đó, tôi nghĩ khó khăn lớn nhất khi onboarding codebase có thể là cài đặt môi trường hoặc hiểu cú pháp của ngôn ngữ lập trình. Tuy nhiên, kết quả cho thấy việc theo dõi luồng thực thi và hiểu mối liên hệ giữa các file cũng là một trở ngại đáng kể. Tỷ lệ 7/8 cho thấy đây không chỉ là vấn đề riêng của một vài sinh viên mà có thể là nhu cầu phổ biến trong nhóm người dùng mục tiêu. Kết quả này khiến tôi nghĩ nhóm nên tập trung vào việc hỗ trợ người mới hiểu cấu trúc và luồng hoạt động của codebase, thay vì chỉ cung cấp tài liệu hoặc giải thích cú pháp.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Phần khó nhất đối với tôi là xác định và diễn đạt vấn đề đủ cụ thể mà không đưa giải pháp AI vào Problem Statement quá sớm. Ban đầu, nhóm có xu hướng mô tả vấn đề khá rộng, chẳng hạn như sinh viên gặp khó khăn khi đọc và hiểu codebase. Cách mô tả này chưa chỉ rõ ai gặp vấn đề, họ gặp khó khăn ở bước nào và vấn đề ảnh hưởng đến hiệu quả công việc ra sao. Nhóm thu hẹp phạm vi vào quá trình onboarding codebase, đặc biệt là việc tìm hiểu cấu trúc dự án và trace code. Tôi nhận ra Problem Statement cần mô tả nhu cầu và khó khăn của người dùng trước, sau đó mới xem xét AI có phù hợp hay không.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu được làm lại, tôi sẽ dành nhiều thời gian hơn để phỏng vấn và quan sát người mới onboarding trên một codebase thực tế, thay vì chỉ dựa vào nhận định ban đầu. Tôi cũng sẽ yêu cầu nhóm chia quy trình onboarding thành các bước nhỏ và đo thời gian từng bước để xác định nguyên nhân gây chậm trễ. Điểm tôi muốn phản biện nhóm là không nên mặc định mọi khó khăn trong onboarding đều cần AI giải quyết. Một số vấn đề có thể được cải thiện bằng tài liệu hướng dẫn, sơ đồ kiến trúc hoặc quy trình setup rõ ràng hơn. Nhóm cần chứng minh AI tạo giá trị bổ sung so với các phương pháp này. Ngoài ra, tôi sẽ đề xuất kiểm tra độ chính xác của câu trả lời AI và khả năng người mới tự thực hiện lại công việc sau khi được hướng dẫn.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Vấn đề nhóm lựa chọn là onboarding codebase, vì sinh viên mới thường mất nhiều thời gian để hiểu cấu trúc dự án, tìm thành phần quan trọng và trace luồng hoạt động của code. Quy trình hiện tại mất khoảng 180 phút, bao gồm đọc tài liệu, tìm hiểu cấu trúc thư mục, xác định file liên quan và lần theo luồng thực thi. Nhóm đặt mục tiêu giảm thời gian này xuống còn 90 phút và dùng tổng thời gian hoàn thành onboarding làm metric chính. Phạm vi giải pháp là hỗ trợ người mới hiểu cấu trúc, thành phần và luồng thực thi, thay vì thay thế lập trình viên hoặc tự phát triển toàn bộ dự án. AI Workflow dự kiến phân tích cấu trúc codebase, hướng dẫn tìm file và chức năng quan trọng, giải thích mối liên hệ giữa các thành phần và hỗ trợ trace luồng từng bước. Dựa trên kết quả kiểm chứng, đặc biệt là 7/8 sinh viên gặp khó khi trace code, nhóm quyết định Go để tiếp tục phát triển và kiểm chứng giải pháp.

*Lưu ý: báo cáo của Lê Nhật Linh ghi mốc 180 phút được tự bấm giờ trong đồ án trước; nhóm cần đo lại trong pilot trên hai repo.*

---

## 7. Tài liệu tham khảo

-
