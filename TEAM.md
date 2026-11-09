# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.
>
> **Phạm vi bản này:** mục "Đóng góp cụ thể" và "Bằng chứng" chỉ dựa trên file và commit có trong repo. Vai trò và phân công là **đề xuất, các thành viên chưa xác nhận**. Mục "chưa ghi nhận" là phần repo chưa có dữ liệu, thành viên liên quan tự bổ sung.

## Thông tin nhóm

- Tên nhóm: Nhom4connguoi
- Candidate problem nhóm chọn (1 câu): Khi sắp làm bài, sinh viên học nhiều môn muốn biết chắc hạn nộp và yêu cầu mới nhất của từng môn, để không phải lục lại nhiều kênh, không nộp trễ và không làm theo thông báo cũ.
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet (đề xuất)

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 |Đinh Hoàng Phong |2A202604090 |Nhóm trưởng; điều phối, chốt quyết định (đề xuất) |Phog2811 |
| 2 |Đỗ Hồng Vỹ |2A202604107 |Thành viên; vẽ quy trình, viết Problem Statement v0 (đề xuất) |Do-Hong-Vy |
| 3 |Nguyễn Việt Hoàng |2A202604104 |Thành viên; phụ trách research (đề xuất) |viethoang126 |
| 4 |Nguyễn Ánh Dương |2A202604087 |Thành viên; phụ trách kiểm chứng (đề xuất) |nganhduong123 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

Bảng dưới là phân công đề xuất, chưa phải ghi nhận việc đã hoàn thành. Bản nháp hiện tại của `group_report.md` do Vỹ tổng hợp với hỗ trợ của AI; người chính chịu trách nhiệm rà soát và chốt phần của mình.

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Đinh Hoàng Phong | Đỗ Hồng Vỹ | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Nguyễn Ánh Dương | Nguyễn Việt Hoàng | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Việt Hoàng | Đỗ Hồng Vỹ | Bảng research có link |
| CP5 — Quy trình trước/sau | Đỗ Hồng Vỹ | Nguyễn Ánh Dương | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Đỗ Hồng Vỹ | Đinh Hoàng Phong | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Đinh Hoàng Phong | Nguyễn Ánh Dương | Ma trận, tiêu chí đánh giá, Problem Statement v1 |
| CP6 — Quyết định | Đinh Hoàng Phong | Nguyễn Việt Hoàng | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### DinhHoangPhong-2A202604090

**Phần việc phụ trách:**

- Nhóm trưởng, giữ repo nhóm.
- Đề xuất: chính CP3, CP6 (mức can thiệp + Problem Statement v1, quyết định); hỗ trợ Problem Statement v0.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- CP1–CP2: scan 5 problem và viết 3 Problem Card. Các card là candidate #1–#3 trong bảng pitch của báo cáo nhóm; card FAP (#1) vào shortlist.
- Phần nhóm: được giao rà soát và chốt mục 2, 6, 7, 8 của báo cáo nhóm; trạng thái: chưa xác nhận hoàn thành.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/individual/2A202604090_DinhHoangPhong.md`; commit `676116d`, `6d0a42d`.
- `group_report.md` mục 2.1, 2.4.

**Điều mình học được từ phần nhóm:**

- Có số liệu rõ chưa đủ để chọn một problem; impact thấp thì vẫn nên loại, như card FAP.
- Phải tách phần mình tác động được với phần phụ thuộc người khác, như thời gian chờ trường duyệt.
- Hướng dẫn hoặc mẫu đơn rõ có thể đủ, nên cần xét No AI trước.

### DoHongVy-2A202604107

**Phần việc phụ trách:**

- Đề xuất: chính CP5 (quy trình trước/sau, Problem Statement v0); hỗ trợ CP3, research.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- CP1–CP2: scan 10 problem và viết 3 Problem Card. Các card là candidate #4–#6 trong bảng pitch; card #4 là một trong hai nguồn của candidate được chọn, và quy trình của card được dùng làm nền cho mục 4 báo cáo nhóm.
- Phần nhóm: dùng Claude Code tổng hợp bản nháp `group_report.md`, `TEAM.md` và sơ đồ quy trình từ các báo cáo cá nhân; nhóm chưa rà soát.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/individual/2A202604107_DoHongVy.md`; commit `0797d67`, `2383b53`.
- `group_report.md` mục 2.1, 2.4, 4.1, 5.
- `report/assets/cp5-workflow-current.png`, `report/assets/cp5-workflow-future.png`.

**Điều mình học được từ phần nhóm:**

- Nghẽn gốc khác với triệu chứng: tìm tin nhắn chậm chỉ là hệ quả, nguyên nhân gốc là lớp không có nơi chốt thông tin mới nhất.
- Nên thử phương án đơn giản như bảng chung trước, chỉ thêm AI khi có bằng chứng phương án đó không đủ.
- Nhiều thành viên cùng gặp một vấn đề vẫn chưa đủ làm bằng chứng; cần bấm giờ và hỏi người ngoài nhóm.
- AI giúp tổng hợp nhanh nhưng không thay được phỏng vấn, và phần nhóm vẫn phải tự rà soát, chốt.

### NguyenVietHoang-2A202604104

**Phần việc phụ trách:**

- Đề xuất: chính CP4 research; hỗ trợ kiểm chứng và quyết định.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- CP1–CP2: scan 5 problem và viết 3 Problem Card. Các card là candidate #7–#9 trong bảng pitch; card email (#8) tạo thành Opportunity D trong cây OST.
- Phần nhóm: được giao tự mở và kiểm tra 4 nguồn ở mục 3.3 của báo cáo nhóm; trạng thái: chưa xác nhận hoàn thành.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/individual/2A202604104_NguyenVietHoang.md`; file chưa được commit lên repo.
- `group_report.md` mục 2.1, 2.2, 2.3.

**Điều mình học được từ phần nhóm:**

- Phải đo được bước nghẽn thì mới nói chắc được vấn đề nằm ở đâu.
- Nhiều công cụ có sẵn đã giải một phần, nên cần tìm hiểu trước khi nghĩ đến tự xây.
- Bộ lọc, nhãn và nhắc việc có sẵn có thể đã đủ trước khi nghĩ đến AI.

### NguyenAnhDuong-2A202604087

**Phần việc phụ trách:**

- Đề xuất: chính CP4 kiểm chứng; hỗ trợ quy trình và Problem Statement v1.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- CP1–CP2: scan 8 problem và viết 3 Problem Card. Các card là candidate #10–#12 trong bảng pitch; card #11 là một trong hai nguồn của candidate được chọn, và card phòng trọ (#10) vào shortlist.
- Phần nhóm: được giao phỏng vấn 2–3 bạn ngoài nhóm và ghi snapshot cho mục 3.2 của báo cáo nhóm; trạng thái: chưa thực hiện.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/individual/2A202604087_NguyenAnhDuong.md`; commit `ef12f35`.
- `group_report.md` mục 2.1, 2.4, 4.1, 7.

**Điều mình học được từ phần nhóm:**

- Hai người độc lập gặp cùng problem là tín hiệu đáng đào sâu, nhưng vẫn cần kiểm chứng với người ngoài nhóm.
- Vấn đề của lớp trưởng cũng là một phần của bài toán, không chỉ của sinh viên.
- Một problem đau nhưng theo mùa, như tìm phòng trọ, sẽ khó đo trong thời gian ngắn.
