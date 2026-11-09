# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: Siuu
- Candidate problem nhóm chọn (1 câu): Khi tiếp nhận dự án phần mềm mới, developer mới muốn hiểu nhanh cấu trúc mã nguồn và luồng xử lý chính của module cần sửa, để bắt đầu thực hiện task đầu tiên mà không làm gián đoạn công việc của mentor/đồng nghiệp.
- Quyết định cuối (Go / Not Yet / No-Go): Go (phạm vi pilot nhỏ)

## Thành viên

| STT | Họ và tên        | MSSV        | Vai trò trong nhóm     | Tài khoản GitHub |
| --: | ---------------- | ----------- | ---------------------- | ---------------- |
|   1 | Lê Nhật Linh     | 2A202603514 | Nhóm trưởng, điều phối | NhatLinh056      |
|   2 | Đặng Thanh Hải   | 2A202603570 | Phản biện, kiểm chứng  | haidangbk        |
|   3 | Hoàng Gia Khiêm  | 2A202603540 | Research, quy trình    | KhiemHG          |
|   4 | Nguyễn Quốc Việt | 2A202603556 | Phản biện, kiểm chứng  | vietnq           |

## Phân công theo checkpoint

| Checkpoint                      | Người chính     | Người hỗ trợ     | Sản phẩm                                                                  |
| ------------------------------- | --------------- | ---------------- | ------------------------------------------------------------------------- |
| **CP3 — Hội tụ nhóm**           | Lê Nhật Linh    | Cả nhóm          | Dựng khung cây OST, gom 3 cluster, chủ trì chấm điểm shortlist            |
| **CP4 — Kiểm chứng**            | Đặng Thanh Hải  | Nguyễn Quốc Việt | Phỏng vấn 2 bạn sinh viên theo Mom Test, ghi lại tín hiệu phản bác        |
| **CP4 — Research**              | Hoàng Gia Khiêm | Lê Nhật Linh     | Bảng research 3 công cụ (Cursor, Copilot, Mintlify) kèm link thật         |
| **CP5 — Quy trình trước/sau**   | Hoàng Gia Khiêm | Nguyễn Quốc Việt | Vẽ 2 sơ đồ Mermaid (180' và 90'), lập bảng Before/After và nhánh Fallback |
| **CP5 — Problem Statement v0**  | Lê Nhật Linh    | Đặng Thanh Hải   | Soạn thảo 6 trường của v0, tính toán phân bổ baseline 180' → target 90'   |
| **CP6 — Mức can thiệp & PS v1** | Lê Nhật Linh    | Hoàng Gia Khiêm  | Chọn AI Workflow (Augment), siết chặt Boundary và 4 tiêu chí Eval         |
| **CP6 — Quyết định**            | Đặng Thanh Hải  | Nguyễn Quốc Việt | Đánh giá 4 rủi ro, chốt Go (pilot 2 repo) và ngưỡng dừng (Kill Switch)    |

## Cá nhân

### LeNhatLinh-2A202603514

**Phần việc phụ trách:**

- Nhóm trưởng điều phối tiến độ, chủ trì hội tụ CP3, viết Problem Statement v0/v1, chốt metric và boundary.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Tổng hợp 12 candidate problems, dựng khung cây OST (Mục 2 CP3).
- Soạn thảo Problem Statement v0 và v1, chuẩn hóa Success Metric (180' → 90', giảm hỏi mentor ≤ 1 lần) và ranh giới Boundary cấm AI tự viết code (Mục 5 & Mục 7).
- Phản biện phương án giảm thời gian và chốt tiêu chí eval của AI Workflow.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md`: Mục 2, Mục 5, Mục 7.
- Commits: `2bd3ba0` (CP3 nhóm), `9f8747a` (CP6 nhóm).

**Điều mình học được từ phần nhóm:**

- Hiểu sâu sắc cách rào Boundary cho AI và tại sao phải có số liệu đo lường cụ thể thay vì chỉ đặt mục tiêu chung chung.

---

### DangThanhHai-2A202603570

**Phần việc phụ trách:**

- Phụ trách kiểm chứng phỏng vấn Mom Test, phản biện các giả định và đánh giá 4 rủi ro quyết định CP6.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Tiến hành phỏng vấn sâu 2 bạn sinh viên IT theo nguyên tắc Mom Test, khai thác được tín hiệu phản bác: AI bịa hàm/file ảo làm mất thêm 45' debug (Mục 3.2 CP4).
- Đánh giá 4 khía cạnh rủi ro (Value, Usability, Feasibility, Viability) và xây dựng điều kiện pilot, ngưỡng dừng Kill Switch (Mục 8 CP6).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md`: Mục 3.1, Mục 3.2, Mục 8.
- Commits: `9f8747a` (CP6 nhóm).

**Điều mình học được từ phần nhóm:**

- Kỹ thuật hỏi hành vi trong quá khứ theo Mom Test giúp phát hiện ra rủi ro ảo giác của AI mà trước đó nhóm chưa lường tới.

---

### HoangGiaKhiem-2A202603540

**Phần việc phụ trách:**

- Phụ trách nghiên cứu thị trường (Research đối thủ) và thiết kế quy trình nghiệp vụ trước/sau.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Research chuyên sâu 3 công cụ (Cursor, Copilot, Mintlify) tìm ra khoảng trống thiếu sơ đồ luồng trực quan (Mục 3.3 CP4).
- Vẽ sơ đồ Mermaid quy trình hiện tại (180') và quy trình tương lai (90'), bổ sung nhánh Fallback (Call Hierarchy IDE + pair 10' mentor) và lập bảng so sánh Before/After (Mục 4 CP5).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md`: Mục 3.3, Mục 4.
- Commits: `9f8747a` (CP6 nhóm).

**Điều mình học được từ phần nhóm:**

- Một quy trình có AI bắt buộc phải có bước con người kiểm tra (HITL) và đường lui (Fallback) thì mới áp dụng được vào thực tế.

---

### NguyenQuocViet-2A202603556

**Phần việc phụ trách:**

- Khảo sát nhanh cộng đồng sinh viên, xây dựng AI Canvas và bộ tiêu chí đánh giá (Eval) đầu ra của AI.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Triển khai Quick-poll với 8 bạn sinh viên IT thu được tỷ lệ 87.5% gặp khó khăn ở khâu trace luồng code (Mục 3.2 CP4).
- Soạn thảo AI Canvas rút gọn, trả lời 2 câu hỏi Google PAIR (Mục 6.3 & 6.4) và định nghĩa 4 tiêu chí Eval kỹ thuật cho AI Workflow (Mục 7.3 CP6).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md`: Mục 3.2, Mục 6.3, Mục 6.4, Mục 7.3.
- Commits: `9f8747a` (CP6 nhóm).

**Điều mình học được từ phần nhóm:**

- Muốn kiểm soát chất lượng AI thì tiêu chí đánh giá phải đo bằng con số kỹ thuật (dòng code, giây phản hồi) chứ không thể đánh giá cảm tính.
