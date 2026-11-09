
# Báo cáo cá nhân — 2A202603998_TranDuyManh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Duy Mạnh
- MSSV: 2A202603998
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:NhomMTGD
- Link repo nhóm: https://github.com/TDM414/L3B--DAY02-NhomMTGD-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi hoàn thành một đợt benchmark nhiều mô hình (ML/DL/LLM), tôi muốn tổng hợp các chỉ số F1, latency p95 và chi phí vào một bảng đối chiếu chuẩn, để không phải sao chép thủ công từ từng notebook/log sang báo cáo. | Học viên làm lab, người nghiên cứu AI | Tự bấm giờ sau 3 buổi lab gần nhất: mất trung bình 45–60 phút/lần, phải rà soát thủ công 4–5 notebook. |
| 2 | Lặp lại | Khi nhóm 3–4 người cùng gán nhãn dữ liệu text cho bài tập lớn, tôi muốn phát hiện ngay các mẫu có nhãn mâu thuẫn giữa các thành viên, để thống nhất quy chuẩn gán nhãn trước khi đưa vào huấn luyện mô hình. | Cả nhóm làm đồ án (3–4 người) | Mỗi đợt gán nhãn ~500 mẫu mất 90 phút họp đối chiếu chéo; có 15–20% số mẫu bị lệch nhãn giữa 2 người. |
| 3 | Tốn thời gian | Khi bắt đầu một bài toán/đề tài mới cần chọn mô hình cơ sở (baseline), tôi muốn nắm nhanh bảng đối chiếu thực nghiệm và điều kiện giả định của 3–5 bài báo khoa học liên quan, để quyết định kiến trúc mô hình phù hợp trước hạn nộp đề cương. | Học viên, kỹ sư AI | Mất 3–4 tiếng/tuần đọc lướt 5–7 paper; từng 2 lần chọn nhầm baseline do không đọc kỹ điều kiện phần cứng. |
| 4 | Tốn thời gian | Khi nhận tập dữ liệu thô từ nhiều nguồn khác nhau (lỗi encoding, format ngày tháng không đồng nhất, missing values ẩn), tôi muốn kiểm tra và chuẩn hóa theo một schema duy nhất, để pipeline huấn luyện không bị dừng đột ngột giữa chừng. | Người tiền xử lý dữ liệu, học viên | Mất 60–90 phút cho mỗi tập dữ liệu mới; trung bình gặp 2 lần lỗi runtime/tuần do ký tự rác hoặc giá trị null ẩn. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi thiết lập môi trường chạy mã nguồn mới trên máy tính hoặc Colab, tôi muốn xác định chính xác các phiên bản tương thích giữa CUDA driver, PyTorch và các thư viện phụ thuộc, để môi trường chạy được ngay mà không phải cài/gỡ thử từng gói. | Lập trình viên AI, học viên | Mất trung bình 45–75 phút mỗi lần dựng môi trường mới; trong tháng trước gặp 3 lần lỗi CUDA version mismatch. |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị nộp bài lab trước deadline, tôi muốn đối chiếu toàn bộ các tệp trong repo với danh mục yêu cầu trong rubric, để đảm bảo không bị trừ điểm vì sai định dạng tên file hoặc thiếu mục bắt buộc. | Học viên nộp bài | Mất 30–40 phút tự kiểm tra chéo giữa README, RUBRIC và SUBMISSION; từng bị trừ 5 điểm ở bài trước do sai tên tệp. |
| 7 | Pain từ người khác | Khi đến hạn nộp báo cáo nhóm vào cuối tuần, tôi muốn có bản tổng hợp tiến độ và đầu việc từng người đã hoàn thành, để điền bảng phân công mà không phải nhắn tin hỏi dồn từng thành viên trong nhóm. | Nhóm trưởng, thành viên nhóm | Mất 60 phút mỗi tuần nhắn tin giục 3 thành viên; 2/3 lần nộp bài sát nút vì chờ thành viên xác nhận phần đóng góp. |
| 8 | Pain từ người khác | Khi các thành viên trong nhóm đưa thay đổi lên repo chung, tôi muốn kiểm tra và cảnh báo trước các commit lệch chuẩn hoặc sai nhánh, để không làm hỏng lịch sử commit của nhánh chính trước khi nộp. | Nhóm trưởng, người review repo | Mất 30–45 phút gỡ conflict git mỗi tuần; tuần trước phải revert 2 commit do thành viên push nhầm lên nhánh chính. |
| 9 | Lặp lại *(ý từ AI)* | Khi hoàn thành một tính năng hoặc một checkpoint trong bài làm, tôi muốn ghi nhận nhanh nội dung thay đổi chính xác, để lịch sử commit rõ ràng và người chấm dễ theo dõi tiến độ. | Người làm bài, người chấm bài | Mất 10–15 phút/lần viết tóm tắt commit; trung bình 4–5 commit/ngày, hay bị thói quen ghi "fix bug" chung chung. |
| 10 | Cần đọc, tổng hợp nhiều thông tin *(ý từ AI)* | Khi gặp một lỗi runtime trong lúc chạy thực nghiệm, tôi muốn tra cứu xem trong diễn đàn/kênh chat lớp đã có ai từng gặp và cách xử lý là gì, để sửa được lỗi mà không phải đăng câu hỏi trùng lặp. | Học viên, trợ giảng lớp học | Mất 20–30 phút lội tìm tin nhắn trong Discord; trợ giảng phản ánh phải trả lời lại cùng một lỗi 5–6 lần/tuần. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại (#9, #10):** Tôi giữ lại ý tưởng về tóm tắt commit log và tra cứu lỗi lặp lại trên Discord, nhưng viết lại hoàn toàn theo bối cảnh thực tế bài lab kỹ thuật của bản thân, gắn kèm số liệu đo đạc thời gian thật.
- **Ý loại bỏ:** Tôi đã từ chối các gợi ý như *"Chatbot tự động làm bài tập thay học viên"* hay *"AI Agent quản lý toàn diện đề tài tốt nghiệp"* vì đây là các giải pháp viển vông, phạm vi vô định và vi phạm nguyên tắc "problem first" (solution trá hình).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp và đối chiếu số liệu benchmark mô hình AI (#1) | Quy trình lặp lại rõ ràng sau mỗi đợt chạy thực nghiệm; có baseline thời gian đo thật; dễ phân định ranh giới giữa Rule và AI. | AI viết phần phân tích nhận định kỹ thuật (narrative) có đủ sâu sắc và chính xác không hay chỉ mô tả lại số liệu. |
| 2 | Phát hiện dữ liệu gán nhãn mâu thuẫn trong nhóm (#2) | Nỗi đau thực tế trong mọi đồ án nhóm có khâu chuẩn bị dữ liệu; ảnh hưởng trực tiếp đến chất lượng mô hình (F1). | Mức độ phức tạp khi người dùng muốn AI giải thích lý do bất đồng theo từng quy chuẩn gán nhãn cụ thể. |
| 3 | Kiểm tra tuân thủ checklist/rubric trước khi nộp bài (#6) | Nỗi đau sát sườn trước mỗi kỳ hạn nộp bài; impact trực tiếp đến điểm số; dễ định lượng tiêu chí đạt/không đạt. | Đa số các bước có thể giải quyết triệt để bằng Rule/Script linter, phần việc cho AI can thiệp tương đối hẹp. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi hoàn thành một đợt benchmark nhiều mô hình (ML/DL/LLM), tôi muốn tổng hợp các chỉ số F1, latency p95 và chi phí vào một bảng đối chiếu chuẩn, để không phải sao chép thủ công từ từng notebook/log sang báo cáo. |
| Actor | Học viên nghiên cứu AI, AI Engineer phụ trách benchmark thực nghiệm mô hình |
| Thời điểm / bối cảnh | Ngay sau khi chạy xong loạt script thực nghiệm trên nhiều notebook/server, cần chuẩn bị bảng số liệu báo cáo |
| Quy trình hiện tại (3–7 bước) | 1. Mở lần lượt từng notebook/terminal log của các mô hình (10')<br>2. Tìm cell/dòng lệnh in kết quả F1, latency, chi phí (15')<br>3. Sao chép số liệu sang Excel/báo cáo nháp (15')<br>4. Tính toán độ lệch delta giữa các mô hình và vẽ bảng so sánh (15')<br>5. Viết nhận định narrative so sánh ưu/nhược điểm các mô hình (15') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 và 3 (tìm log và copy số liệu thủ công): mất 30 phút, dễ nhìn nhầm số liệu giữa các lần chạy (runs/seeds khác nhau) |
| Impact (nếu không giải thì sao) | Mất 70 phút mỗi đợt chạy; nếu copy nhầm số liệu sẽ dẫn đến nhận xét sai về mô hình Pareto tối ưu, phải chạy và viết lại từ đầu |
| Success metric (baseline → target) | Tổng thời gian: từ 70 phút xuống dưới 15 phút/lần tổng hợp; Tỉ lệ sai sót copy số liệu: từ ~15% xuống 0% |
| Phương án không dùng AI | Viết script Python export kết quả ra file JSON chuẩn (`lab_report.json`) + dùng template Markdown parse tự động |
| Giả thuyết về AI (nếu có) | AI đọc file JSON số liệu đã gom để sinh bản nháp nhận định (narrative draft) chỉ ra mô hình tối ưu Pareto; con người review lại |
| Cảm nhận nhanh | Workflow (Script gom số liệu định sẵn + AI hỗ trợ nháp narrative có con người kiểm duyệt) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 70 phút

[1 Mở các notebook: 10']
       │
       ▼
[2 Tìm log print metrics: 15'] ◄── BOTTLENECK (hoa mắt, dễ nhầm run/seed)
       │
       ▼
[3 Copy số liệu sang Excel/Docs: 15'] ◄── BOTTLENECK (dễ gõ nhầm số)
       │
       ▼
[4 Tính delta & lập bảng so sánh: 15']
       │
       ▼
[5 Viết nhận định narrative: 15']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhóm 3–4 người cùng gán nhãn dữ liệu text cho bài tập lớn, tôi muốn phát hiện ngay các mẫu có nhãn mâu thuẫn giữa các thành viên, để thống nhất quy chuẩn gán nhãn trước khi đưa vào huấn luyện mô hình. |
| Actor | Thành viên nhóm phụ trách dữ liệu / Data annotator trong nhóm học tập |
| Thời điểm / bối cảnh | Sau khi từng thành viên hoàn thành đợt gán nhãn độc lập (~500 mẫu), chuẩn bị hợp nhất tập dữ liệu |
| Quy trình hiện tại (3–7 bước) | 1. Thu thập file CSV gán nhãn từ từng thành viên (10')<br>2. Ghép dữ liệu vào Google Sheets chung (15')<br>3. Dò tìm thủ công các dòng bị lệch nhãn giữa các thành viên (30')<br>4. Họp nhóm thảo luận từng câu mâu thuẫn để chốt nhãn cuối (45')<br>5. Xuất file dataset sạch đã thống nhất (10') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 và 4 (lọc thủ công và họp tranh luận từng dòng): mất 75 phút, tốn thời gian cả nhóm vì không phân loại trước mức độ mâu thuẫn |
| Impact (nếu không giải thì sao) | Mất gần 2 tiếng mỗi đợt gán nhãn; nếu bỏ qua khâu này dữ liệu sẽ dơ (noisy labels), làm suy giảm 5–10% độ chính xác của mô hình |
| Success metric (baseline → target) | Tổng thời gian xử lý: từ 110 phút xuống dưới 30 phút/đợt; Phát hiện 100% các mẫu có mâu thuẫn nhãn |
| Phương án không dùng AI | Dùng script Python/công thức Excel tính chỉ số Fleiss' Kappa và tự động lọc ra các dòng có nhãn bất đồng (`label_A != label_B`) |
| Giả thuyết về AI (nếu có) | AI đối chiếu hướng dẫn gán nhãn (guidelines) để đề xuất nhãn phù hợp kèm giải thích ngắn cho các ca tranh cãi, giúp nhóm biểu quyết nhanh |
| Cảm nhận nhanh | Rule + Workflow (Rule lọc bất đồng + Workflow gợi ý giải quyết mẫu khó) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 110 phút

[1 Thu thập CSV từ thành viên: 10']
       │
       ▼
[2 Ghép file vào Sheets: 15']
       │
       ▼
[3 Dò tìm thủ công dòng lệch nhãn: 30'] ◄── BOTTLENECK
       │
       ▼
[4 Họp nhóm tranh luận từng mẫu: 45']  ◄── BOTTLENECK (mất thời gian cả nhóm)
       │
       ▼
[5 Xuất dataset sạch cuối: 10']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nộp bài lab trước deadline, tôi muốn đối chiếu toàn bộ các tệp trong repo với danh mục yêu cầu trong rubric, để đảm bảo không bị trừ điểm vì sai định dạng tên file hoặc thiếu mục bắt buộc. |
| Actor | Học viên làm bài lab kỹ thuật nộp bài trên LMS/GitHub |
| Thời điểm / bối cảnh | Khoảng 30–60 phút trước hạn chót nộp bài (thường là 23h59) |
| Quy trình hiện tại (3–7 bước) | 1. Mở file RUBRIC.md và SUBMISSION.md đọc từng tiêu chí (10')<br>2. Mở cây thư mục repo kiểm tra từng tên file, định dạng nhánh git (10')<br>3. Mở file báo cáo đọc rà soát từng mục xem còn sót ô trống nào không (15')<br>4. Kiểm tra quyền truy cập repo và link nộp bài (5')<br>5. Nộp link lên hệ thống LMS (5') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (rà soát từng trường mục trong báo cáo dài): mất 15 phút, khi sát giờ nộp rất dễ hoa mắt và bỏ quên các ô checklist hoặc template chưa xóa |
| Impact (nếu không giải thì sao) | Nguy cơ bị trừ 5–10 điểm cấu trúc (lỗi sai định dạng file, giữ nguyên template, thiếu bảng chứng minh) dù nội dung cốt lõi làm tốt |
| Success metric (baseline → target) | Thời gian kiểm tra: từ 45 phút xuống dưới 10 phút; Độ bao phủ lỗi cấu trúc: phát hiện 100% lỗi sai định dạng tệp trước khi nộp |
| Phương án không dùng AI | Viết kịch bản kiểm tra tự động (Pre-submission Linter script bằng Python/Bash) regex kiểm tra tên tệp và grep các placeholder chưa điền |
| Giả thuyết về AI (nếu có) | AI rà soát nhanh phần văn bản mở (Reflection/Nhận định) để cảnh báo đoạn nào quá ngắn (dưới 200 từ) hoặc thiếu chiều sâu phản biện |
| Cảm nhận nhanh | Rule (Chủ yếu là Rule-based linter, chỉ cần chút Workflow rất nhỏ cho phần text) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 45 phút

[1 Đọc Rubric & Checklist: 10']
       │
       ▼
[2 Kiểm tra tên file & thư mục: 10']
       │
       ▼
[3 Đọc rà soát thủ công báo cáo: 15'] ◄── BOTTLENECK (dễ sót ô trống sát deadline)
       │
       ▼
[4 Kiểm tra link & quyền repo: 5']
       │
       ▼
[5 Nộp link lên LMS: 5']
```

### Card muốn pitch nhất

- Card số: **Card #1** (Tổng hợp và đối chiếu số liệu benchmark mô hình AI)
- Vì sao: Đây là vấn đề lặp đi lặp lại ở mọi bài lab AI/Data Science (vừa trải qua ở Lab 1 và còn lặp lại ở các lab tiếp theo); quy trình và dữ liệu số liệu rất rõ ràng, có baseline thời gian đo thật (70 phút), phân tách tường minh giữa phần việc của Rule (parse file JSON số liệu) và phần việc của AI (hỗ trợ nháp narrative phân tích tương quan), hoàn toàn nằm trong tầm tay kiểm soát của nhóm.
- Câu hỏi muốn nhóm phản biện: *"Nếu dùng script Python định dạng sẵn log ra file JSON là đã giải quyết được phần lớn thời gian gom số liệu rồi, thì phần AI viết nhận định so sánh (narrative) có thực sự cần thiết không, hay chỉ cần một template Markdown có sẵn là đủ?"*

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI cho rằng "bước viết nhận định narrative có thể tự động hóa 100% bằng AI mà không cần con người can thiệp" | Không đồng ý | Giữ ranh giới nghiêm ngặt: AI chỉ đề xuất bản nháp nhận định ban đầu; kỹ sư/học viên bắt buộc phải kiểm duyệt chuyên môn (Human-in-the-loop) trước khi đưa vào báo cáo chính thức. |
| AI chỉ ra thời lượng 70 phút có thể bị tính lẫn thời gian chạy mô hình | Đồng ý | Đã làm rõ lại phạm vi: 70 phút là thời gian thuần túy dành cho việc đọc log, sao chép số liệu và viết báo cáo so sánh, hoàn toàn không tính thời gian chờ máy train mô hình. |
| Giả định "các notebook của các thành viên đều print log giống nhau" là không thực tế | Đồng ý | Đã bổ sung phương án kỹ thuật: chuẩn hóa cấu trúc xuất file JSON chung (`lab_report.json`) từ script thay vì trông chờ vào việc đọc các dòng print tự do trên console. |

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
