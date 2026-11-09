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
| Pitch Problem Card |Chọn Card #1 (FAP) làm card pitch; 3 card của tôi là candidate #1–#3 trong bảng pitch của nhóm. Khi pitch, tôi nhấn mạnh pain point bị trả đơn phải chờ 6–9 ngày. Nhóm phản hồi rằng thời gian chờ là do trường, tác động của sinh viên chỉ là 10 phút viết lại đơn. |Card FAP vào shortlist nhưng xếp thứ 3 (23 điểm) và bị loại vì impact thấp và thời gian chờ do phía trường quyết định. |
| Phản biện bài của bạn khác | Nhóm có trao đổi nhưng chưa ghi lại vào biên bản. Tôi đã đặt câu hỏi cho Vỹ ở bài toán tìm hạn nộp: "Nếu lớp có bảng chung thì ai sẽ là người đảm bảo cập nhật liên tục để bảng không bị cũ?" |Vỹ đã đồng ý với rủi ro này và đưa "người phụ trách cập nhật bảng" vào quy trình tương lai cũng như thêm phần Boundary giới hạn vai trò của AI. |
| Nhận phản biện | Câu hỏi tôi nhận được: phản biện của AI ở CP2. Câu hỏi từ Vỹ: "Đơn bị trả thường do sinh viên điền sai nội dung hay chọn nhầm loại đơn trên hệ thống?"| Tôi đã sửa gì: Đã ghi "ước chừng" ở trường Actor của Card #1. Tôi cũng nhận ra rằng hai lỗi này là khác nhau và đã điều chỉnh quy trình để phân rõ nguyên nhân.|
| Gom cluster / Bản nháp do Vỹ tổng hợp bằng AI; tôi được giao là người chính CP3. Tôi đã rà soát cluster, cây OST và thống nhất phân loại. |Hai card của tôi (#1, #2) được xếp chính xác vào cluster D "Phát hiện lỗi quá muộn". Rút gọn cây OST tập trung vào outcome giảm thời gian tra cứu. |
| Chọn candidate problem |Nhóm đề xuất chọn "Tìm hạn nộp và yêu cầu mới nhất" (#4 + #11). Nhóm trao đổi thống nhất qua chat, chưa có biên bản chấm điểm chính thức. Tôi đồng ý chọn bài này vì impact tác động tới nhiều sinh viên hơn bài FAP của tôi.|Nhóm chốt candidate #4 + #11. Card FAP của tôi không được chọn vì impact thấp và khó can thiệp vào quy trình của trường. |
| Kiểm chứng / research |Dương (kiểm chứng) và Hoàng (research) được giao. Phỏng vấn và survey hiện chưa thực hiện nên tôi chưa trực tiếp lấy số liệu ngoài nhóm. |Báo cáo nhóm ghi nhận Value đang ở mức rủi ro Cao vì chưa có kiểm chứng ngoài nhóm, tôi đồng tình cần ưu tiên phỏng vấn ở bước sau. |
| Quy trình nhóm |Vỹ là người chính làm CP5. Tôi đã góp ý rà soát sơ đồ quy trình hiện tại và xác nhận số liệu thời gian chỉ đang là ước lượng. |Nhóm chốt được Bottleneck chính ở bước 4 (tìm, cuộn đọc tin nhắn mất 8 phút) trong quy trình hiện tại. |
| Problem Statement |Vỹ viết v0. Tôi đã góp ý phần Success Metric cần thiết thực hơn thay vì chỉ đo thời gian. |Nhóm đã đồng ý sửa thành v1: Thêm đo lường "số lần nộp trễ" và "số câu hỏi lặp lại trong group" để đánh giá chính xác hiệu quả. |
| Mức can thiệp AI |Tôi được giao CP6, cùng nhóm phân tích ma trận độ mơ hồ × độ phức tạp. Bài toán có hạn nộp đúng/sai rõ ràng, nên tôi đồng tình chưa cần đến Workflow.|Chốt đề xuất mức No AI + Rule cho pilot (dùng bảng ghim và nhắc hẹn lịch), không dùng AI đề xuất vì rủi ro sai sót thông báo. |
| Quyết định |Tham gia thảo luận và chốt phương án cuối cùng cùng cả nhóm. |Đồng thuận chốt Not Yet vì Value rủi ro cao (chưa phỏng vấn người ngoài nhóm) và cần chạy pilot bảng ghim trước khi nghĩ tới AI. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan |Tự liệt kê 3 việc (VinUni, gym, FAP), sau đó nhờ AI hỏi thêm chi tiết, ghép Job Story nháp và soát số liệu |Chỉ ra dòng gym chưa có bước nghẽn, "nhàm chán" là cảm xúc không đo được; nhắc ghi con số thật cho từng dòng |AI dùng số 12 giờ theo lời tôi mà chưa kiểm; AI cũng đánh giá FAP là ứng viên mạnh nhất trước khi biết impact thấp |Tôi tự sửa 12 giờ thành 4 giờ; bỏ ý "nhàm chán" và thay bằng việc làm lại chức năng chậm 20% và đơn miễn điểm danh, mỗi dòng có số thật |
| CP2 Problem Card |Nhờ AI đề xuất top 3 và phản biện Card #1 theo 6 điểm yếu |Chỉ ra metric chưa rõ (mỗi lần chờ hay tổng), có thể nhảy sang AI quá sớm, hai lý do bị trả là hai nguyên nhân khác nhau |Điểm "chờ do phía trường duyệt" là suy đoán, AI chưa biết quy trình thật của FAP; AI xếp FAP hạng 1 nhưng nhóm xếp hạng 3 vì impact thấp |Đã ghi "ước chừng" ở Actor. Ghi nhận thời gian chờ thuộc về trường, tác động của sinh viên chỉ là số lần bị trả đơn và thời gian điền lại form. |
| CP4 Research |Nhờ AI tìm kiếm các công cụ tự động tổng hợp lịch từ tin nhắn Zalo/Messenger. |Gợi ý được tính năng nhắc hẹn của Zalo và tích hợp Gemini trong Gmail. |Các giải pháp AI tự động hóa hoàn toàn với Zalo không khả thi, hướng dẫn cũ từ năm 2021. |Loại bỏ kỳ vọng làm Workflow đọc tin Zalo tự động, chốt lại bài học là sử dụng tính năng nhắc lịch thủ công làm Rule thay vì dùng AI. |
| CP5 Quy trình |Dùng AI (Claude/Gemini) để cấu trúc hóa quy trình chữ thành sơ đồ bước nối tiếp. |Chuyển đổi rành mạch các actor và input/output từng bước. |AI ban đầu phân bổ thời gian sai và không xác định đúng vị trí của bottleneck (đặt nghẽn ở khâu giảng viên đính chính). |Tự điều chỉnh và chốt Bottleneck nằm ở bước "SV tìm, cuộn đọc tin nhắn" với 8 phút/lần. |
| CP5–6 Problem Statement |Cung cấp cho AI bản v0 để kiểm tra lỗ hổng logic giữa Bottleneck và Boundary. |Chỉ ra rằng nếu nguyên nhân gốc là "lớp thiếu một nơi chốt thông tin" thì Success Metric không thể chỉ đo thời gian. |Gợi ý metric chung chung như "độ hài lòng của sinh viên". |Bỏ metric cảm tính, tự đưa số liệu cụ thể cần đo vào v1: Đếm số lần nộp trễ và số câu hỏi lặp lại trên nhóm chat. |
| CP6 Mức can thiệp / quyết định |Dùng AI để so sánh ưu/nhược điểm giữa Workflow và mức No AI + Rule cho bài toán tìm hạn nộp. |Giải thích rất rõ rủi ro Value và Viability nếu áp dụng AI khi bài toán có độ phức tạp thấp. |Đề xuất chạy AI song song với con người ngay lập tức (Go) để đối chiếu. |Bác bỏ đề xuất "Go", tự thống nhất với nhóm đưa ra quyết định "Not Yet" và viết rõ các ngưỡng dừng cho pilot No AI trước. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Khi nghe Vỹ và Dương pitch về problem tìm hạn nộp môn học và tìm phòng trọ, tôi nhận ra problem về hệ thống FAP của mình có tác động (impact) quá nhỏ. Hơn nữa, "nút thắt" (bottleneck) tốn thời gian nhất lại nằm ở khâu chờ nhà trường duyệt, tức là nằm ngoài tầm kiểm soát của sinh viên. Qua đó, tôi học được rằng một problem đáng giải quyết không chỉ cần tần suất lặp lại cao mà actor (người dùng) còn phải có khả năng chủ động can thiệp vào quy trình đó
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có, nhóm đã bị "solution-first" khi đưa ngay các ý tưởng như "Bảng deadline chung được ghim", "AI trích hạn nộp", và "Lọc, gắn nhãn email" vào làm các nhánh cơ hội (Opportunity). Nhóm nhận ra điều này khi rà soát lại cây Opportunity Solution Tree (OST) và thấy rằng đó là các công cụ giải pháp chứ không phải nỗi đau (pain) hay nhu cầu thật sự của người dùng. Nhóm xử lý bằng cách gạch bỏ các ý đó và viết lại thành nhu cầu gốc rễ: "Lớp thiếu một nơi chốt thông tin mới nhất".
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Ban đầu, tôi đánh giá rất cao bài toán đơn FAP bị trả và xếp nó ở vị trí thứ nhất trong báo cáo cá nhân. Tuy nhiên, AI đã phản biện rằng impact của việc này khá thấp (chỉ tốn khoảng 10 phút để viết lại đơn) và thời gian chờ 6-9 ngày hoàn toàn do quy trình của trường. Khi chấm điểm chéo, nhóm cũng chỉ đánh giá problem này được 23 điểm (xếp thứ 3). Tôi đã đổi ý, đồng thuận loại bỏ card của mình để chọn bài toán "Tìm hạn nộp và yêu cầu mới nhất" (#4 + #11) vì nó mang tính phổ biến và khả thi để can thiệp hơn.
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ nhất là khi nhìn vào kết quả tổng hợp: nhóm hiện tại chưa hề thực hiện một cuộc phỏng vấn hay khảo sát nào với người dùng thật. Tất cả các con số thời gian như "mất 20 phút/lần", "8 phút cuộn đọc chat", hay "3-4 lần/tuần" hoàn toàn chỉ là tự ghi nhận và giả thuyết đầu vào của thành viên nhóm. Việc nhận ra dự án đang xây dựng hoàn toàn trên các ước lượng chủ quan khiến tôi hiểu vì sao rủi ro Value (giá trị) của nhóm hiện tại lại bị xếp ở mức Cao.
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Với bài toán của nhóm, điều khó nhất là xác định chính xác Success Metric (Tiêu chí thành công). Ban đầu v0 chỉ định hướng vào việc đo lường tổng thời gian tìm kiếm. Tuy nhiên, nếu sinh viên tìm hạn nhanh nhưng lại làm theo thông báo cũ đã bị đính chính, thì bài toán cốt lõi vẫn chưa được giải quyết. Do đó, chúng tôi phải vất vả định hình lại và bổ sung thêm hai metric thực tế hơn: đưa số lần nộp trễ về 0 và giảm thiểu "số câu hỏi lặp lại" trong nhóm chat.
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, tôi sẽ thúc đẩy nhóm tiến hành phỏng vấn 3-5 bạn học ngoài nhóm ngay từ những ngày đầu thay vì chỉ ngồi tự ước lượng thời gian với nhau. Đồng thời, tôi sẽ phản biện nhóm mạnh hơn ở yếu tố Viability (Tính khả thi) đối với phương án No AI. Việc duy trì một bảng tính deadline hoàn toàn phụ thuộc vào "một người phụ trách cập nhật thủ công" là một rủi ro rất lớn; tôi sẽ đặt câu hỏi gay gắt hơn về việc làm sao để người này duy trì động lực cập nhật bảng liên tục trong suốt học kỳ.
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Bài toán của nhóm tập trung vào sự bất tiện của sinh viên học nhiều môn khi phải tra cứu hạn nộp bài rải rác trên các kênh chat, LMS và email. Quy trình hiện tại bị nghẽn (bottleneck) ở bước sinh viên phải cuộn tìm thông báo trong nhóm chat, gây tốn khoảng 8 phút mỗi lần và dễ dẫn đến bỏ sót thông tin đã đính chính. Nhóm đặt metric kỳ vọng là giảm thời gian tìm kiếm xuống dưới 5 phút, không còn sinh viên nộp trễ và giảm thiểu câu hỏi lặp lại trên group lớp. Boundary cốt lõi được đặt ra là AI không được phép tự động đăng hay sửa hạn nộp, mọi thông tin mâu thuẫn phải ưu tiên nguồn chính thức từ giảng viên. Vì bài toán có độ phức tạp thấp, nhóm quyết định chọn mức can thiệp là No AI kết hợp với Rule (sử dụng bảng ghim chung và nhắc hẹn tự động). Kết luận hiện tại là nhóm đưa ra quyết định "Not Yet", yêu cầu phải kiểm chứng thực tế và chạy pilot phương án bảng thủ công trước khi cân nhắc áp dụng AI.
---

## 7. Tài liệu tham khảo
Báo cáo nhóm Nhom4connguoi — Day 02 Discovery & Problem Framing (File: group_report.md).   
Hướng dẫn và framework của lab: docs/01-worksheet.md.   
Google Classroom Help, View due dates and events in a calendar: https://support.google.com/edu/classroom/answer/6272985.   
Quản Trị Mạng, Cách tạo nhắc hẹn, kỷ niệm nhóm trên Zalo (2021): https://quantrimang.com/cong-nghe/cach-tao-lich-hen-tren-nhom-chat-zalo-pc-156529.   
Google Workspace Updates, Quickly add events to Google Calendar based on your emails with Gemini in Gmail (03/2025): https://workspaceupdates.googleblog.com/2025/03/add-events-to-google-calendar-using-gemini-in-gmail.html.   
Zapier, Extract due dates from Gmail, analyze with AI, run code, and create Google Calendar reminders: https://zapier.com/templates/details/34f7f11d27aa22bcd0b5e4207c4537d2d59e0c4451dd56dfc3a4199c482ba2d8.
-

