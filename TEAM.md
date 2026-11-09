# Nhóm

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: Siuu
- Candidate problem nhóm chọn (1 câu): Sinh viên/người mới mất nhiều thời gian để hiểu cấu trúc và trace luồng xử lý trong codebase dự án.
- Quyết định cuối (Go / Not Yet / No-Go): Go — pilot trên 2 repo, theo ngưỡng dừng ở báo cáo nhóm.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Lê Nhật Linh | 2A202603514 | Nhóm trưởng, điều phối | NhatLinh056 |
| 2 | Đặng Thanh Hải | 2A202603570 | Phản biện, kiểm chứng/phỏng vấn | Chưa khai báo |
| 3 | Hoàng Gia Khiêm | 2A202603540 | Research, quy trình | Chưa khai báo |
| 4 | Nguyễn Quốc Việt | 2A202603556 | Khảo sát, đánh giá AI | Chưa khai báo |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Lê Nhật Linh | Cả nhóm | Gom 12 candidate thành 3 cluster; khung cây OST từ outcome 180 → 90 phút tới 3 opportunity |
| CP4 — Kiểm chứng | Đặng Thanh Hải, Nguyễn Quốc Việt | Cả nhóm | 2 phỏng vấn Mom Test; quick-poll 8 sinh viên, 7/8 gặp khó khi trace luồng code |
| CP4 — Research | Hoàng Gia Khiêm | Cả nhóm | Research Cursor, Copilot, Mintlify; cần bổ sung liên kết nguồn vào báo cáo nhóm |
| CP5 — Quy trình trước/sau | Hoàng Gia Khiêm | Lê Nhật Linh | Hai sơ đồ Mermaid 180 phút và 90 phút; fallback bằng Call Hierarchy IDE và 10 phút mentor pair |
| CP5 — Problem Statement v0 | Lê Nhật Linh | Cả nhóm | Statement về onboarding codebase; metric 180 → 90 phút, hỏi mentor ≤ 1 lần; AI không tự viết code |
| CP6 — Mức can thiệp + Problem Statement v1 | Lê Nhật Linh, Nguyễn Quốc Việt | Cả nhóm | Problem Statement v1; AI Canvas, Google PAIR và 4 tiêu chí Eval (Grounding, Accuracy, Latency, Completeness) |
| CP6 — Quyết định | Lê Nhật Linh; Đặng Thanh Hải phản biện | Cả nhóm | Go pilot trên 2 repo; ngưỡng dừng: hallucination >15% hoặc tiết kiệm thời gian <40 phút |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NguyenQuocViet-2A202603556

**Phần việc phụ trách:**

- Khảo sát nhanh và đánh giá mức can thiệp AI.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Chạy quick-poll với 8 sinh viên; 7/8 (87,5%) cho biết gặp khó khi trace luồng code giữa các file.
- Soạn AI Canvas, trả lời hai câu hỏi Google PAIR và xây 4 tiêu chí Eval: Grounding, Accuracy, Latency, Completeness.
- Chuyển tiêu chí chung chung thành tiêu chí kỹ thuật có thể kiểm tra, gồm citation `filepath:linenumber` và độ trễ ≤15 giây.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`, mục 3.2, 6.3, 6.4 và 7; báo cáo cá nhân CP1–CP2 tại `report/individual/2A202603556_NguyenQuocViet.md`.

**Điều mình học được từ phần nhóm:**

- [Việt tự điền bằng trải nghiệm thật của mình.]
