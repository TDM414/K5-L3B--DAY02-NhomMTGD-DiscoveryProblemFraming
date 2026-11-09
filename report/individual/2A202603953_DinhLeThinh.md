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
| 5 | Lặp lại | Khi bắt đầu buổi họp nhóm, tôi muốn có sẵn agenda và trạng thái các việc từ buổi trước để không mất thời gian ôn lại đầu giờ | Cả team | 10–15 phút đầu mỗi buổi họp bị dùng để nhớ lại việc cũ; họp nhóm ~2 lần/tuần |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận thông báo thay đổi deadline/format nộp bài, tôi muốn biết chính xác điều gì đổi và ai bị ảnh hưởng để cập nhật kế hoạch cá nhân | Học viên trong nhóm | Thông báo nằm rải rác ở nhiều kênh (email, Discord, LMS); đã từng suýt nộp sai format |
| 7 | Pain từ người khác | Khi thành viên mới vào nhóm, tôi muốn họ tự nắm được quy ước và lịch sử quyết định của nhóm để không phải giải thích lại nhiều lần | Người hướng dẫn/leader, thành viên mới | Mỗi thành viên mới tốn ~20–30 phút được giải thích lại; lặp lại mỗi khi có người mới |
| 8 | Tốn thời gian | Khi chuẩn bị nộp bài, tôi muốn kiểm tra nhanh checklist yêu cầu nộp để tránh thiếu file hoặc sai định dạng | Cả team | Mất ~10 phút rà checklist mỗi lần nộp; rủi ro thiếu mục nếu làm vội |

**Nếu có dùng AI để gợi ý thêm:** 
- Giữ lại #5 (agenda họp) và #6 (thay đổi deadline/format): AI gợi ý từ lăng kính "lặp lại" và "cần đọc, tổng hợp nhiều thông tin"; mình thấy khớp với trải nghiệm thật của nhóm.
- Bỏ gợi ý "chatbot hỏi đáp toàn bộ tài liệu chương trình": phạm vi quá rộng, khó đo success metric trong thời gian lab.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp issue (#3) | Pain thật nhiều người gặp phải; ghi nhận khoảng 30 phút mỗi tuần | |
| 2 | Tìm checkpoint cũ (#4) | Xảy ra khoảng 2 lần/tuần, mỗi lần khoảng 15 phút | Chưa rõ checkpoint thường được lưu ở kênh nào; chưa rõ 15 phút chỉ tính thời gian tìm hay gồm cả hỏi lại và xác nhận thông tin. |
| 3 | Chuẩn bị họp nhóm (#5) | Lặp lại ~2 lần/tuần, ảnh hưởng cả team; dễ đo bằng thời gian đầu buổi họp | Chưa bấm giờ chính xác; chưa rõ ai đang điều phối họp |

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
| Job Story | Khi bắt đầu buổi họp nhóm, tôi muốn có sẵn agenda và trạng thái các việc từ buổi trước, để không mất thời gian ôn lại đầu giờ và tập trung vào quyết định mới. |
| Actor | Người điều phối họp (thường là leader hoặc người được phân công); cả nhóm là người hưởng lợi |
| Thời điểm / bối cảnh | Đầu mỗi buổi họp nhóm, khoảng 2 lần/tuần; ghi nhận 10–15 phút đầu buổi bị dùng để nhớ lại việc cũ |
| Quy trình hiện tại (3–7 bước) | 1. Mở lại kênh/tài liệu của buổi họp trước · 2. Đọc lại các việc đã giao và trạng thái · 3. Nhớ lại ai chưa xong, vì sao · 4. Viết agenda sơ bộ cho buổi họp mới · 5. Chia sẻ agenda trong kênh nhóm trước hoặc đầu buổi họp |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3: đọc lại và tổng hợp trạng thái việc cũ; ước lượng 10–15 phút đầu mỗi buổi họp. Cần bấm giờ để xác nhận. |
| Impact (nếu không giải thì sao) | Mỗi tuần mất khoảng 20–30 phút tổng cộng cho cả nhóm; buổi họp dễ sa vào ôn lại việc cũ thay vì ra quyết định mới. |
| Success metric (baseline → target) | Baseline sơ bộ: 10–15 phút đầu buổi họp × ~2 buổi/tuần. Target đề xuất: ≤5 phút đầu buổi họp có agenda và trạng thái việc cũ sẵn sàng; không tăng số việc bị bỏ sót. Đo bằng thời điểm agenda được gửi trước/sau khi họp bắt đầu và số việc cũ không được nhắc lại. |
| Phương án không dùng AI | Template agenda + bảng trạng thái việc cố định; cuối mỗi buổi họp, người điều phối cập nhật ngay trạng thái và việc tiếp theo để buổi sau dùng lại. |
| Giả thuyết về AI (nếu có) | AI có thể tóm tắt ghi chú/tin nhắn của buổi họp trước thành agenda nháp và danh sách việc còn mở; người điều phối rà soát và chỉnh trước khi gửi nhóm. Chỉ cân nhắc sau khi template + bảng trạng thái tỏ ra chưa đủ. |
| Cảm nhận nhanh | Rule / Workflow trước; AI chỉ hỗ trợ bước tóm tắt nháp, không tự gửi. |

Quy trình nháp hiện tại:

```
[Mở lại kênh/tài liệu buổi họp trước]
  → [Đọc lại việc đã giao và trạng thái]
  → [Nhớ lại ai chưa xong, vì sao]  ← BOTTLENECK (~10–15 phút đầu buổi họp, cần bấm giờ)
  → [Viết agenda sơ bộ cho buổi mới]
  → [Chia sẻ agenda trong kênh nhóm]
  ```

### Card muốn pitch nhất

- Card số: #1 — Tổng hợp issue (#3)
- Vì sao: Đây là pain lặp lại hằng tuần, ảnh hưởng trực tiếp đến deadline chung của cả nhóm; baseline (khoảng 30 phút/tuần) và target (≤15 phút/tuần) rõ ràng, dễ đo. Phương án không dùng AI (bảng tiến độ + mốc check-in) đủ đơn giản để thử ngay, nên có thể so sánh công bằng trước khi cân nhắc AI.
- Câu hỏi muốn nhóm phản biện: (1) 30 phút/tuần là thời gian của một người hay cả nhóm? (2) Ai thường là người tổng hợp tiến độ — có phải lúc nào cũng là leader không? (3) Nếu chỉ dùng bảng tiến độ + mốc check-in cố định, nhóm có thực sự duy trì cập nhật đều không, hay sẽ tái phát việc hỏi rải rác trong kênh?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline "30 phút/tuần" chưa rõ là của một người hay cả nhóm | Đồng ý | Ghi rõ trong Card #1 và câu hỏi pitch: cần xác nhận phạm vi thời gian |
| "Success metric" chỉ đo thời gian, chưa đo chất lượng (issue phát hiện muộn) | Đồng ý | Thêm điều kiện "không tăng số issue được phát hiện sát hoặc sau deadline" vào target |
| Giả thuyết AI có thể là giải pháp quá sớm khi chưa thử bảng tiến độ | Đồng ý | Đặt phương án không dùng AI (bảng tiến độ + check-in) làm bước thử trước; AI chỉ là giả thuyết dự phòng |
| Actor chưa xác định rõ ai tổng hợp tiến độ | Đồng ý | Ghi chú "cần xác nhận ai thường đảm nhiệm" trong trường Actor |

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
