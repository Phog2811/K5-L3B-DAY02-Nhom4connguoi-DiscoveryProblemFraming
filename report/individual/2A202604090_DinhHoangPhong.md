# Báo cáo cá nhân — 2A202604090_DinhHoangPhong

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đinh Hoàng Phong
- MSSV: 2A202604090
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhom4connguoi
- Link repo nhóm: https://github.com/Phog2811/K5-L3B-DAY02-Nhom4connguoi-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin| Khi chuẩn bị tham gia chương trình AI của VinUni, tôi muốn tìm nhanh luật lệ và quy trình của chương trình, để không phải lục từng nguồn rời rạc|Tôi |Khoảng 4 giờ trong một tuần, thông tin nằm ở nhiều nguồn |
| 2 |Lặp lại |Khi đi làm về đã mệt, tôi muốn vẫn giữ được lịch tập đã đặt, để đi đủ số buổi |Tôi |Định đi 4 buổi, đi 1 buổi |
| 3 |Pain từ người khác |Khi nộp đơn xin giấy tốt nghiệp sớm trên FAP, tôi muốn biết đơn đã đúng loại và đúng yêu cầu trước khi gửi, để không bị trả lại rồi phải chờ duyệt lại |Tôi và khoảng 10 bạn quen (ước chừng) |Bị trả 2 lần, mỗi lần chờ 2–3 ngày, tổng khoảng 6–9 ngày |
| 4 |Tốn thời gian |Khi viết một chức năng trong sản phẩm của khách hàng, tôi muốn biết trước chức năng đó có làm hệ thống chậm hay không, để không phải sửa lại sau khi làm xong |Tôi, team lead, tester |Chậm 20%; làm lại 2 giờ/lần; 2 lần tuần vừa rồi (khoảng 4 giờ/tuần); team lead và tester phát hiện |
| 5 |Lặp lại |Khi cần nộp đơn miễn điểm danh trên FAP, tôi muốn đơn được duyệt đúng ý ngay lần đầu, để không phải nộp lại nhiều lần |Tôi |Bị trả 2 lần, mỗi lần chờ 2–3 ngày, tổng khoảng 6 ngày |
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
| 1 |FAP: đơn bị trả rồi phải chờ lại (dòng 3, có thể gộp cả đơn miễn điểm danh ở dòng 5) |Actor rõ (sinh viên FPT), quy trình vẽ được, bước nghẽn là chờ duyệt rồi bị trả, có con số 6–9 ngày và khoảng 10 bạn cùng gặp |Có thể chỉ cần mẫu đơn hoặc checklist là đủ, nên đây là bài tốt để so sánh No AI / Rule / Workflow |
| 2 |Làm lại chức năng vì chậm 20% (dòng 4) |Actor rõ (dev), con số cụ thể (2 giờ/lần, 2 lần/tuần), có người xác nhận (team lead, tester) |Không đưa tên khách hàng hay chi tiết nội bộ vào báo cáo; nhóm có thể ít hiểu domain này |
| 3 |Tìm luật lệ, quy trình chương trình VinUni (dòng 1) |Có con số 4 giờ, thông tin ở nhiều nguồn |Ít lặp lại hơn hai cái trên, nên cần nghĩ xem impact kéo dài hay chỉ một lần |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nộp đơn xin giấy tốt nghiệp sớm trên FAP, tôi muốn biết đơn đã đúng loại và đúng yêu cầu trước khi gửi, để không bị trả lại rồi phải chờ duyệt lại |
| Actor | Sinh viên ĐH FPT nộp đơn trên FAP (tôi và khoảng 10 bạn quen, ước chừng)|
| Thời điểm / bối cảnh |Khi cần xin giấy tốt nghiệp sớm hoặc miễn điểm danh |
| Quy trình hiện tại (3–7 bước) |Xem sơ đồ bên dưới |
| Bottleneck (bước nào, mất bao nhiêu phút) |Chờ duyệt 2–3 ngày mỗi lần, và chỉ khi đơn bị trả mới biết loại đơn hoặc nội dung chưa đúng; bị trả 2 lần |
| Impact (nếu không giải thì sao) |thì tiếp tục viết lại |
| Success metric (baseline → target) |khoảng 6–9 ngày (theo đơn giấy tốt nghiệp), bị trả 2 lần. 2 ngày |
| Phương án không dùng AI |Đơn có hướng dẫn đầy đủ; xem mẫu đơn của các anh chị đi trước |
| Giả thuyết về AI (nếu có) |chưa có |
| Cảm nhận nhanh | Chưa biết |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 6–9 ngày

