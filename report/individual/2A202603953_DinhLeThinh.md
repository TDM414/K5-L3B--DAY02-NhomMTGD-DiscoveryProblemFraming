## 1. Thông tin học viên

- Họ tên: Đinh Lê Thịnh
- MSSV: 2A202603953
- Email trường (không bắt buộc, repo có thể để public): 26ai.thinhdl@vinuni.edu.vn
- Tên nhóm: NhomMTGD
- Link repo nhóm: https://github.com/TDM414/L3B--DAY02-NhomMTGD-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi tham gia chương trình có nhiều kênh thông báo, tôi muốn cập nhật đầy đủ thông tin kịp thời để không bỏ sót các thông tin quan trọng | Học viên, Staff | Suýt trễ workshop |
| 2 | Tốn thời gian | Khi làm lab có nhiều tài liệu để đọc hay tham khảo, tôi muốn tìm nhanh yêu cầu để hoàn thành để không tốn thời gian dò lại các tài liệu | Học viên | Mất khoảng 2 phút mỗi lần và xảy ra khoảng 10 lần mỗi bài lab |
| 3 | Lặp lại | Khi nhóm đến deadline nộp bài tôi muốn biết thành viên nào còn gặp issues để nhóm kịp hoàn thành công việc chung | Cả team | Mỗi tuần 1 lần khoảng 30 phút |
| 4 | Tốn thời gian | Khi cần tìm lại quyết định hoặc câu trả lời đã chốt tối muốn tìm lại nội dung đó nhanh để không hỏi lại hoặc tranh luận lại | Cả team | Khoảng 2 lần mỗi tuần khoảng 15 phút |
| 5 | | | | |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp issue (#3) | Pain thật nhiều người gặp phải; ghi nhận khoảng 30 phút mỗi tuần | |
| 2 | Tìm checkpoint cũ (#4) | Xảy ra khoảng 2 lần/tuần, mỗi lần khoảng 15 phút | Chưa rõ checkpoint thường được lưu ở kênh nào; chưa rõ 15 phút chỉ tính thời gian tìm hay gồm cả hỏi lại và xác nhận thông tin. |
| 3 | | | |

### Problem Card #1 — Tổng hợp issue (#3)

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhóm gần đến deadline nộp bài, tôi muốn biết thành viên nào còn gặp issue, để nhóm kịp hỗ trợ và hoàn thành công việc chung. |
| Actor | Thành viên nhóm; người hỏi/tổng hợp tiến độ (cần xác nhận ai thường đảm nhiệm việc này) |
| Thời điểm / bối cảnh | Khi nhóm đang làm bài và gần deadline; theo ghi nhận hiện tại khoảng 1 lần mỗi tuần. |
| Quy trình hiện tại (3–7 bước) | 1. Hỏi tiến độ trong kênh nhóm · 2. Chờ thành viên phản hồi · 3. Hỏi thêm người chưa nêu rõ tình trạng hoặc issue · 4. Tổng hợp ai đã xong, ai đang vướng · 5. Nhóm thống nhất việc cần hỗ trợ tiếp theo. Cần chỉnh lại nếu quy trình thực tế khác. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Hỏi và tổng hợp tình hình; ghi nhận khoảng 30 phút mỗi tuần cho hoạt động này. Cần xác nhận đây là thời gian của một người hay cả nhóm. |
| Impact (nếu không giải thì sao) | Issue có thể được phát hiện muộn, khiến nhóm còn ít thời gian hỗ trợ thành viên trước deadline. |
| Success metric (baseline → target) | Baseline sơ bộ: khoảng 30 phút/tuần. Target đề xuất: ≤15 phút/tuần để tổng hợp issue, đồng thời không tăng số issue được phát hiện sát hoặc sau deadline. Đo thời gian thực tế trong một tuần và ghi số issue phát hiện muộn. |
| Phương án không dùng AI | Dùng bảng tiến độ chung ghi người phụ trách, trạng thái, issue đang gặp và hạn hoàn thành; cả nhóm cập nhật trước mốc check-in cố định. |
| Giả thuyết về AI (nếu có) | Nếu cập nhật tiến độ nằm rải rác trong tin nhắn, công cụ có thể gom các thông tin thành danh sách issue để nhóm rà soát. Thành viên phải xác nhận nội dung trước khi nhóm hành động; cần thử bảng tiến độ trước để xem đã đủ chưa. |
| Cảm nhận nhanh | Rule / Workflow; thử bảng tiến độ và mốc check-in trước, chưa có căn cứ để cần Agent. |

Quy trình nháp hiện tại:

```text
[Hỏi tiến độ trong kênh nhóm]
  → [Chờ thành viên phản hồi]
  → [Hỏi thêm người chưa nêu rõ tình trạng]
  → [Tổng hợp người đã xong / đang vướng]  ← BOTTLENECK (~30 phút/tuần, cần xác nhận phạm vi)
  → [Thống nhất việc cần hỗ trợ tiếp theo]
```

### Problem Card #2 — Tìm checkpoint cũ (#4)

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần tìm lại quyết định hoặc câu trả lời nhóm đã chốt, tôi muốn tìm được nội dung đó nhanh, để không phải hỏi lại hoặc thảo luận lại từ đầu. |
| Actor | Thành viên nhóm |
| Thời điểm / bối cảnh | Khi tiếp tục làm bài và cần tra cứu nội dung đã trao đổi; ghi nhận khoảng 2 lần mỗi tuần. |
| Quy trình hiện tại (3–7 bước) | 1. Nhớ lại chủ đề hoặc từ khóa · 2. Mở kênh trao đổi của nhóm · 3. Tìm hoặc cuộn lại tin nhắn · 4. Đọc các tin liên quan để xác định câu trả lời/quyết định cuối · 5. Hỏi lại nhóm nếu chưa tìm thấy hoặc chưa chắc. Cần chỉnh theo kênh và cách tìm thực tế. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Tìm và xác định đúng nội dung đã chốt; ước lượng khoảng 15 phút/lần, khoảng 2 lần/tuần. Cần bấm giờ để xác nhận. |
| Impact (nếu không giải thì sao) | Mất khoảng 30 phút mỗi tuần theo ước lượng hiện tại; có thể hỏi lại hoặc lặp lại thảo luận nếu không tìm thấy quyết định cũ. |
| Success metric (baseline → target) | Baseline sơ bộ: 15 phút/lần × 2 lần/tuần = khoảng 30 phút/tuần. Target đề xuất: ≤7 phút/lần và không tăng số lần hỏi lại. Đo từ lúc bắt đầu tìm đến khi xác nhận đúng nội dung. |
| Phương án không dùng AI | Ghi quyết định vào một tài liệu chung theo ngày, chủ đề, nội dung đã chốt và người xác nhận; đặt tiêu đề nhất quán để tìm kiếm. |
| Giả thuyết về AI (nếu có) | Có thể thử tìm kiếm ngữ nghĩa để gợi ý các trao đổi liên quan, nhưng kết quả cần dẫn về tin nhắn nguồn và thành viên tự xác nhận. Trước tiên thử log quyết định chung để xem cách đơn giản này đã giải quyết đủ chưa. |
| Cảm nhận nhanh | Rule / Workflow trước; chuẩn hóa nơi ghi quyết định và cách đặt tên. Chỉ cân nhắc AI nếu cách này chưa đủ. |

Quy trình nháp hiện tại:

```text
[Nhớ chủ đề / từ khóa cần tìm]
  → [Mở kênh trao đổi nhóm]
  → [Tìm hoặc cuộn lại tin nhắn]
  → [Đọc và xác định nội dung đã chốt]  ← BOTTLENECK (~15 phút/lần, cần bấm giờ xác nhận)
  → [Hỏi lại nhóm nếu chưa chắc]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

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
