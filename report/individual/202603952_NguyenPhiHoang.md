# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Phi Hoàng
- MSSV: 2A202603952
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Titanic
- Link repo nhóm: https://github.com/phihoang1709/K5-L3B-DAY02-Titanic-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Cần đọc, tổng hợp nhiều thông tin |Mỗi 7h hằng ngày tôi muốn tổng hợp các tin tức mới nhất về công nghệ để bắt kịp xu hướng |Bản thân | 1-2h mỗi ngày |
| 2 |Tăng hiệu suất |Khi bắt đầu chạy một dự án mới, tôi muốn xác định đúng môi trường và các thư viện cần thiết, tài liệu nội bộ để tham gia vào dự án |Dev, tester | 2h|
| 3 |Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị cho kỳ thi cuối kỳ để có thể ôn tập nằm ở nhiều tài liệu, tôi muốn xác định đầy đủ các mục phải ôn tập, các bài tập điều kiện để không bỏ sót nội dung, bị trừ điểm hoặc bị cấm thi. |Học sinh, sinh viên | 1 tuần |
| 4 |Sự tập trung |Khi học buổi tối thường dễ mất tập trung hơn sau 20p, tôi muốn tập trung hơn dể đạt kết quả tốt |Học sinh, sinh viên | Mỗi tối |
| 5 |Lặp lại, tốn thời gian| Khi công ty có thêm nhân sự mới, cần tạo tài nguyên(tài khoản, vé xe ...), hướng dẫn với các tài liệu dự án công ty, nội quy để có thể bắt nhịp với công việc  | Nhân viên mới| 1 tuần |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- AI gợi ý về việc chạy dự án python cá nhân với các thư viện phù hợp, tôi muốn 1 ý tưởng bao quát hơn cho nhiều dự án khác nhau thay vì 1 dự án python đơn lẻ

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

