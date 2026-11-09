# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Siuu
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi tiếp nhận dự án phần mềm mới, developer mới muốn hiểu nhanh cấu trúc mã nguồn và luồng xử lý chính của module cần sửa, để bắt đầu thực hiện task đầu tiên mà không làm gián đoạn công việc của mentor/đồng nghiệp.
- Quyết định cuối: Go / Not Yet / No-Go (sẽ chốt ở CP6)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

|   # | Người đưa ra  | Candidate (Job Story ngắn)                                                                                                              | Actor                    | Bottleneck                                                                      | Câu hỏi phản biện nhận được (ai hỏi)                                                                                |
| --: | ------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
|   1 | Lê Nhật Linh  | Khi tiếp nhận dự án mới, dev mới muốn hiểu cấu trúc và luồng xử lý code, để làm task chính xác.                                         | Developer mới            | Đọc code và trace luồng gọi hàm giữa các tầng (60' trên tổng 180' onboarding).   | "AI chỉ giảm bước 5 được 35', vậy 55' còn lại để đạt 180' → 90' giảm ở đâu?" (Hoàng Gia Khiêm hỏi)                |
|   2 | Lê Nhật Linh  | Khi nhận task chưa rõ ràng, dev muốn hiểu đúng tiêu chí hoàn thành, để tránh bị reject khi review code.                                 | Developer, thành viên    | Chờ phản hồi giải thích yêu cầu từ người giao task (60' chờ trên tổng 210').    | "Vấn đề này do người giao thiếu template hay do dev chưa chủ động research?" (Đặng Thanh Hải hỏi)                   |
|   3 | Lê Nhật Linh  | Khi đến kỳ báo cáo tuần, nhóm trưởng muốn tổng hợp tiến độ, để nộp báo cáo đúng hạn.                                                    | Trưởng nhóm, thành viên  | Thu thập và nhắc các thành viên gửi cập nhật (20' trên tổng 70').                | "Jira và GitHub Projects đã có dashboard số liệu, tại sao khâu này vẫn mất 70 phút?" (Hoàng Gia Khiêm hỏi)         |
|   4 | Đặng Thanh Hải| Khi tới thứ Sáu, Content Lead muốn lên lịch phân phối 10-12 bài viết lên Facebook, LinkedIn, Blog, để không đăng thủ công.             | Content Lead             | Copy/paste và định dạng từng kênh (45' trên tổng 95').                           | "Buffer và Hootsuite đã hỗ trợ lên lịch đa kênh bằng Rule/API, AI tạo thêm giá trị gì ở đây?" (Lê Nhật Linh hỏi)    |
|   5 | Đặng Thanh Hải| Khi nhận bài blog 2.000 từ từ agency, Content Lead muốn soát lỗi diễn đạt và chuẩn SEO, để duyệt bài đúng hạn.                          | Content Lead             | Đọc kỹ và viết nhận xét chi tiết (55' trên tổng 60'/bài).                       | "Tại sao không bắt agency tự chạy checklist format/chính tả trước khi nộp mà Lead phải tốn 60' sửa thay? Lỗi quy trình hay cần AI?" (Lê Nhật Linh hỏi) |
|   6 | Đặng Thanh Hải| Khi cần lên idea bài viết mới, Content Lead muốn gom nhóm thắc mắc của độc giả, để không bỏ sót pain point.                            | Content Lead             | Lọc thủ công qua nhiều luồng bình luận/chat (35' trên tổng 45').                 | "Nếu số lượng comment ít (vài chục cái), dùng bảng tính Google Sheets filter có nhanh hơn không?" (Hoàng Gia Khiêm hỏi) |
|   7 | Hoàng Gia Khiêm| Khi đồng nghiệp hỏi câu trùng lặp (quy trình, giá, hạn), người phụ trách muốn có câu trả lời chuẩn, để không gõ lại từ đầu.          | Người trực tiếp trả lời  | Tìm lại thông tin và gõ lại câu trả lời (3.5' trên tổng 4'/câu).                | "Đã có quick reply/snippet trên Zalo/Slack, sao cần AI nháp lại từng câu?" (Đặng Thanh Hải hỏi)                     |
|   8 | Hoàng Gia Khiêm| Khi họp xong, người ghi biên bản muốn có ngay tóm tắt việc và hạn chót, để không mất công nghe lại ghi âm.                             | Người ghi biên bản       | Nghe lại ghi âm để không sót ý (12' trên tổng 30'/buổi).                        | "Ghi âm cuộc họp đưa lên AI có vi phạm bảo mật thông tin nội bộ của nhóm không?" (Lê Nhật Linh hỏi)                 |
|   9 | Hoàng Gia Khiêm| Khi chuẩn bị gửi tài liệu cho sếp duyệt, nhân viên muốn tự kiểm tra lỗi format và số liệu, để giảm số lần bị trả về.                   | Nhân viên làm văn bản    | Soát thủ công từng trang theo quy định (15'/bản).                               | "Tiêu chí bắt lỗi của sếp có định lượng thành rule rõ ràng được không hay phụ thuộc cảm tính?" (Đặng Thanh Hải hỏi) |
|  10 | Nguyễn Quốc Việt| Khi nhiều môn giao bài với hạn khác nhau, sinh viên muốn theo dõi hạn nộp, để hoàn thành đúng hạn.                                      | Sinh viên học nhiều môn  | Tổng hợp và nhớ hạn từ nhiều nền tảng (10–15'/tuần).                            | "Google Calendar và tính năng nhắc hẹn của LMS đã giải quyết tự động việc này rồi, sao cần AI?" (Lê Nhật Linh hỏi)   |
|  11 | Nguyễn Quốc Việt| Khi làm bài tập nhóm 3–5 người, thành viên muốn chia việc và theo dõi tiến độ, để hoàn thành bài hiệu quả.                             | Thành viên nhóm bài tập  | Thu thập cập nhật tiến độ và ghép các phần (1–2h/dự án).                        | "Dùng bảng Kanban Trello/Notion kết hợp họp nhanh 10' có nhanh hơn là đợi AI điều phối không?" (Đặng Thanh Hải hỏi) |
|  12 | Nguyễn Quốc Việt| Khi làm bài lập trình gặp lỗi, sinh viên muốn hiểu nguyên nhân và sửa lỗi, để hoàn thành bài mà vẫn học được cách debug.               | Sinh viên học lập trình  | Tìm hiểu nguyên nhân gốc của lỗi khó (20–60'/lỗi).                              | "Làm sao đảm bảo AI giải thích bản chất lỗi để sinh viên hiểu bài chứ không chỉ đưa đáp án chép vẹt?" (Hoàng Gia Khiêm hỏi) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
| ------- | ------------- | ------------- |
| A — Đọc hiểu Kỹ thuật & Gỡ lỗi Mã nguồn | #1 (Tìm hiểu codebase dự án mới), #12 (Gỡ lỗi lập trình sinh viên) | Người mới/sinh viên tiếp cận hệ thống mã nguồn hoặc lỗi phức tạp, tài liệu/thông báo lỗi khó hiểu, tốn 30–60 phút đọc code và tìm nguyên nhân gốc. |
| B — Kiểm duyệt & Soát lỗi Nội dung / Văn bản | #5 (Review bài blog agency), #9 (Soát lỗi tài liệu trước khi duyệt) | Người kiểm duyệt phải đọc lượng lớn văn bản để bắt lỗi ngữ pháp, format, chính tả và chuẩn quy định; tốn nhiều thời gian đọc rà soát thủ công. |
| C — Tổng hợp Thông tin, Điều phối & Giao tiếp lặp lại | #2 (Task không rõ), #3 (Báo cáo tuần), #4 (Lên lịch đa kênh), #6 (Gom feedback), #7 (Câu hỏi trùng lặp), #8 (Biên bản họp), #10 (Theo dõi hạn nộp), #11 (Điều phối bài nhóm) | Dữ liệu bị phân tán ở nhiều kênh (chat, tool, họp), thao tác thu thập/phản hồi thủ công lặp lại nhiều lần gây gián đoạn công việc chính. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian Developer mới cần để bắt đầu hoàn thành task đầu tiên trong dự án từ 180 phút xuống ≤ 90 phút
├── Opportunity A: Khó xác định luồng xử lý chính và điểm chạm giữa các tầng (Route → Controller → Service → Database) trong codebase lớn
├── Opportunity B: Tài liệu dự án (README, Wiki) sơ sài, thiếu sơ đồ luồng dữ liệu hoặc đã lỗi thời so với code thực tế
└── Opportunity C: Mentor và đồng nghiệp bận rộn, thời gian chờ phản hồi hướng dẫn kéo dài gây nghẽn tiến độ làm task
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ *"Xây dựng Chatbot AI trả lời tự động mọi thắc mắc về mã nguồn"* (Solution trá hình đội lốt, gạch bỏ)
- ✗ *"Plugin tự động sinh tài liệu code bằng AI Agent"* (Solution trá hình đội lốt, gạch bỏ)
- ✗ *"Dashboard trực quan hóa kiến trúc codebase"* (Solution trá hình đội lốt, gạch bỏ)

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| --------- | -------: | -----------: | -----------------: | -------------: | ----------: | -------------------------------------: | ---------------: | ---: |
| 1. Tìm hiểu codebase mới khi tiếp nhận dự án (Linh #1) | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| 2. Trợ lý gỡ lỗi lập trình sinh viên (Việt #3) | 4 | 4 | 5 | 4 | 4 | 4 | 5 | **30** |
| 3. Review/soát lỗi bài viết blog agency (Hải #2) | 4 | 5 | 4 | 4 | 4 | 3 | 4 | **28** |

**Candidate được chọn:**
`Tìm hiểu codebase mới khi tiếp nhận dự án (Candidate #1 của Lê Nhật Linh).`

**Vì sao chọn:**
1. **Actor rõ & đo được:** Developer mới / thực tập sinh IT; bottleneck trace code giữa các tầng mất 60' trên tổng 180' onboarding task đầu.
2. **Hiểu sâu domain:** Cả 4 thành viên đều học CNTT/lập trình, có sẵn số liệu bấm giờ thật từ đồ án để kiểm chứng ngay.
3. **Đất diễn 4 mức can thiệp:** So sánh rành mạch No AI (README + C4 model), Rule (linter/grep), Workflow (LLM sinh call-graph theo use-case + dev tự debug xác minh) và Agent (tự duyệt toàn bộ repo).

**Vì sao loại các candidate còn lại:**
- **Loại bài Gỡ lỗi code (Việt):** Phạm vi lỗi lập trình quá rộng; rủi ro sinh viên ỷ lại chép code sửa sẵn thay vì học bản chất lỗi, ranh giới an toàn (boundary) khó kiểm soát trong 1 buổi lab.
- **Loại bài Review blog (Hải):** 70% vấn đề giải quyết được bằng Rule (bắt agency điền checklist nghiệm thu trước khi nộp); tiêu chuẩn "brand voice" định tính, khó đo lường chính xác.

**Xử lý bất đồng (nếu có):**
- Cả 4 thành viên thống nhất chọn bài Codebase vì có baseline đo lường bằng phút cụ thể (180' → 90') và khớp năng lực kỹ thuật của cả nhóm.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
