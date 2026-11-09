# Báo cáo cá nhân — 2A202603998_TranDuyManh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Duy Mạnh
- MSSV: 2A202603998
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomMTGD
- Link repo nhóm: https://github.com/TDM414/L3B--DAY02-NhomMTGD-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi đợt huấn luyện mô hình dài 5–7 tiếng kết thúc, tôi muốn tổng hợp nhanh bảng đối chiếu các chỉ số (Loss, F1, Latency) và các ca phân loại sai so với lần chạy trước, để quyết định hướng điều chỉnh siêu tham số tiếp theo mà không phải cuộn tìm thủ công trong log terminal. | Học viên làm lab, người trực tiếp train model AI | Mất 30–45 phút sau mỗi lần train; trung bình chạy 2–3 đợt/tuần; từng chỉnh nhầm thông số do nhìn nhầm log của lần chạy cũ. |
| 2 | Lặp lại | Khi hoàn thành bài thực nghiệm trên lớp với nhiều mô hình (ML/DL/LLM), tôi muốn tổng hợp các chỉ số F1, latency p95 và chi phí vào một bảng đối chiếu chuẩn, để không phải sao chép thủ công từ từng notebook sang báo cáo nộp bài. | Học viên làm bài lab | Mất 45–60 phút mỗi buổi lab (đã làm ở Lab 1 với 5 mô hình); phải mở lại 4–5 notebook để copy từng ô số liệu. |
| 3 | Tốn thời gian | Khi mô hình huấn luyện xong nhưng chỉ số F1 không đạt kỳ vọng, tôi muốn khoanh vùng nhanh các nhãn dữ liệu bị dự đoán sai nhiều nhất và các tham số đang gây overfitting, để sửa code và tinh chỉnh tham số trong vòng 30–60 phút thay vì phải thử sai mò mẫm. | Người tinh chỉnh mô hình (Fine-tuner) | Mất từ 30–60 phút mỗi lần fix và kiểm tra lại; trung bình lặp lại 3–4 lần/tuần trước khi có mô hình ưng ý. |
| 4 | Tốn thời gian | Khi thiết lập môi trường chạy mã nguồn mới trên máy tính cá nhân hoặc Google Colab, tôi muốn xác định chính xác các phiên bản tương thích giữa CUDA driver, PyTorch và các thư viện phụ thuộc, để code chạy được ngay mà không phải cài/gỡ thử từng gói nhiều lần. | Lập trình viên AI, học viên | Mất 45–75 phút mỗi lần dựng môi trường mới; trong tháng trước gặp 3 lần lỗi `CUDA mismatch` khiến script dừng ngay từ bước load model. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi theo dõi tiến trình huấn luyện mô hình kéo dài 5–7 tiếng, tôi muốn có một bảng tổng quan duy nhất hiển thị trạng thái epoch, mức tiêu thụ GPU memory và các cảnh báo lỗi, để không phải chuyển đổi liên tục giữa terminal, TensorBoard và file mã nguồn. | Người chạy thực nghiệm | Phải mở 4–5 cửa sổ song song; mất 15–20 phút mỗi lần kiểm tra tiến độ; từng bị dừng tiến trình 1 lần do không phát hiện kịp lỗi GPU tràn bộ nhớ (OOM). |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị nộp bài lab trước deadline 23h59, tôi muốn đối chiếu toàn bộ các tệp trong repo với danh mục yêu cầu trong rubric, để đảm bảo không bị trừ điểm vì sai định dạng tên file hoặc thiếu mục bắt buộc. | Học viên nộp bài | Mất 30–45 phút tự kiểm tra chéo giữa README, RUBRIC và SUBMISSION; từng bị trừ 5 điểm ở bài trước do sai quy cách đặt tên tệp. |
| 7 | Pain từ người khác | Khi đến hạn nộp báo cáo nhóm vào cuối tuần, tôi muốn có bản tổng hợp tiến độ và đầu việc từng người đã hoàn thành, để điền bảng phân công mà không phải nhắn tin hỏi dồn từng thành viên trong nhóm. | Nhóm trưởng, người tổng hợp bài | Mất khoảng 1 tiếng mỗi tuần nhắn tin giục các thành viên trong nhóm; 2/3 lần nộp bài sát nút vì chờ thành viên xác nhận phần đóng góp. |
| 8 | Pain từ người khác | Khi các thành viên trong nhóm đưa thay đổi lên repo chung, tôi muốn kiểm tra và cảnh báo trước các commit lệch chuẩn hoặc sai nhánh, để không làm hỏng lịch sử commit của nhánh chính trước khi nộp. | Nhóm trưởng, người review repo | Mất 30–45 phút gỡ conflict git mỗi tuần; vừa phải xử lý xung đột do thành viên push nhầm lên nhánh chính. |
| 9 | Lặp lại *(ý từ AI)* | Khi thử nghiệm thay đổi kiến trúc hoặc hàm loss của mô hình, tôi muốn ghi nhận tự động cấu hình tham số cùng với commit git tương ứng, để sau này có thể tái lập lại đúng phiên bản mô hình tốt nhất mà không phải dựa vào trí nhớ. | Học viên, kỹ sư AI | Mất 15 phút mỗi lần ghi chép tay cấu hình tham số; từng mất nửa ngày tìm lại phiên bản code cũ vì quên không ghi lại commit hash ứng với kết quả tốt nhất. |
| 10 | Cần đọc, tổng hợp nhiều thông tin *(ý từ AI)* | Khi gặp lỗi runtime lạ trong lúc tiền xử lý dữ liệu hoặc chạy train, tôi muốn tra cứu xem trong diễn đàn/kênh chat lớp đã có ai từng gặp lỗi tương tự và cách sửa là gì, để khắc phục nhanh mà không phải chờ đợi trợ giảng trả lời. | Học viên, trợ giảng lớp học | Mất 20–30 phút lội tìm tin nhắn trong Discord; trợ giảng phản ánh phải trả lời lại cùng một lỗi 5–6 lần/tuần. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại (#9, #10):** Tôi giữ lại ý tưởng về tự động lưu vết thực nghiệm (Experiment tracking log) và tra cứu lỗi lặp lại trên diễn đàn Discord của lớp, nhưng viết lại hoàn toàn theo bối cảnh thực tế bài lab kỹ thuật của bản thân, gắn kèm số liệu đo đạc thời gian thật.
- **Ý loại bỏ:** Tôi đã từ chối các gợi ý như *"Chatbot tự động viết code train model"* hay *"AI Agent tự động fix toàn bộ lỗi pipeline"* vì đây là các giải pháp viển vông, phạm vi vô định và vi phạm nguyên tắc "problem first" (solution trá hình).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Trích xuất và đối chiếu kết quả thực nghiệm sau khi train model 5–7 tiếng để điều chỉnh siêu tham số (#1) | Quy trình lặp lại thường xuyên; tốn thời gian lớn sau mỗi lần chạy; ảnh hưởng trực tiếp đến kết quả của vòng lặp train tiếp theo; có ranh giới rõ ràng giữa Rule và AI. | Khả năng AI tổng hợp các trường hợp dự đoán sai (error patterns) có đủ sâu sắc và chính xác để gợi ý hướng chỉnh tham số hay không. |
| 2 | Tổng hợp số liệu benchmark nhiều mô hình sau buổi lab vào báo cáo kỹ thuật (#2) | Nỗi đau lặp đi lặp lại sau mỗi bài lab AI (đã trải qua ở Lab 1); có baseline đo thật 45–60 phút; tiêu chí hoàn thành rất rõ ràng. | AI viết phần phân tích nhận định so sánh (narrative) có đủ tính logic chuyên môn hay chỉ đọc lại số liệu trong bảng. |
| 3 | Rà soát checklist và rubric bài nộp trước deadline để tránh mất điểm cấu trúc (#6) | Nỗi đau thực tế trước mỗi kỳ hạn nộp bài; ảnh hưởng trực tiếp đến điểm số; dễ định lượng tiêu chí đạt/không đạt. | Đa số các bước kiểm tra có thể giải quyết triệt để bằng Rule-based linter, phần việc cho AI can thiệp tương đối hẹp. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi một đợt huấn luyện mô hình dài 5–7 tiếng kết thúc, tôi muốn tổng hợp nhanh bảng đối chiếu các chỉ số (Loss, F1, Latency) và các ca phân loại sai so với lần chạy trước, để quyết định hướng điều chỉnh siêu tham số tiếp theo trong vòng 30–60 phút mà không phải cuộn tìm thủ công trong log terminal. |
| Actor | Học viên nghiên cứu AI, người trực tiếp huấn luyện mô hình (Model Fine-tuner) |
| Thời điểm / bối cảnh | Sau khi script huấn luyện mô hình (5–7 tiếng) hoàn thành trên GPU/Colab, chuẩn bị cho vòng lặp điều chỉnh tiếp theo |
| Quy trình hiện tại (3–7 bước) | 1. Mở file log terminal dài hàng nghìn dòng, tìm dòng in kết quả đánh giá cuối cùng (15')<br>2. Mở log của các lần chạy trước (runs cũ) để đối chiếu sự thay đổi của validation loss và F1 (15')<br>3. Trích xuất thủ công danh sách các mẫu dữ liệu dự đoán sai (error analysis) từ dataframe/file nháp (15')<br>4. Suy luận nguyên nhân lỗi (do dữ liệu, learning rate hay overfit) và sửa code/tham số cho lần train tiếp theo (30') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 1 và 2 (tìm log và đối chiếu thủ công giữa các run): mất 30 phút, rất dễ nhầm dòng giữa các run khác nhau dẫn đến suy đoán sai hướng |
| Impact (nếu không giải thì sao) | Mất 75 phút mỗi vòng lặp; nếu chỉnh nhầm tham số do nhìn nhầm log cũ, sẽ lãng phí tiếp 5–7 tiếng huấn luyện của vòng lặp tiếp theo |
| Success metric (baseline → target) | Thời gian tổng hợp và đối chiếu log: từ 30 phút xuống dưới 5 phút/lần; Tỉ lệ nhầm lẫn thông số giữa các lần chạy: từ ~20% xuống 0% |
| Phương án không dùng AI | Tích hợp thư viện theo dõi thực nghiệm (như TensorBoard/Wandb hoặc script tự xuất JSON `metrics_history.json`) để vẽ biểu đồ so sánh tự động |
| Giả thuyết về AI (nếu có) | Sau khi script trích xuất bảng so sánh số liệu và danh sách mẫu lỗi, AI phân tích nhanh các mẫu lỗi phổ biến (error patterns) và gợi ý giả thuyết nguyên nhân; kỹ sư xem xét và quyết định |
| Cảm nhận nhanh | Workflow (Script gom log cố định + AI hỗ trợ phân tích mẫu lỗi có con người kiểm duyệt) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 75 phút

[1 Chờ train 5-7h: thụ động]
       │
       ▼
[2 Dò tìm log terminal: 15'] ◄── BOTTLENECK (hoa mắt, hàng nghìn dòng log)
       │
       ▼
[3 Đối chiếu thủ công với run cũ: 15'] ◄── BOTTLENECK (dễ nhầm seed/run)
       │
       ▼
[4 Trích xuất mẫu phân loại sai: 15']
       │
       ▼
[5 Suy luận nguyên nhân & sửa code/tham số: 30']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi hoàn thành bài thực nghiệm trên lớp với nhiều mô hình (ML/DL/LLM), tôi muốn tổng hợp các chỉ số F1, latency p95 và chi phí vào một bảng đối chiếu chuẩn, để không phải sao chép thủ công từ từng notebook sang báo cáo nộp bài. |
| Actor | Học viên làm bài lab AI, kỹ sư tổng hợp báo cáo kỹ thuật |
| Thời điểm / bối cảnh | Sau mỗi buổi thực nghiệm trên lớp hoặc trước hạn nộp bài lab kỹ thuật |
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

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nộp bài lab trước deadline 23h59, tôi muốn đối chiếu toàn bộ các tệp trong repo với danh mục yêu cầu trong rubric, để đảm bảo không bị trừ điểm vì sai định dạng tên file hoặc thiếu mục bắt buộc. |
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

- Card số: **Card #1** (Trích xuất và đối chiếu kết quả thực nghiệm sau khi train model 5–7 tiếng để điều chỉnh siêu tham số)
- Vì sao: Đây là công việc lặp lại tốn thời gian và đau đớn nhất trong chu kỳ phát triển mô hình AI của tôi; mỗi lần chạy máy mất 5–7 tiếng, nếu bước đối chiếu log và tìm nguyên nhân lỗi bị nhầm sẽ làm lãng phí cả một đêm train tiếp theo; bài toán có ranh giới rõ ràng giữa Rule (trích xuất log) và AI (hỗ trợ phân tích mẫu lỗi).
- Câu hỏi muốn nhóm phản biện: *"Nếu dùng TensorBoard/Wandb đã vẽ được đồ thị Loss và F1 qua các epoch rồi, thì việc dùng thêm AI để phân tích các ca phân loại sai (error analysis) có thực sự đem lại giá trị vượt trội so với việc tự nhìn confusion matrix không?"*

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI cho rằng "có thể để AI tự động chỉnh luôn siêu tham số (AutoML) và tự chạy đợt train tiếp theo không cần người" | Không đồng ý | Giữ ranh giới (boundary) nghiêm ngặt: AI chỉ tóm tắt các ca lỗi và gợi ý giả thuyết; kỹ sư bắt buộc phải tự tay quyết định thay đổi code/siêu tham số nào để kiểm soát chi phí tính toán GPU. |
| AI chỉ ra rằng thời gian train 5–7 tiếng không phải là bottleneck mà bước con người chờ đợi mới là bottleneck | Đồng ý một phần | Làm rõ lại: Thời gian train 5–7 tiếng là thời gian máy chạy ngầm; bottleneck con người thực sự là 30 phút cuộn log thủ công và 30–60 phút mò mẫm tìm lý do mô hình không hội tụ. |
| Giả định log của các framework khác nhau (PyTorch, TensorFlow, HuggingFace) đều giống nhau là không thực tế | Đồng ý | Bổ sung phương án: Chuẩn hóa việc ghi log qua một callback thống nhất lưu ra file JSON/CSV thay vì đọc chuỗi text in tự do trên stdout. |

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