[Chọn loại đơn + điền thông tin cá nhân, tiêu đề, nội dung: ~10']
→ [FAP thông báo có đơn mới]
→ [Chờ duyệt: 2–3 ngày]  ← BOTTLENECK (biết đơn sai chỉ sau khi chờ xong)
→ [Bị trả: nội dung chưa đúng ý / nhầm loại đơn]
→ [Nộp lại:10p' ] → [Chờ duyệt: 2–3 ngày] → ... (bị trả 2 lần)
→ [Được duyệt]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story |Khi viết một chức năng trong sản phẩm của khách hàng, tôi muốn biết trước chức năng đó có làm hệ thống chậm hay không, để không phải sửa lại sau khi làm xong |
| Actor |Tôi (lập trình viên), tester, team lead |
| Thời điểm / bối cảnh |Sau khi viết xong một chức năng và đưa cho tester |
| Quy trình hiện tại (3–7 bước) |Xem sơ đồ bên dưới |
| Bottleneck (bước nào, mất bao nhiêu phút) |Việc chậm 20% chỉ bị phát hiện sau khi chức năng đã qua tester, kéo theo vòng báo, đo, review (~1 giờ) và viết lại (~2 giờ) |
| Impact (nếu không giải thì sao) |Trễ task, mất thời gian của team |
| Success metric (baseline → target) |Baseline: 2 lần/tuần, mỗi lần khoảng 3 giờ. Target và cách đo: (bạn điền) |
| Phương án không dùng AI |chưa có |
| Giả thuyết về AI (nếu có) |chưa có |
| Cảm nhận nhanh | Chưa biết |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 3 giờ làm lại mỗi lần, 2 lần tuần vừa rồi

[Viết code: ?'] → [Tự test sơ qua: ?'] → [Đưa tester] → [Tester chạy thử, thấy chậm]
→ [Tester báo team lead; team lead hiểu vấn đề, đo hiệu suất, review code, chỉ ra lỗi: ~1 giờ]  ← BOTTLENECK
→ [Tôi nghe review, tìm nguyên nhân, viết lại code tối ưu: ~2 giờ]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị tham gia chương trình AI của VinUni, tôi muốn tìm nhanh luật lệ và quy trình của chương trình, để không phải lục từng nguồn rời rạc |
| Actor |Tôi (người chuẩn bị tham gia chương trình) |
| Thời điểm / bối cảnh |Tuần chuẩn bị trước khi bắt đầu chương trình |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) |Tìm được tài liệu nhưng khó hiểu, phải hỏi lại nhiều người đã biế |
| Impact (nếu không giải thì sao) |Chỉ tốn thời gian, chưa gặp hậu quả khác |
| Success metric (baseline → target) |Baseline: khoảng 4 giờ trong tuần vừa rồi. 1 giờ |
| Phương án không dùng AI |không |
| Giả thuyết về AI (nếu có) | chưa có|
| Cảm nhận nhanh | Chưa biết |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 4 giờ trong một tuần

[Tìm nguồn trên web: 10'] → [Mở và đọc tài liệu PDF, web: 30'] 
→ [Đọc hiểu luật, quy trình: ?']  ← khó hiểu
→ [Hỏi lại người đã biết / hỏi ban tổ chức: ?']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Actor chưa chặt. “Khoảng 10 bạn quen cũng gặp” là ước chừng, chưa rõ họ bị trả vì lý do giống bạn hay khác, và là loại đơn nào |Actor chưa chặt, “10 bạn” là ước chừng |Ghi rõ “khoảng 10 bạn quen, ước chừng, chưa kiểm chứng”; hoặc hỏi nhanh 2–3 bạn xem họ có bị trả đơn không rồi cập nhật |
|Hai lý do bị trả là hai nguyên nhân khác nhau (nội dung chưa đúng ý, và nhầm loại đơn). Chưa biết lý do nào hay xảy ra hơn nên chưa rõ đang giải vấn đề nào |Hai lý do bị trả là hai nguyên nhân khác nhau |Tách rõ trong quy trình: lần trả thứ nhất do lý do nào, lần thứ hai do lý do nào |
|Thời gian chờ 2–3 ngày có thể do phía trường duyệt, không phải do sinh viên. Nếu vậy, phần bạn tác động được chỉ là số lần bị trả |Thời gian chờ có thể do phía trường |Ghi trong bottleneck: khoảng chờ do phía trường duyệt, phần bạn tác động được là số lần bị trả |
|Metric chưa chặt. Target “còn 1 ngày” chưa rõ là mỗi lần chờ hay tổng; mẫu mới chỉ 2 lần bị trả của bạn; chưa có cách đo |Metric chưa rõ, chưa có cách đo |Chốt một metric (số lần bị trả: 2 → 0, hoặc tổng số ngày) và ghi cách đo |
|Có thể đang nhảy sang AI quá sớm. Bạn tự nói đơn có hướng dẫn đầy đủ là đủ, và impact chỉ là viết lại đơn. Chưa có bằng chứng mức No AI không đủ |Có thể nhảy sang AI quá sớm |Ghi nhận mức No AI (đơn có hướng dẫn) là phương án đầu tiên, và “chưa có bằng chứng No AI không đủ” |
|Impact thấp. Bạn mô tả chỉ tốn khoảng 10 phút viết lại và chờ thêm. Tại sao đáng giải so với hai card kia? |Impact thấp |Giữ nguyên impact nhỏ, hoặc bổ sung nếu bạn còn nhớ hậu quả cụ thể nào khác |
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