> Ba card phát triển từ CP1 #5, #2 và #1. Thời gian hiện tại và phân bổ từng bước là ước lượng. Các mục tiêu bên dưới dùng để đánh giá phương án khi thử nghiệm.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Onboarding nhân viên mới (#5) | Có nhiều bên bàn giao; liên quan tài khoản, tài liệu và người hướng dẫn; phù hợp hướng muốn đào sâu | 1 tuần gồm bao nhiêu thời gian chờ, tìm tài liệu và học việc bình thường? Với mỗi 1 vị trí sẽ cần thời gian tìm hiểu cũng như vai trò khác nhau |
| 2 | Thiết lập dự án cho dev/tester (#2) | Có đầu ra kiểm tra được: chạy ứng dụng hoặc bộ test| Nghẽn ở tài liệu, phiên bản thư viện hay quyền truy cập? Liệu việc cập nhật mã nguồn và tài liệu có phù hợp ? |
| 3 | Tổng hợp tin công nghệ mỗi sáng (#1) | Lặp lại hằng ngày | Cần cập nhật chủ đề nào, và tin nào thực sự giúp công việc? Và cần đi sâu vào những thông tin nào ? Tránh cập nhật các thông tin không có ý nghĩa |

Không chọn #3 ôn thi và #4 tập trung buổi tối vào top 3 vì bối cảnh còn rộng, chưa tách được bước nghẽn và cách đo kết quả. Đây là lựa chọn cá nhân để chuẩn bị pitch, chưa phải kết luận CP3 của nhóm.

### Problem Card #1 — Onboarding nhân viên mới

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu tuần làm việc đầu tiên ở công ty, tôi muốn nắm rõ thủ tục cần hoàn thành, quyền lợi và nội quy, tài nguyên được cấp cùng tài liệu và đầu mối hỗ trợ phù hợp với vai trò, để bắt đầu nhiệm vụ đầu tiên mà không phải hỏi vòng qua nhiều người. |
| Actor | Nhân viên mới thuộc các vị trí dev/tester/ITBA. HR phụ trách hồ sơ và nội quy; IT/Admin phụ trách tài khoản, quyền truy cập và tài nguyên; mentor phụ trách hướng dẫn dự án và xác nhận khả năng bắt đầu nhiệm vụ. |
| Thời điểm / bối cảnh | Tuần làm việc đầu tiên, từ khi nhận hướng dẫn HR đến khi hoàn tất thủ tục cần thiết, có đủ tài nguyên và bắt đầu nhiệm vụ đầu tiên với mentor xác nhận. Phạm vi không bao gồm hiểu toàn bộ mã nguồn hoặc hoàn tất thử việc. |
| Quy trình hiện tại | 1. Nhận hướng dẫn HR · 2. Xác định thủ tục, tài khoản và tài nguyên · 3. Gửi hồ sơ/yêu cầu tới đầu mối · 4. Chờ duyệt và nhận tài nguyên · 5. Tìm tài liệu phù hợp với vai trò và phiên bản dự án · 6. Đọc nội quy, hướng dẫn và hỏi lại điểm chưa rõ · 7. Tìm hiểu phần dự án liên quan, bắt đầu nhiệm vụ đầu tiên và được mentor xác nhận. |
| Bottleneck | Bước 5: tìm và đối chiếu tài liệu đúng vai trò/phiên bản, ước lượng khoảng 60 phút. Việc phải xác định lại người phụ trách làm tăng số lượt hỏi. Thời gian chờ cấp quyền tại bước 4 được theo dõi riêng vì có thể chặn việc truy cập tài liệu hoặc dự án. |
| Impact |  Nhân viên mới phải dành thời gian tìm tài liệu và hỏi nhiều đầu mối trước khi bắt đầu công việc; HR/IT/Admin/mentor phải giải thích lại nội dung onboarding. Khoảng 3 ngày tìm hiểu dự án được tách khỏi thời gian xử lý thủ tục và tra cứu, vì đây còn là thời gian học nghiệp vụ cần thiết. Các mốc thời gian hiện là ước lượng cá nhân. |
| Success metric | Mục tiêu hoàn tất phạm vi onboarding trong tối đa 4 ngày làm việc, so với mức hiện tại khoảng 1 tuần ghi ở CP1. Theo dõi 3 nhân viên mới tiếp theo: ghi ngày nhận hướng dẫn, thời điểm có đủ tài nguyên và thời điểm mentor xác nhận bắt đầu nhiệm vụ đầu tiên; thống nhất đơn vị ngày làm việc khi đối chiếu baseline. Ghi thêm phút tìm tài liệu, thời gian chờ cấp quyền và số lượt chuyển đầu mối. Chỉ tính đạt khi hoàn tất thủ tục bắt buộc và bắt đầu đúng nhiệm vụ, không cắt giảm phần hướng dẫn cần thiết để đạt thời gian. |
| Phương án không dùng AI | Checklist onboarding theo vai trò; một trang tập trung tài liệu và danh bạ hỗ trợ; mỗi tài liệu có người phụ trách và ngày cập nhật. Yêu cầu cấp tài nguyên dùng biểu mẫu có trạng thái, người xử lý và hạn hoàn thành. Rule tạo đầu việc, nhắc hạn và chuyển yêu cầu theo vai trò; người có thẩm quyền phê duyệt quyền truy cập. |
| Hướng ứng dụng AI | Agent dựa vào vai trò của nhân viên và tiến độ onboarding để chọn việc cần làm tiếp theo. Nếu nhân viên báo chưa mở được tài liệu dự án, Agent kiểm tra trạng thái yêu cầu cấp quyền. Nếu yêu cầu đang chờ, Agent báo đầu mối xử lý và hướng dẫn một việc khác có thể làm ngay. Nếu chưa có yêu cầu, Agent soạn phiếu để admin duyệt trước khi cấp quyền. Khi quyền đã sẵn sàng, Agent tra tài liệu được phép đọc, dẫn nguồn đúng phiên bản và hướng dẫn nhân viên tiếp tục. |
| Cảm nhận nhanh | **Agent.** Cùng một vướng mắc có thể cần tra tài liệu, kiểm tra phiếu hoặc hỏi mentor. Agent tự chọn công cụ và điều chỉnh bước tiếp theo theo kết quả vừa nhận. Khi các nguồn mâu thuẫn, Agent chuyển câu hỏi cho người phụ trách. Mentor xác nhận nhân viên đã bắt đầu nhiệm vụ đầu tiên. |

Quy trình hiện tại — thời gian ước lượng cá nhân:

```text
[1 Nhận hướng dẫn HR: 35 phút]
→ [2 Xác định thủ tục/tài khoản/tài nguyên: 30 phút]
→ [3 Gửi hồ sơ và yêu cầu tới đầu mối: 45 phút]
→ [4 Chờ duyệt, nhận tài nguyên: ghi theo mốc gửi và hoàn tất thực tế]
→ [5 Tìm tài liệu đúng vai trò/phiên bản: 60 phút] ← BOTTLENECK TRA CỨU
→ [6 Đọc hướng dẫn/nội quy, hỏi mentor: 40 phút]
→ [7 Tìm hiểu phần dự án, bắt đầu nhiệm vụ và mentor xác nhận: khoảng 3 ngày]
```

Tổng thời gian chủ động ước lượng ở bước 1–3 và 5–6 là 210 phút. Thời gian chờ cấp quyền và tìm hiểu dự án được ghi riêng. Do các việc có thể diễn ra song song, thời gian toàn trình được tính từ lúc nhận hướng dẫn đến lúc mentor xác nhận bắt đầu nhiệm vụ đầu tiên, không cộng cơ học các khoảng thời gian trên.

**Câu hỏi phản biện khi pitch:** Trong khoảng 1 tuần onboarding, bước nào thực sự chặn nhiệm vụ đầu tiên, và phần nào có thể giảm bằng checklist, tài liệu tập trung hoặc phân công đầu mối rõ ràng?

### Problem Card #2 — Thiết lập môi trường dự án

| Trường | Nội dung |
|---|---|
| Job Story | Khi mới tham gia hoặc chuyển sang một dự án, tôi muốn xác định đúng phiên bản công cụ, thư viện, cấu hình và hướng dẫn tương ứng với mã nguồn hiện tại, để chạy được ứng dụng hoặc bộ test và bắt đầu nhiệm vụ được giao. |
| Actor | Dev/tester lần đầu thiết lập dự án; mentor hoặc người duy trì dự án hỗ trợ khi hướng dẫn không đủ. |
| Thời điểm / bối cảnh | Sau khi có quyền truy cập mã nguồn và tài nguyên cần thiết, trước lần chạy thành công đầu tiên. Giới hạn ở một dự án và hệ điều hành được dự án hỗ trợ. |
| Quy trình hiện tại | 1. Lấy đúng nhánh mã nguồn · 2. Đọc tài liệu và yêu cầu phiên bản · 3. Cấu hình công cụ/môi trường · 4. Cài thư viện và dịch vụ phụ thuộc · 5. Tra lỗi, hỏi mentor và chạy lại · 6. Kiểm tra ứng dụng hoặc bộ test tối thiểu. |
| Bottleneck | Bước 5: tìm nguyên nhân lỗi khi phiên bản công cụ, tài liệu và mã nguồn không khớp. Thời gian phân bổ ước lượng khoảng 40 phút trong tổng 120 phút. Cần phân biệt lỗi setup với lỗi có sẵn của dự án. |
| Impact | CP1 ghi khoảng 2 giờ/lần. Chậm bắt đầu nhiệm vụ và có thể khiến mentor hướng dẫn lặp lại. Chưa đo số lượt hỏi, thời gian mentor hỗ trợ hoặc số người cùng gặp. |
| Success metric | Mức hiện tại tự ghi ở CP1 khoảng 120 phút/lần; mục tiêu giảm xuống ≤60 phút tới lần chạy thành công. Theo dõi 3 lượt setup tiếp theo: ghi mốc đầu/cuối, thời gian từng bước và thời gian chờ hỗ trợ riêng. Chỉ tính thành công khi ứng dụng khởi động và hoàn thành smoke test/bộ test tối thiểu do người duy trì xác định; không bỏ kiểm tra để giảm thời gian. |
| Phương án không dùng AI | README cập nhật cùng mã nguồn; ghi rõ phiên bản và hệ điều hành hỗ trợ; khóa dependency; cung cấp cấu hình mẫu không chứa bí mật và script setup/kiểm tra môi trường. Kiểm thử hướng dẫn trên môi trường sạch khi đổi dependency. Dev/tester gửi log đã lọc thông tin nhạy cảm cho người duy trì khi script báo lỗi ngoài danh mục. Người duy trì xác định nguyên nhân và cập nhật hướng dẫn theo phiên bản. |
| Hướng ứng dụng AI | Không sử dụng AI trong phương án Rule đã chọn. |
| Cảm nhận nhanh | **Rule.** Script đối chiếu phiên bản công cụ và thư viện với cấu hình của dự án, báo mục cần sửa rồi chạy bộ test tối thiểu. Kết quả đạt hoặc lỗi có thể kiểm tra trực tiếp. |

Quy trình hiện tại — thời gian phân bổ ước lượng, chưa đo từng bước:

```text
THỜI GIAN ƯỚC LƯỢNG: 120 PHÚT
[1 Lấy đúng nhánh mã nguồn: 10 phút]
→ [2 Đọc tài liệu/yêu cầu phiên bản: 20 phút]
→ [3 Cấu hình công cụ/môi trường: 20 phút]
→ [4 Cài thư viện/dịch vụ phụ thuộc: 20 phút]
→ [5 Tra lỗi, hỏi mentor và chạy lại: 40 phút] ← BOTTLENECK
→ [6 Chạy ứng dụng và kiểm tra tối thiểu: 10 phút]

Đầu ra: dự án chạy đúng tiêu chí người duy trì xác định.
Thời gian chờ hỗ trợ cần ghi riêng, chưa có dữ liệu thực tế.
```

**Câu hỏi phản biện khi pitch:** Nếu tài liệu luôn khớp mã nguồn và đã có script setup, phần nào trong 2 giờ vẫn còn? Lỗi do thiếu hướng dẫn, dịch vụ phụ thuộc hay bản thân mã nguồn?

**Phân biệt với card #1:** Card #1 xét onboarding và bàn giao HR–IT–mentor; card #2 chỉ xét setup kỹ thuật sau khi có quyền truy cập, áp dụng cả với nhân viên cũ chuyển dự án. Không cộng impact hai card nếu cùng một lượt onboarding.

### Problem Card #3 — Tổng hợp tin công nghệ buổi sáng

| Trường | Nội dung |
|---|---|
| Job Story | Khi cập nhật tin công nghệ lúc 7 giờ mỗi ngày, tôi muốn chọn được các thay đổi đáng tin và liên quan tới chủ đề đang học hoặc dự án đang làm, để biết nội dung cần tìm hiểu sâu mà vẫn dành đủ thời gian cho công việc chính. |
| Actor | Bản thân người viết báo cáo, cập nhật công nghệ phục vụ học tập và công việc. |
| Thời điểm / bối cảnh | Lúc 7 giờ mỗi sáng, trước công việc chính; cập nhật từ nhiều nguồn để phục vụ việc học và dự án đang làm. |
| Quy trình hiện tại | 1. Mở nguồn tin · 2. Lướt tiêu đề và chọn bài · 3. Đọc để xác định mức liên quan · 4. Đối chiếu nguồn gốc, thời điểm và tin trùng · 5. Ghi điểm chính và nội dung cần đọc sâu. |
| Bottleneck | Bước 3: phải đọc nhiều bài trước khi biết có giúp việc đang làm không, dễ tiếp tục theo các bài liên quan. Thời gian phân bổ ước lượng khoảng 40 phút trong một buổi 90 phút; phần đọc tin ít liên quan được theo dõi riêng. |
| Impact | CP1 ghi 1–2 giờ/ngày. Có thể lấn thời gian học/làm và mất công đọc lại tin trùng. Chưa có số liệu chứng minh số nhiệm vụ bị chậm hoặc tỷ lệ nội dung không liên quan. |
| Success metric | Mức hiện tại tự ghi ở CP1 là 60–120 phút/ngày; mục tiêu giảm xuống ≤30 phút/buổi, theo dõi 5 buổi. Mỗi buổi lưu thời gian, chủ đề, tin giữ lại và lý do liên quan. Mọi tin giữ lại phải có link gốc, ngày công bố và một câu giải thích ý nghĩa với công việc/học tập. Cuối buổi rà tiêu đề trong cùng tập nguồn, ghi tin quan trọng bị bỏ sót để kiểm soát chất lượng; không đo thành công bằng số bài đọc. |
| Phương án không dùng AI | Giới hạn tối đa 3 chủ đề theo mục tiêu học/dự án, chọn nguồn ưu tiên, dùng RSS/bản tin định kỳ, lọc từ khóa/tin trùng và đặt khung 30 phút. Tách cập nhật nhanh khỏi nghiên cứu sâu; bài cần đào sâu được lưu thành nhiệm vụ riêng có lý do. Giữ bài có nguồn gốc rõ ràng và ghi một câu giải thích thay đổi đó ảnh hưởng thế nào đến việc đang làm. Các bài cùng đưa một tin được gom về nguồn gốc để tránh đọc lặp. |
| Hướng ứng dụng AI | Không sử dụng AI. Người đọc tự chọn và đối chiếu tin với nguồn gốc. |
| Cảm nhận nhanh | **No AI.** Mỗi sáng chọn tối đa ba chủ đề, đọc các nguồn ưu tiên trong 30 phút và lưu bài cần nghiên cứu riêng. Sau năm buổi, đối chiếu thời gian đọc và số tin liên quan bị bỏ sót. |

Quy trình hiện tại — thời gian phân bổ ước lượng, chưa đo từng bước:

```text
THỜI GIAN PHÂN BỔ ƯỚC LƯỢNG: 90 PHÚT/BUỔI
[1 Mở các nguồn thường đọc: 5 phút]
→ [2 Lướt tiêu đề, chọn bài: 20 phút]
→ [3 Đọc và xác định mức liên quan: 40 phút] ← BOTTLENECK
→ [4 Đối chiếu nguồn, ngày và tin trùng: 15 phút]
→ [5 Ghi điểm chính/nội dung cần đọc sâu: 10 phút]

Đầu ra: danh sách tin liên quan có nguồn và lý do cần quan tâm.
Nghiên cứu sâu sau buổi cập nhật được ghi thời gian riêng.
```

**Câu hỏi phản biện khi pitch:** Tôi đọc lâu vì nguồn phân tán hay vì chưa xác định mục tiêu và giới hạn thời gian? Nếu chọn nguồn/chủ đề đã giảm còn 30 phút thì chưa có căn cứ thêm AI.

### Card muốn pitch nhất

- Card số: **1 — Onboarding nhân viên mới**.
- Vì sao: phù hợp hướng đào sâu; có thể khảo sát cả nhân viên mới và bên hỗ trợ; có phương án cải thiện quy trình đơn giản để so sánh.
- Câu hỏi muốn nhóm phản biện: “Trong khoảng 1 tuần onboarding, phần chậm nhất là chờ cấp quyền, tìm đúng tài liệu hay học nghiệp vụ; dữ liệu nào giúp phân biệt ba nguyên nhân này?”

### AI đã phản biện card thế nào


| Điểm yếu AI chỉ ra | Đồng ý? | Thay đổi trong bản nháp sau phản biện |
|---|----|---|
| “Onboarding mất 1 tuần” chưa xác định thế nào là hoàn tất | Đồng ý | Đề xuất mốc có đủ điều kiện và bắt đầu nhiệm vụ đầu tiên; tách thời gian theo lịch và làm chủ động. |
| Đang gom cấp tài khoản, vé xe và học dự án thành một bottleneck | Đồng ý | Tách bước chờ cấp quyền và tìm tài liệu; đo riêng từng bước ở CP4 để xác định bước nào chặn nhiệm vụ đầu tiên. |
| Có thể chỉ thiếu checklist, không cần AI | Đồng ý | Bổ sung phương án trang bắt đầu, owner tài liệu và phân công hỗ trợ trước khi thử AI. |
| Thời gian từng bước chưa có nguồn đo | Đồng ý | Đánh dấu toàn bộ số phân bổ là minh họa; không dùng làm bằng chứng CP4. |

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
| CP2 Problem Card | Hỗ trợ phát triển 3 card từ CP1 và phản biện onboarding | Tách phạm vi, metric và giả thuyết nghẽn | Phân bổ thời gian từng bước chưa có dữ liệu thật | Chờ tôi đối chiếu quy trình, sửa số và tự đánh giá phản biện |
| CP4 Research | Tìm tài liệu chính thức và chuẩn bị kế hoạch kiểm chứng onboarding | So sánh checklist, wiki và quản trị tri thức | Tài liệu sản phẩm không chứng minh pain tại công ty | Chờ tôi kiểm link, phỏng vấn người thật và cập nhật kết luận |
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
