# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: NhomMTGD
- Candidate problem nhóm chọn (1 câu): Hỗ trợ sinh viên chuyển thông báo học tập không có cấu trúc từ LMS, Zalo, Discord thành nhiệm vụ có cấu trúc và deadline theo dõi được trên lịch cá nhân.
- Quyết định cuối (Go / Not Yet / No-Go): Go (Phạm vi nhỏ — Workflow kết hợp AI trích xuất + Rule validation + Sinh viên xác nhận HITL)

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Trần Duy Mạnh | 2A202603998 | Nhóm trưởng, phụ trách quy trình, Problem Statement và quản trị Git | TDM414 |
| 2 | Nguyễn Xuân Dương | 2A202603955 | Phụ trách pitch, research giải pháp và AI Canvas | xuanduong2k5 |
| 3 | Trần Thị Hồng Gấm | 2A202603967 | Phụ trách kiểm chứng phỏng vấn Mom Test, Assumption Map | Cactus_2995 |
| 4 | Đinh Lê Thịnh | 2A202603953 | Người phản biện chính, phân tích 4 rủi ro và ngưỡng dừng | thinh |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Trần Duy Mạnh | Nguyễn Xuân Dương, Đinh Lê Thịnh | Bảng Pitch 12 candidates, Cluster, cây OST, bảng chấm điểm shortlist |
| CP4 — Kiểm chứng | Trần Thị Hồng Gấm | Nguyễn Xuân Dương | Assumption map, 3 Interview Snapshots phỏng vấn sinh viên thật |
| CP4 — Research | Nguyễn Xuân Dương | Đinh Lê Thịnh | Bảng research 3 công cụ (Google Tasks, Todoist, Notion) có link kiểm chứng |
| CP5 — Quy trình trước/sau | Trần Duy Mạnh | Trần Thị Hồng Gấm | Sơ đồ quy trình Before/After, bảng so sánh chỉ số thời gian |
| CP5 — Problem Statement v0 | Đinh Lê Thịnh | Trần Duy Mạnh | Bản Problem Statement v0 hoàn chỉnh có baseline và target |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Xuân Dương | Trần Duy Mạnh | Ma trận phức tạp × mơ hồ, AI Canvas, 2 câu hỏi PAIR, Problem Statement v1, Bộ Eval 10 test cases |
| CP6 — Quyết định | Đinh Lê Thịnh | Cả nhóm | Phân tích 4 rủi ro, kết luận Go và Ngưỡng dừng đo được |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### TranDuyManh-2A202603998

**Phần việc phụ trách:**
- Điều phối chung nhóm, chủ trì phiên họp hội tụ CP3, xây dựng sơ đồ quy trình trước/sau (CP5) và quản trị kho lưu trữ GitHub (PR, conflict resolution).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Trình bày 3 Problem Cards cá nhân ở phiên pitch; chủ trì phân loại 12 candidate thành 4 cụm logic.
- Thiết kế sơ đồ quy trình hiện tại (6 bước, 30 phút) và quy trình tương lai (4 bước, 15 phút) có đánh dấu bước nghẽn Bottleneck và ranh giới Boundary.
- Đồng tác giả Problem Statement v1 và bộ 10 test case eval mẫu.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Mục 2 (bảng Pitch, Cluster, OST), Mục 4 (sơ đồ quy trình 4.1 và 4.2), Mục 7 trong `group_report.md`.
- Các commit merge PR #2 và cập nhật báo cáo nhóm trên nhánh `main`.

**Điều mình học được từ phần nhóm:**
- Hiểu sâu sắc mô hình Double Diamond: từ 12 bài toán rất khác nhau của các cá nhân, nhóm có thể tìm ra điểm giao thoa (pattern) để hội tụ về một vấn đề thực tế nhất.
- Nhận ra rằng không phải cứ dùng Agent là ngầu, mà một Workflow đơn giản có Human-in-the-loop mới là giải pháp tối ưu cho bài toán có rủi ro cao như lịch học/deadline.

---

### NguyenXuanDuong-2A202603955

**Phần việc phụ trách:**
- Tham gia phiên pitch CP3, phụ trách research giải pháp có sẵn (CP4) và điền AI Canvas rút gọn (CP6).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Đóng góp 3 candidate ban đầu; đặt câu hỏi phản biện cho bài toán trích xuất log thực nghiệm AI.
- Thực hiện research chuyên sâu 3 công cụ (Google Tasks/Calendar, Todoist, Notion), phân tích điểm mạnh và khoảng trống chưa xử lý được văn bản tiếng Việt tự do.
- Xây dựng bảng AI Canvas rút gọn (Prediction, Judgment, Action, Outcome, Input, Feedback) và trả lời 2 câu hỏi Google PAIR.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Mục 3.3 (Bảng research giải pháp), Mục 6.3 (AI Canvas), Mục 6.4 (Google PAIR) trong `group_report.md`.

**Điều mình học được từ phần nhóm:**
- Học được cách làm research có mục đích: không chỉ liệt kê tính năng của đối thủ mà phải chỉ ra được khoảng trống họ bỏ sót để tìm ra ngách cho bài toán của nhóm.

---

### TranThiHongGam-2A202603967

**Phần việc phụ trách:**
- Tham gia phiên pitch CP3, phụ trách xây dựng Assumption Map và phỏng vấn người dùng thực tế theo The Mom Test (CP4).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Trình bày 3 candidate về quản lý thông báo và deadline; đặt câu hỏi phản biện về việc phân biệt deadline bắt buộc vs thảo luận.
- Thiết lập bảng Assumption Map 6 giả định; trực tiếp phỏng vấn 5 sinh viên thật theo The Mom Test để thu thập bằng chứng về hành vi bỏ sót deadline và workaround hiện tại.
- Tổng hợp bảng tín hiệu xác nhận vs tín hiệu phản bác, giúp nhóm đổi hướng không xây app lịch mới mà làm tool trích xuất.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Mục 3.1 (Assumption Map), Mục 3.2 (3 Interview Snapshots và bảng tổng hợp kiểm chứng) trong `group_report.md`.

**Điều mình học được từ phần nhóm:**
- Thấm nhuần tư tưởng The Mom Test: phỏng vấn người thật không bao giờ được hỏi "bạn có muốn dùng AI không?", mà phải hỏi về những lần họ quên deadline trong quá khứ để tìm bằng chứng hành vi thật.

---

### DinhLeThinh-2A202603953

**Phần việc phụ trách:**
- Người phản biện chính của nhóm, phụ trách viết Problem Statement v0 (CP5), phân tích 4 rủi ro và xác lập Ngưỡng dừng (CP6).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Đóng góp 3 candidate; liên tục đặt câu hỏi phản biện sắc sảo ("Tại sao không dùng Ctrl+F?", "Nếu thành viên giấu issue thì sao?").
- Soạn thảo Problem Statement v0 gồm 6 trường chuẩn; tham gia phản biện lỗ hổng với AI.
- Đánh giá chi tiết 4 rủi ro (Value, Usability, Feasibility, Viability) và thiết lập Ngưỡng dừng đo được (Stop condition) cho quyết định Go.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Mục 2.1 (câu hỏi phản biện), Mục 5 (Problem Statement v0), Mục 8 (Bốn rủi ro, Kết luận Go và Ngưỡng dừng) trong `group_report.md`.

**Điều mình học được từ phần nhóm:**
- Hiểu được giá trị của việc phản biện: một ý tưởng dù hay đến đâu nếu không vượt qua được bài kiểm tra về 4 rủi ro và không có ngưỡng dừng thì rất dễ biến thành một dự án "thây ma" tốn kém tài nguyên.
