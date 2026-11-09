# Báo cáo cá nhân — 2A202603998_TranDuyManh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Duy Mạnh
- MSSV: 2A202603998
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomMTGD
- Link repo nhóm: https://github.com/TDM414/K5-L3B--DAY02-NhomMTGD-DiscoveryProblemFraming

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
| Pitch Problem Card | Trình bày 3 card của mình, đặc biệt nhấn mạnh Card #1 về trích xuất log thực nghiệm AI và Card #3 về rà soát rubric trước deadline. | Giúp nhóm có thêm góc nhìn về các bài toán tự động hóa quy trình kỹ thuật. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt:<br>• Hỏi Dương: *"Các công cụ như Google Calendar hay Notion đã có sẵn, tại sao sinh viên vẫn bị quên deadline?"*<br>• Hỏi Gấm: *"Bài toán đọc hiểu paper AI quá rộng, làm sao đánh giá được AI tóm tắt đúng hay bịa đặt (hallucination)?"* | Giúp nhóm nhận ra bài toán tổng hợp tài liệu của Gấm có rủi ro ảo giác quá cao và không vừa sức lab; đồng thời thúc đẩy làm rõ vì sao các app lịch hiện tại chưa giải quyết được khâu nhập liệu. |
| Nhận phản biện | Câu hỏi tôi nhận được:<br>• Dương hỏi: *"Dùng TensorBoard hay Wandb đã hiển thị biểu đồ loss/metric rồi, AI can thiệp vào bước nào?"*<br>• Gấm hỏi: *"Check rubric nộp bài dùng script linter regex là đủ, AI có thừa không?"* | Tôi đã sửa gì:<br>• Thừa nhận Card #3 chỉ cần Rule, không nên cố nhét AI vào.<br>• Làm rõ lại Card #1: AI chỉ giúp phân tích mẫu lỗi (error pattern) chứ không can thiệp vào việc vẽ đồ thị số liệu. |
| Gom cluster / cây OST | Chủ trì gom 12 candidate của 4 bạn thành 4 cụm logic; cùng nhóm xây dựng cây OST với Outcome giảm thời gian gom việc từ 30p xuống ≤ 15p/tuần. | Nhóm có bức tranh tổng thể rõ ràng, loại bỏ được các giải pháp trá hình ("chatbot toàn năng"). |
| Chọn candidate problem | Cùng nhóm thảo luận chấm điểm 7 tiêu chí cho 3 bài shortlist; biểu quyết chọn bài toán Quản lý deadline và trích xuất thông báo (Cụm A). | Thống nhất chọn được bài toán thực tế nhất, vừa sức và có thể kiểm chứng được ngay trong lớp. |
| Kiểm chứng / research | Hỗ trợ phân tích kết quả phỏng vấn 5 bạn sinh viên; đóng góp ý kiến về khoảng trống của các công cụ Todoist, Google Calendar. | Nhóm kiên định không làm app lịch mới mà chỉ làm công cụ trích xuất trung gian có con người xác nhận (HITL). |
| Quy trình nhóm | Trực tiếp vẽ sơ đồ quy trình hiện tại (6 bước, 30 phút) và quy trình tương lai (4 bước, 15 phút) trên ASCII/Mermaid. | Xác lập rõ ràng bước nào Rule làm, bước nào AI làm và bước nào con người bắt buộc phải phê duyệt. |
| Problem Statement | Cùng Thịnh rà soát và hoàn thiện 6 trường của Problem Statement v0 và v1, đặc biệt là Success Metric có baseline và target đo được. | Đảm bảo Problem Statement chặt chẽ, không bị lỗi thiếu số liệu hay metric mơ hồ. |
| Mức can thiệp AI | Phản biện kịch liệt phương án dùng Autonomous Agent; đề xuất và bảo vệ phương án Workflow kết hợp Rule validation. | Giúp bài nhóm tránh được bẫy over-engineering và rủi ro vi phạm bảo mật dữ liệu cá nhân. |
| Quyết định | Tham gia đánh giá 4 rủi ro, đồng thuận kết luận Go ở quy mô pilot nhỏ và xác lập Ngưỡng dừng (Stop condition). | Giúp nhóm có kế hoạch thử nghiệm thực tế và tiêu chí dừng cuộc chơi an toàn. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm các góc nhìn về lãng phí thời gian khi làm bài tập kỹ thuật. | Gợi ý được ý tưởng về tự động lưu vết thực nghiệm (experiment log) và tra cứu lỗi lặp lại. | AI đưa ra các gợi ý rất viển vông kiểu "AI tự động hoàn thành bài tập thay sinh viên" (solution trá hình). | Loại bỏ các ý viển vông; tự viết lại 10 bài toán gắn với số liệu đo thời gian thực tế của bản thân. |
| CP2 Problem Card | Đóng vai "PM hoài nghi" để phản biện điểm yếu của Problem Card #1. | Chỉ ra được giả định ngầm sai lầm rằng các framework khác nhau sẽ có log stdout giống nhau. | AI khuyên nên làm Agent tự động chỉnh luôn siêu tham số (AutoML) và tự chạy đợt train tiếp theo. | Bác bỏ gợi ý làm Agent; giữ vững ranh giới an toàn: AI chỉ gợi ý giả thuyết lỗi, kỹ sư phải tự tay chỉnh tham số. |
| CP4 Research | Tìm kiếm thông tin về tính năng Natural Language Input của Todoist và Google Tasks. | Cung cấp nhanh tài liệu về cú pháp nhận diện ngày giờ tiếng Anh của Todoist. | AI khẳng định Todoist đã xử lý hoàn hảo tiếng Việt tự nhiên (thực tế thử nghiệm tiếng Việt rất hay sai lệch ngữ cảnh). | Tự kiểm tra lại bằng tài liệu và đưa nhận định chính xác vào bảng research: Todoist vẫn bỏ sót câu phức tiếng Việt. |
| CP5 Quy trình | Chuyển đổi mô tả các bước thành sơ đồ dạng text box rõ ràng. | Căn chỉnh sơ đồ ASCII và syntax Mermaid nhanh, tiết kiệm thời gian vẽ tay. | AI tự động bỏ qua bước Rule validation và tự ý nối AI thẳng vào Google Calendar mà không có bước con người xác nhận. | Bổ sung ngay bước con người duyệt (Human-in-the-loop) làm Boundary bắt buộc trước khi lưu dữ liệu. |
| CP5–6 Problem Statement | Rà soát lỗ hổng logic trong bản thảo Problem Statement v0. | Cảnh báo việc metric "nhanh hơn" là không đạt chuẩn, ép phải có baseline và target dạng số. | AI gợi ý viết Problem Statement dài dòng như một bài văn thuyết minh giải pháp. | Cắt gọt lại ngắn gọn, tuân thủ đúng 6 trường chuẩn của bài lab. |
| CP6 Mức can thiệp / quyết định | So sánh ưu/nhược điểm giữa Workflow và Autonomous Agent. | Tổng hợp nhanh các rủi ro về chi phí token và độ trễ của hệ thống Agent. | AI có xu hướng ca ngợi Agent và khuyên nhóm nên dùng Multi-agent để "bắt kịp xu hướng công nghệ". | Giữ vững nguyên tắc "đơn giản nhất đủ dùng": kiên quyết chọn Workflow vì Agent quá rủi ro cho bài toán deadline. |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**  
Khi lắng nghe phần pitch của 3 bạn trong nhóm, tôi nhận ra góc nhìn của mỗi người chịu ảnh hưởng rất lớn từ trải nghiệm cá nhân của họ. Bạn Gấm và bạn Dương xuất phát từ nỗi đau quản lý lịch học và tổng hợp tài liệu nghiên cứu, bạn Thịnh quan tâm đến việc trôi thông tin trong các kênh chat và việc các thành viên trong nhóm gặp issue nhưng không dám nói, còn bản thân tôi lại thiên về các vấn đề kỹ thuật sâu như benchmark mô hình AI hay cấu hình CUDA. Điều quý giá nhất tôi học được là khi đặt cạnh nhau, các vấn đề tưởng như rời rạc lại cùng chia sẻ một mô thức chung (pattern): thông tin bị phân tán trên quá nhiều nền tảng và người dùng phải làm "cầu nối thủ công" bằng cách copy-paste qua lại giữa các ứng dụng.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**  
Nhóm tôi đã bị rơi vào bẫy "solution-first" ngay từ những phút đầu tiên khi vừa gặp nhau. Ý tưởng ban đầu xuất hiện trong đầu mọi người là: *"Hãy làm một con bot Telegram/Discord AI xịn sò, tự động đọc mọi tin nhắn của giảng viên rồi tự tạo sự kiện vào Google Calendar"*. Khi đó, nhóm đang nghĩ về công nghệ (Bot, Agent, LLM) trước khi hiểu được thực tế. Chúng tôi chỉ thực sự tỉnh ngộ khi đặt câu hỏi: *"Nếu bot đọc nhầm một tin nhắn đùa của bạn cùng lớp thành lịch thi thì chuyện gì xảy ra?"* và *"Sinh viên có dám cấp quyền cho bot đọc toàn bộ tin nhắn riêng tư trên Zalo không?"*. Nhận ra rủi ro nghiêm trọng về bảo mật và sự tin tưởng của người dùng, nhóm đã lập tức kéo nhau về lại bước Problem: vấn đề cốt lõi chỉ là hỗ trợ nhận diện và trích xuất thông tin từ đoạn văn bản cụ thể mà người dùng chủ động cung cấp, chứ không phải là thay thế toàn bộ hành vi của người dùng.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**  
Tôi đã đổi ý hoàn toàn ở Card #3 (Kiểm tra rubric trước khi nộp bài). Ban đầu, tôi rất hào hứng với ý tưởng dùng AI để quét toàn bộ bài lab và so sánh với file RUBRIC.md. Tuy nhiên, bạn Gấm và bạn Thịnh đã phản biện rất thẳng thắn: *"Việc kiểm tra tên file, kiểm tra nhánh git hay đếm số từ hoàn toàn có thể viết bằng một script Python linter chạy trong 1 giây với độ chính xác 100%, tại sao phải tốn tiền gọi API AI để làm một việc có tính xác định cao như vậy?"*. Câu hỏi này đã đánh trúng vào điểm yếu của tôi: đang cố nhét AI vào một bài toán thuần Rule. Tôi đã đồng ý với nhóm loại bỏ ý tưởng dùng AI cho khâu này và chỉ giữ lại bài toán trích xuất deadline phi cấu trúc – nơi mà Rule thực sự bất lực trước ngôn ngữ tự nhiên.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**  
Điều làm tôi bất ngờ nhất khi xem kết quả phỏng vấn 5 bạn sinh viên thật là: **Hầu hết mọi người đều từng bị quên hoặc suýt trễ deadline ngay trong tuần vừa rồi (tại bài Lab 1)**, nhưng **không một ai muốn tải thêm một ứng dụng quản lý lịch mới**. Trước đó, giả định ngầm của nhóm là sinh viên thiếu một app quản lý thời gian tốt. Thực tế chứng minh sinh viên đã có quá nhiều app (Google Calendar, Todoist, Notion, Apple Notes), họ không thiếu nơi lưu trữ mà họ chỉ thiếu một công cụ giúp họ giảm bớt thao tác gõ tay từ tin nhắn vào app lịch sẵn có. Phát hiện này đã cứu nhóm khỏi việc lãng phí thời gian xây dựng một giao diện lịch biểu thừa thãi.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**  
Điều khó khăn nhất đối với tôi và nhóm là việc xác định **Success Metric có baseline đo được và ranh giới Boundary**. Lúc đầu, chúng tôi quen tay viết những câu sáo rỗng như *"giúp sinh viên quản lý thời gian hiệu quả hơn"* hoặc *"giảm đáng kể việc trễ hạn"*. Khi bị ép phải đưa ra con số cụ thể (Baseline là bao nhiêu? Muốn đạt Target nào? Đo bằng cách nào?), nhóm phải ngồi bấm giờ lại từng thao tác và lục lại lịch sử nộp bài cũ để có con số 30 phút/tuần và mục tiêu giảm xuống ≤ 15 phút/tuần kèm điều kiện ngặt nghèo là 0% deadline bị bỏ sót. Ngoài ra, việc vạch rõ AI **không được làm gì** (Boundary) đòi hỏi phải suy nghĩ thấu đáo về các kịch bản lỗi xấu nhất có thể xảy ra.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**  
Nếu được làm lại từ đầu, tôi sẽ yêu cầu nhóm thực hiện phỏng vấn người dùng (The Mom Test) sớm hơn ngay từ bước CP1 thay vì đợi đến CP4 mới đi hỏi. Việc có dữ liệu người thật sớm sẽ giúp nhóm không mất thời gian tranh cãi về các giả định chủ quan. Ngoài ra, tôi sẽ phản biện nhóm mạnh hơn ở khâu thiết kế dữ liệu đầu vào: thay vì chỉ nhận văn bản copy-paste, nhóm nên cân nhắc thêm trường hợp thông báo bằng hình ảnh (ảnh chụp màn hình tin nhắn hoặc ảnh chụp thời khóa biểu) vì sinh viên chia sẻ rất nhiều thông tin qua ảnh chụp màn hình.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.  
1. **Problem:** Sinh viên đại học thường xuyên nhận thông báo bài tập dưới dạng văn bản tự nhiên phi cấu trúc nằm rải rác trên LMS, Zalo, Discord, dẫn đến mất thời gian đọc lọc và nguy cơ cao bị ghi sót hoặc nhầm deadline.  
2. **Quy trình:** Người dùng dán nội dung thông báo vào hệ thống $\rightarrow$ AI bóc tách thực thể (tên môn, nhiệm vụ, thời hạn) $\rightarrow$ Rule kiểm tra định dạng ngày giờ $\rightarrow$ Sinh viên xem trước và bấm xác nhận $\rightarrow$ Hệ thống tự động đồng bộ sự kiện vào Google Calendar.  
3. **Metric:** Giảm thời gian tổng hợp lịch từ 30 phút xuống còn $\le 15$ phút/tuần (giảm $\ge 50\%$), đồng thời duy trì tỷ lệ bỏ sót deadline là 0% và tỷ lệ trích xuất đúng trường ngày giờ đạt $\ge 90\%$.  
4. **Boundary:** AI tuyệt đối không được tự ý ghi vào lịch khi người dùng chưa bấm xác nhận, không được tự đoán mò ngày nếu thông báo thiếu dữ kiện thời gian (phải bật cảnh báo), và không lưu trữ tin nhắn riêng tư lên máy chủ công cộng.  
5. **Mức can thiệp AI:** Chọn mức **Workflow** (kết hợp AI trích xuất thực thể theo cấu trúc JSON + Rule validation + Human-in-the-loop phê duyệt), kiên quyết không chọn Rule vì tiếng Việt tự nhiên quá đa dạng, và từ chối Agent vì rủi ro ảo giác và xâm phạm quyền riêng tư.  
6. **Quyết định:** Chọn **Go** ở quy mô pilot nhỏ (MVP bằng Streamlit thử nghiệm trên 20 sinh viên trong 2 tuần), kèm ngưỡng dừng rõ ràng: nếu tỷ lệ sinh viên chấp nhận lưu kết quả $< 80\%$ hoặc thời gian sửa lỗi $> 3$ phút/lần thì dừng dự án và quay về phương án nhập liệu thủ công chuẩn hóa trên Todoist.

---

## 7. Tài liệu tham khảo

- Google PAIR (People + AI Research Guidebook): [https://pair.withgoogle.com/guidebook](https://pair.withgoogle.com/guidebook)
- The Mom Test — Rob Fitzpatrick
- Opportunity Solution Tree — Teresa Torres
- Building Effective Agents — Anthropic Research: [https://www.anthropic.com/research/building-effective-agents](https://www.anthropic.com/research/building-effective-agents)
- Four Big Risks — Marty Cagan (SVPG): [https://www.svpg.com/four-big-risks](https://www.svpg.com/four-big-risks)

