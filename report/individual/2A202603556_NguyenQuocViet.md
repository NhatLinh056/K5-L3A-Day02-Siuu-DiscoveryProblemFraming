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
| 2 | Lặp lại | Khi có nhiều bài tập ở các môn với hạn nộp khác nhau, tôi muốn sắp xếp công việc và hạn nộp, để hoàn thành mọi bài đúng hạn. | Sinh viên học nhiều môn | Xảy ra gần như mỗi tuần; đôi khi quên bài nhỏ hoặc phát hiện hạn nộp muộn. Chưa có số lần cụ thể. |
| 3 | Tốn thời gian; pain từ người khác | Khi làm bài nhóm với 3–5 bạn cùng lớp, tôi muốn chia việc và theo dõi tiến độ, để mọi thành viên hiểu trách nhiệm của mình. | Tất cả thành viên nhóm | Hầu hết bài tập nhóm; dành khoảng 15–30 phút thảo luận phân công; đôi khi thành viên hiểu khác nhau về trách nhiệm. |
| 4 | Tốn thời gian | Khi làm bài lập trình bằng Python, Java hoặc ngôn ngữ khác, tôi muốn tìm nguyên nhân và sửa lỗi nhanh, để hoàn thành bài và dành thời gian hiểu nội dung khác. | Sinh viên học lập trình, lập trình viên | Vài lần mỗi tuần; một lỗi cú pháp hoặc logic nhỏ có thể mất 20–60 phút để tìm. |
| 5 | Tốn thời gian | Khi giảng viên trình bày khái niệm nhanh, tôi muốn ghi lại ý chính mà vẫn theo kịp bài giảng, để không bỏ lỡ nội dung quan trọng. | Sinh viên | Vài lần mỗi tuần; đôi khi bỏ lỡ ý mới vì còn đang ghi phần trước. Chưa đo thời lượng hoặc số lần bỏ lỡ. |
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
| Thời điểm / bối cảnh | Gần như mỗi tuần khi nhận thông báo bài tập từ giảng viên và các nền tảng/nhóm lớp khác nhau. |
| Quy trình hiện tại (3–7 bước) | 1. Nhận thông tin bài tập từ giảng viên. 2. Kiểm tra hạn trên nền tảng học tập hoặc nhóm lớp. 3. Ghi hạn vào ghi chú hoặc lịch. 4. Xếp thứ tự ưu tiên. 5. Làm bài. 6. Kiểm tra và nộp trước hạn. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Tổng hợp và nhớ hạn từ nhiều nền tảng; Việt ước tính mất khoảng 10–15 phút mỗi tuần, chưa tính thời gian/hậu quả khi quên bài. Chưa tách thời gian từng bước. |
| Impact (nếu không giải thì sao) | Có thể nộp trễ, giảm điểm, căng thẳng và quản lý thời gian kém. |
| Success metric (baseline → target) | Baseline hiện biết: đôi khi quên bài nhỏ hoặc phát hiện hạn muộn; chưa có tỷ lệ cụ thể. Target: 100% bài tập được ghi nhận và nộp đúng hạn. Đo bằng cách đối chiếu danh sách bài tập với nền tảng môn học và thời điểm nộp trong một giai đoạn theo dõi; cần bổ sung baseline bằng số liệu. |
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
| Success metric (baseline → target) | Baseline ước tính: 20–60 phút cho một lỗi khó. Target: dưới 10 phút cho các lỗi phổ biến. Đo thời gian từ lúc gặp lỗi đến khi hiểu nguyên nhân, sửa và xác nhận đầu ra; cần định nghĩa nhóm lỗi phổ biến. |
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
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
