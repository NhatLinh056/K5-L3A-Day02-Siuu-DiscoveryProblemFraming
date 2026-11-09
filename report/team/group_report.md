# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Siuu
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Sinh viên/người mới mất nhiều thời gian để hiểu cấu trúc và trace luồng xử lý trong codebase dự án.
- Quyết định cuối: Go — pilot trên 2 repo; dừng nếu tỷ lệ hallucination >15% hoặc thời gian tiết kiệm được <40 phút.

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Lê Nhật Linh | Khi nhận codebase mới, tôi muốn hiểu cấu trúc và luồng xử lý để bắt đầu task đúng hướng. | Developer/sinh viên mới | Trace code qua nhiều tầng mất 60 phút; onboarding tổng cộng 180 phút. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 2 | Lê Nhật Linh | Khi nhận task, tôi muốn hiểu yêu cầu và tiêu chí hoàn thành để tránh làm lại. | Developer | Chờ người giao giải thích khoảng 60 phút; làm lại có thể mất 4–6 giờ. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 3 | Lê Nhật Linh | Cuối tuần, tôi muốn tổng hợp tiến độ từ nhiều nguồn để gửi báo cáo đúng hạn. | Nhóm trưởng, thành viên | Tổng hợp khoảng 70 phút/tuần; 2/4 tuần gần nhất gửi sau 22h. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 4 | Hoàng Gia Khiêm | Khi nhận câu hỏi lặp lại, tôi muốn tìm câu trả lời chuẩn để phản hồi nhanh. | Người trả lời và người hỏi | Khoảng 15 câu/ngày, 3–5 phút/câu. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 5 | Hoàng Gia Khiêm | Sau cuộc họp, tôi muốn tạo biên bản và danh sách việc để người tham dự và vắng mặt nắm được việc cần làm. | Người ghi biên bản, người vắng họp | 3 cuộc họp/tuần, khoảng 30 phút soạn lại mỗi cuộc. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 6 | Hoàng Gia Khiêm | Trước khi gửi tài liệu duyệt, tôi muốn tự kiểm tra lỗi trình bày để giảm việc bị trả lại. | Người viết và người duyệt | Ước tính 2–3 lần bị trả về/tuần; mỗi lần người duyệt mất khoảng 15 phút và người viết sửa khoảng 20 phút. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 7 | Đặng Thanh Hải | Cuối tuần, tôi muốn lên lịch và phân phối bài viết trên nhiều kênh để tránh đăng từng bài thủ công. | Content Lead | 90–110 phút/tuần theo tự bấm giờ 3 tuần. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 8 | Đặng Thanh Hải | Khi nhận bài blog từ agency, tôi muốn soát lỗi và format để duyệt đúng hạn. | Content Lead, freelancer | 60–75 phút/bài; khoảng 3 bài/tuần. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 9 | Đặng Thanh Hải | Khi lên ý tưởng nội dung, tôi muốn gom câu hỏi/feedback độc giả để không bỏ sót pain point. | Content Lead, content team | 30–45 phút/lần; khoảng 2 lần/tuần. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 10 | Nguyễn Quốc Việt | Khi có bài tập nhiều môn với hạn khác nhau, tôi muốn sắp xếp deadline để nộp đúng hạn. | Sinh viên | Xảy ra gần như mỗi tuần; đôi khi quên bài nhỏ hoặc phát hiện hạn muộn. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 11 | Nguyễn Quốc Việt | Khi làm bài nhóm, tôi muốn chia việc và theo dõi tiến độ để mọi người hiểu trách nhiệm. | Thành viên nhóm 3–5 người | Thảo luận phân công 15–30 phút; điều phối/cập nhật/ghép phần ước tính 1–2 giờ/dự án. | Chưa ghi nhận câu hỏi nhóm nhận được. |
| 12 | Nguyễn Quốc Việt | Khi gặp lỗi lập trình, tôi muốn hiểu nguyên nhân và sửa để hoàn thành bài và học cách debug. | Sinh viên lập trình | Một lỗi khó có thể mất 20–60 phút. | Chưa ghi nhận câu hỏi nhóm nhận được. |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Hiểu và tìm thông tin | Onboarding codebase; task thiếu tiêu chí; câu hỏi lặp lại; biên bản họp; tự kiểm tra tài liệu; tìm thông tin học tập; gỡ lỗi | Người dùng khó tìm, hiểu hoặc kiểm chứng thông tin trong nhiều file/tài liệu. *(Phân cụm dự thảo, nhóm cần xác nhận.)* |
| B — Điều phối và theo dõi công việc | Báo cáo tiến độ; deadline bài tập; điều phối bài nhóm | Thông tin phân tán, cần tổng hợp trạng thái, trách nhiệm hoặc thời hạn. *(Phân cụm dự thảo, nhóm cần xác nhận.)* |
| C — Vận hành nội dung | Lên lịch nội dung; review bài agency; tìm ý tưởng từ feedback | Lặp lại các bước sản xuất, kiểm tra và khai thác phản hồi nội dung. *(Phân cụm dự thảo, nhóm cần xác nhận.)* |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian onboarding codebase từ 180 phút xuống 90 phút
├── Opportunity A: Người mới cần hiểu nhanh cấu trúc và vai trò các module trong repo.
├── Opportunity B: Người mới khó trace luồng xử lý của use-case qua nhiều file/tầng.
└── Opportunity C: Người mới cần kiểm chứng lời giải thích và có lối thoát khi thông tin không khớp với code.
```

*Cây trên là bản nháp suy luận từ candidate được chọn, 2 phỏng vấn và quick-poll; nhóm cần xác nhận wording cơ hội.*

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- “AI tự viết code” là giải pháp, không phải opportunity; nhóm giới hạn đề xuất ở giải thích luồng và hỗ trợ trace code.
- “Dùng agent tự động sửa toàn bộ repo” là giải pháp vượt quá nhu cầu xác định luồng; cần xác nhận bằng pilot trước khi mở rộng.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

*Điểm số và tên các candidate trong shortlist chưa có trong ghi chú nhóm; cần nhóm trưởng bổ sung, không suy đoán điểm.*

**Candidate được chọn:** Sinh viên/developer mới mất nhiều thời gian để hiểu cấu trúc và trace luồng xử lý trong codebase dự án.

**Vì sao chọn:** Có quy trình và bottleneck đo được (180 phút tổng onboarding, 60 phút trace); quick-poll sau đó ghi nhận 7/8 sinh viên gặp khó khi trace code qua nhiều file. Nhóm có thể so sánh giải pháp tài liệu/Rule/Workflow và kiểm chứng trong pilot 2 repo.

**Vì sao loại các candidate còn lại:** Chưa có ghi chú nêu lý do loại từng candidate; cần nhóm trưởng bổ sung căn cứ thảo luận.

**Xử lý bất đồng (nếu có):** Chưa ghi nhận bất đồng hoặc cách xử lý cụ thể.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Người mới mất nhiều thời gian để hiểu cấu trúc và trace luồng code. | Value | Chưa chấm | Khảo sát 8 sinh viên và 2 phỏng vấn; mẫu nhỏ, cần pilot đo thời gian thật. | Có — đối chiếu với repo mới và trace task cụ thể. |
| 2 | AI có thể tạo sơ đồ luồng code chính xác, có ích cho use-case. | Feasibility | Chưa chấm | Người được hỏi lo AI bịa file/hàm; một lần sai có thể làm tăng 45 phút debug. | Có — kiểm tra citation và đối chiếu code thật. |
| 3 | Người mới hiểu và kiểm chứng được sơ đồ AI tạo ra. | Usability | Chưa chấm | Chưa có thử nghiệm usability; thiết kế yêu cầu dev đặt breakpoint. | Có — quan sát người mới dùng và sửa đầu ra. |
| 4 | Workflow có thể giảm onboarding 180 → 90 phút mà không tăng lỗi. | Value / Feasibility | Chưa chấm | Hiện là mục tiêu; chưa có kết quả pilot. | Có — pilot trên 2 repo và đo thời gian/lỗi. |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này: sinh viên/người mới gặp khó khăn khi trace luồng code giữa nhiều file; AI có thể giúp nếu giải thích dựa trên code và người dùng kiểm chứng được. Bằng chứng hiện tại là quick-poll 8 người và 2 cuộc phỏng vấn; đây chưa phải bằng chứng đại diện cho toàn bộ sinh viên.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Chưa có ghi chú riêng theo từng người; tổng cộng 2 sinh viên IT. |
| Câu nói đáng nhớ nhất (nguyên văn) | Chưa cung cấp trích dẫn nguyên văn; không ghi lại dưới dạng quote. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Chưa có tường thuật riêng theo từng người. |
| Hiện đang xử lý bằng cách nào (workaround)? | Chưa có ghi chú riêng về workaround. |
| Mất bao lâu, bao lần? | Một tín hiệu phỏng vấn: người học lo AI bịa tên file/hàm khiến họ mất thêm khoảng 45 phút debug. Chưa rõ đây là trải nghiệm đã xảy ra hay lo ngại giả định; cần xác nhận từ ghi chú phỏng vấn. |
| Insight / opportunity rút ra | Cần kiểm chứng độ bám nguồn của lời giải thích và có fallback rõ khi AI nêu file/hàm không tồn tại. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn Mom Test | 2 sinh viên IT | Tín hiệu: lo AI bịa file/hàm và tăng thời gian debug; chưa đủ dữ liệu để kết luận nhu cầu sử dụng. | Chưa có tín hiệu phản bác riêng được ghi lại. |
| Quick-poll tại lớp (mẫu thuận tiện) | 8 sinh viên | 7/8 (87,5%) cho biết gặp khó khi trace luồng code qua nhiều file. | 1/8 không chọn câu trả lời cho biết gặp khó khăn; câu hỏi và cách ghi nhận cần lưu kèm để diễn giải chính xác. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Bổ sung rủi ro lời giải thích bịa file/hàm, yêu cầu dev kiểm tra bằng breakpoint, và thiết kế fallback dùng Call Hierarchy của IDE cùng 10 phút mentor pair. Cần bổ sung snapshot phỏng vấn và nguyên văn câu hỏi poll để hoàn thiện dấu vết kiểm chứng.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Cursor | [Tính năng chính thức](https://www.cursor.com/features) | Hỗ trợ hiểu codebase và cung cấp ngữ cảnh khi làm việc với mã. | Tích hợp hỗ trợ AI trực tiếp trong trình soạn thảo. | Nhóm ghi nhận còn thiếu sơ đồ trực quan theo use-case task; cần kiểm tra điều này trên các use-case thử nghiệm của nhóm. | Không giả định AI explanation thay thế call graph hoặc kiểm chứng của dev. |
| GitHub Copilot | [Trang sản phẩm chính thức](https://github.com/features/copilot) | Hỗ trợ hiểu repo, lập kế hoạch, chỉnh sửa và review code trong quy trình phát triển. | Tích hợp với repo, issue và pull request. | Khả năng rộng có thể vượt nhu cầu giải thích luồng; nhóm cần kiểm thử mức citation và độ chính xác cho từng đường đi qua file. | Dùng như đối chứng sản phẩm; giữ người phát triển kiểm tra và quyết định. |
| Mintlify | [Nền tảng tài liệu chính thức](https://www.mintlify.com/) | Tạo và duy trì tài liệu kỹ thuật cho sản phẩm. | Có thể giúp chuẩn hóa tài liệu onboarding và tài liệu dự án. | Tài liệu tĩnh có thể không bao quát đường đi của một use-case qua code; cần phân biệt khoảng trống tài liệu với khoảng trống AI. | Chuẩn hóa README/sơ đồ trước; AI chỉ bổ sung khi tài liệu và công cụ tĩnh chưa đủ. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — tổng cộng khoảng 180 phút

[1 Nhận repo và task: 5'] → [2 Đọc README/tài liệu cài đặt: 15']
→ [3 Xem cấu trúc thư mục và config: 20'] → [4 Tìm module liên quan: 30']
→ [5 Đọc code, trace Controller → Service → Repository: 60'] ← BOTTLENECK
→ [6 Chạy thử và debug: 30'] → [7 Hỏi lead xác nhận: 20']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Developer mới | Repo và task | Nắm phạm vi task | 5 phút | Nhận bàn giao |
| 2 | Developer mới | Repo, README, hướng dẫn cài đặt | Môi trường và hướng dẫn ban đầu | 15 phút | Tài liệu có thể chưa có sơ đồ use-case |
| 3 | Developer mới | Cây thư mục, file config | Xác định cấu trúc repo | 20 phút | Phải tự tìm module liên quan |
| 4 | Developer mới | Mô tả task, cây thư mục | Danh sách module/file liên quan | 30 phút | Chưa rõ đường đi qua các tầng |
| 5 | Developer mới | Code nhiều tầng | Hiểu luồng gọi hàm của use-case | 60 phút | Bottleneck chính: trace thủ công qua Controller → Service → Repository |
| 6 | Developer mới | Mã và môi trường local | Kết quả chạy thử, lỗi được phát hiện | 30 phút | Kiểm chứng hành vi trên máy |
| 7 | Developer mới, lead | Câu hỏi chưa rõ | Xác nhận luồng nghiệp vụ | 20 phút | Linh nêu 3–4 lần hỏi lead cho một lần onboarding; cần đối chiếu cách tính |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — mục tiêu tổng thời gian onboarding khoảng 90 phút

[1 Nhận repo và task]
→ [2 Đọc README/sơ đồ kiến trúc đã chuẩn hóa]
→ [3 Dùng Call Hierarchy và AI Workflow để tạo nháp luồng theo use-case]
→ [4 Developer mở các filepath:linenumber, đặt breakpoint và kiểm chứng — HITL]
→ [5 Bắt đầu task đầu tiên]
   Nếu AI nêu file/hàm không tồn tại hoặc luồng không khớp:
   [Fallback: Call Hierarchy của IDE + 10 phút mentor pair]

Boundary: AI chỉ giải thích và gợi ý sơ đồ; không tự viết code hoặc quyết định thay developer.
Thời lượng chi tiết từng bước cần chép từ sơ đồ Mermaid gốc của người phụ trách quy trình.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 7 | 5 bước chính + 1 nhánh fallback có điều kiện | Bản tóm tắt; cần đối chiếu sơ đồ Mermaid gốc |
| Tổng thời gian | 180 phút | Mục tiêu 90 phút | Mục tiêu giảm 50%, chưa có kết quả pilot |
| Số bước thủ công | 7 bước hiện tại | Chưa thống nhất | Developer vẫn phải tự kiểm chứng và thực hiện task |
| Bottleneck chính | Trace code qua nhiều tầng: 60 phút | AI tạo nháp luồng có dẫn nguồn; developer xác minh | Cần đo lại thời gian ở pilot |
| Rủi ro mới phát sinh | Không có AI hallucination trong quy trình hiện tại | Bịa file/hàm/luồng, có thể tăng 45 phút debug | Bắt buộc dẫn nguồn, đặt breakpoint, có fallback |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên hoặc developer mới tiếp nhận repo dự án có khoảng 30–50 file mã nguồn. |
| **Quy trình** | Từ lúc nhận repo và task đầu tiên đến khi hiểu luồng liên quan, chạy thử và bắt đầu thực hiện task. |
| **Bottleneck** | Đọc code và trace luồng gọi hàm qua Controller → Service → Repository; hiện ước tính 60 phút vì thiếu sơ đồ call graph theo use-case. |
| **Impact** | Onboarding mất khoảng 180 phút; cần hỏi mentor/lead 3–4 lần; hiểu sai luồng có thể dẫn đến 2–3 bug khi merge và 2–4 giờ refactor (ước tính từ báo cáo cá nhân, cần đo trong pilot). |
| **Success Metric** (baseline → target, cách đo) | Tổng thời gian onboarding 180 → ≤90 phút; thời gian trace luồng 60 → ≤25 phút; số lần hỏi mentor/lead 3–4 → ≤1 lần/task. Bấm giờ từ lúc nhận repo đến khi chạy thử task đầu tiên và ghi số lần hỏi. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI không tự viết hoặc sửa code, không tự quyết định thay developer. Developer phải mở và kiểm tra filepath:linenumber, đặt breakpoint để xác nhận hành vi; khi lời giải thích không khớp thì chuyển sang Call Hierarchy và mentor pair. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- AI cảnh báo mục tiêu giảm 50% thời gian chưa có cơ sở. Nhóm trưởng cho biết đã tính lại tác động dây chuyền qua 4 bước trong bảng Before/After; cần đưa phép tính và giả định vào bảng để người đọc kiểm tra.
- Phỏng vấn nêu rủi ro AI bịa tên file/hàm, có thể làm tăng khoảng 45 phút debug. Nhóm đồng ý thêm citation, bước developer đặt breakpoint và fallback thủ công.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ phức tạp cao, độ mơ hồ trung bình** (nhận định sơ bộ của nhóm).

Vì sao: Repo có nhiều file và luồng gọi qua nhiều tầng; đầu ra cần gắn với task/use-case cụ thể. Code có cấu trúc để kiểm chứng bằng công cụ và developer nên không hoàn toàn mơ hồ. Cần kiểm tra nhận định này trong pilot.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Chuẩn hóa README, sơ đồ kiến trúc C4/Mermaid, pair walkthrough 20 phút. | Nếu tài liệu và walkthrough giúp đạt metric. | Tài liệu có thể lỗi thời, không trả lời câu hỏi riêng của use-case. | Không chọn làm mức duy nhất; dùng làm nền. |
| **Rule** | Call Hierarchy/call graph tĩnh từ IDE. | Khi cần xem cấu trúc gọi hàm có thể suy ra tĩnh. | Không giải thích đầy đủ nghiệp vụ hoặc luồng động. | Dùng trong quy trình và fallback. |
| **Workflow** | AI tạo nháp giải thích luồng theo task/use-case, kèm nguồn; developer kiểm chứng bằng code và breakpoint. | Khi tra cứu lặp lại nhưng quyết định và kiểm tra vẫn do developer làm. | Hallucination về file/hàm; nguồn sai; người mới có thể tin quá mức. | **Chọn — pilot có HITL và fallback.** |
| **Agent** | Agent tự khám phá repo, tự chọn bước và có thể sửa code. | Chỉ khi cần tự điều phối nhiều bước và có kiểm soát phù hợp. | Vượt nhu cầu; khó kiểm soát; nguy cơ sửa code sai. | Không chọn. |

**Mức chọn:** Workflow.

**Vì sao không chọn mức đơn giản hơn:** Tài liệu chuẩn và Call Hierarchy vẫn cần thiết, nhưng chưa chắc giải thích được luồng của use-case cụ thể. Workflow thêm bước tạo giải thích theo task, nhưng giữ con người xác minh; nếu pilot cho thấy tài liệu/Rule đã đủ thì quay về mức đơn giản hơn.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Nháp sơ đồ/giải thích đường đi của use-case qua file, module và hàm trong repo. |
| **Judgment** — con người cân nhắc, quyết định gì? | Developer xác nhận đường đi có đúng code và task không; quyết định bước tiếp theo. |
| **Action** — hành động cuối cùng là gì, ai làm? | Developer tự điều hướng code, đặt breakpoint, chạy thử và làm task; AI không tự viết code. |
| **Outcome** — đo kết quả bằng gì? | Thời gian onboarding 180 → ≤90 phút; trace 60 → ≤25 phút; hỏi mentor ≤1 lần/task; theo dõi hallucination. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Repo/code, task hoặc use-case, README và call hierarchy; có sẵn trong pilot repo nhưng cần kiểm soát quyền truy cập. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Developer ghi nhận nguồn sai, bước bị bỏ sót và thời gian xác minh trong mỗi pilot task; lưu bộ test đã kiểm chứng. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: Chọn augment — developer dùng lời giải thích làm gợi ý rồi tự kiểm tra bằng code và breakpoint; AI không được giao quyền viết code.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: Trong pilot, bịa file/hàm/đường đi có thể làm người mới mất thêm khoảng 45 phút debug (tín hiệu phỏng vấn). Thiết kế yêu cầu citation, developer xác minh và fallback Call Hierarchy + 10 phút mentor pair; đây là tín hiệu từ mẫu nhỏ.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên/developer mới nhận repo dự án khoảng 30–50 file. |
| **Quy trình** | Nhận repo và task → đọc tài liệu → tìm module → trace luồng → chạy thử/debug → thực hiện task đầu tiên. |
| **Bottleneck** | Trace luồng xử lý qua nhiều file/tầng, hiện khoảng 60 phút. |
| **Impact** | Onboarding khoảng 180 phút; 3–4 lần hỏi mentor/lead; sai luồng có thể gây bug và làm lại. |
| **Success Metric** (baseline → target, cách đo) | Tổng onboarding 180 → ≤90 phút; trace 60 → ≤25 phút; hỏi mentor 3–4 → ≤1 lần/task. Bấm giờ trên 2 repo pilot; kết quả chưa có. |
| **Boundary** | AI không tự viết/sửa code hoặc tự quyết định thay developer; mọi claim về luồng phải có filepath:linenumber và được kiểm tra bằng breakpoint. |
| **AI intervention point** | Sau khi xác định task/use-case và trước khi developer tự trace: AI tạo nháp luồng qua các file/hàm; developer kiểm chứng rồi mới dùng. |
| **Mức chọn** | Workflow |
| **Rủi ro & người kiểm tra** | AI bịa hoặc bỏ sót file/hàm/đường đi; developer mới kiểm tra citation và breakpoint, mentor hỗ trợ khi fallback. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| AI intervention point / boundary | AI chưa được tích hợp cụ thể ở v0; nguyên tắc không để AI tự viết code đã nêu. | Workflow tạo nháp luồng có citation; developer xác minh bằng breakpoint, AI không tự sửa code. | Sau khi so sánh No AI/Rule/Workflow/Agent và phản ánh rủi ro hallucination. |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Grounding — dẫn nguồn | Mỗi khẳng định về luồng gắn filepath:linenumber tồn tại và trỏ đúng vị trí. | Thiếu citation, sai đường dẫn hoặc dòng không hỗ trợ khẳng định. |
| 2 | Accuracy — độ chính xác | Không bịa file/hàm hoặc thứ tự gọi; đối chiếu với luồng chuẩn do developer xác minh. | Hallucination >15% trên bộ eval/pilot. |
| 3 | Latency — độ trễ | Thời gian tạo giải thích ≤15 giây. | Vượt quá 15 giây. |
| 4 | Completeness — độ đầy đủ | Có đủ các bước quan trọng của use-case trong luồng tham chiếu. | Bỏ sót một bước quan trọng hoặc không nối được các tầng liên quan. |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Trung bình | 7/8 poll gặp khó khi trace code qua nhiều file; chỉ 2 phỏng vấn. Chưa có bằng chứng về willingness to use. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Cao | Người được phỏng vấn lo file/hàm bịa làm tăng khoảng 45 phút debug; cần citation, breakpoint và mentor fallback. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Trung bình | Có repo, IDE và workflow để thử; độ chính xác citation/luồng chưa được pilot xác nhận. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Trung bình — cần kiểm chứng | Pilot giới hạn 2 repo; chi phí mô hình, quyền truy cập code và người duy trì chưa được đánh giá. |

### 8.2. Kết luận

**Quyết định:** Go — pilot giới hạn trên 2 repo.

**Lý do:** Poll 8 sinh viên có 7 phản hồi gặp khó khăn khi trace code; nhóm có thể đo hiệu quả trên repo thật và giữ con người trong vòng kiểm tra. Bằng chứng hiện tại còn nhỏ và chưa chứng minh mức giảm thời gian hoặc độ chính xác, nên chỉ Go cho pilot.

**Nếu Go — pilot nhỏ nhất:** Thử workflow trên 2 repo; ghi thời gian onboarding, thời gian trace, số lần hỏi mentor, citation đúng/sai và hallucination. Developer xác minh mọi luồng bằng breakpoint; dùng Call Hierarchy + 10 phút mentor pair khi AI sai hoặc không đủ.

**Nếu Not Yet — cần kiểm chứng gì trước:** Không áp dụng cho quyết định hiện tại; nếu pilot không đạt ngưỡng thì dừng theo kill switch.

**Nếu No-Go — nên làm gì thay AI:** Không áp dụng cho quyết định hiện tại; quay về README/sơ đồ kiến trúc, Call Hierarchy của IDE và mentor pair.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …): Nếu hallucination >15% trên bộ eval/pilot hoặc thời gian tiết kiệm được <40 phút so với baseline, dừng AI Workflow và quay về tài liệu chuẩn + Call Hierarchy IDE + mentor pair.

---

## 9. Hạn chế và hướng tiếp theo

- Quick-poll chỉ có 8 sinh viên cùng lớp/nhóm ngồi gần; kết quả 7/8 chưa đại diện cho toàn bộ sinh viên.
- Hai phỏng vấn chưa có snapshot riêng, trích dẫn nguyên văn hoặc workaround được lưu trong repo; cần bổ sung từ ghi chú thật, không dựng lại từ trí nhớ nếu không chắc.
- Các mốc 180 phút, 60 phút trace, 3–4 lần hỏi mentor và mục tiêu 90 phút hiện dựa trên ước tính/báo cáo cá nhân; cần đo đồng nhất trong pilot.
- Bộ Eval cần có các task/use-case mẫu và luồng tham chiếu do developer xác minh để tính grounding, accuracy, completeness và hallucination.
- Bước tiếp theo: chạy pilot trên 2 repo, ghi thời gian và lỗi theo cùng cách đo, kiểm tra quyền truy cập code và đối chiếu hiệu quả với tài liệu/Call Hierarchy không AI.

## 10. Tài liệu tham khảo

- [Cursor — Tính năng](https://www.cursor.com/features)
- [GitHub Copilot — Trang sản phẩm](https://github.com/features/copilot)
- [Mintlify — Nền tảng tài liệu](https://www.mintlify.com/)
