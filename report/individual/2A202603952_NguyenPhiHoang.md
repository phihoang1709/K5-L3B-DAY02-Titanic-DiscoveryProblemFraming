# Báo cáo cá nhân — 2A202603952_NguyenPhiHoang

> Báo cáo của Nguyễn Phi Hoàng, nhóm Titanic. Hướng dẫn: [worksheet](../../docs/01-worksheet.md). Các phần biên soạn bổ sung và bản nháp reflection có hỗ trợ AI được ghi ở mục 4–6.

## 1. Thông tin học viên

- Họ tên: Nguyễn Phi Hoàng
- MSSV: 2A202603952
- Email trường: không công khai trong repo.
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
| Cảm nhận nhanh | **Agent — nhận định ban đầu ở CP2.** Cùng một vướng mắc có thể cần tra tài liệu, kiểm tra phiếu hoặc hỏi mentor. Agent tự chọn công cụ và điều chỉnh bước tiếp theo theo kết quả vừa nhận. Khi các nguồn mâu thuẫn, Agent chuyển câu hỏi cho người phụ trách. Mentor xác nhận nhân viên đã bắt đầu nhiệm vụ đầu tiên. |

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

Phần bổ sung có AI hỗ trợ; snapshot thuộc case mô phỏng, không phải cuộc phỏng vấn tôi đã làm.

| Hoạt động | Đóng góp / kết quả |
|---|---|
| Pitch | Chuẩn bị ba card; onboarding được nhóm chọn. |
| Phản biện bạn khác | TEAM có ghi đóng góp nhưng chưa lưu câu hỏi tại lớp. Câu hỏi bổ sung cho #4: “Ghi lỗi sau mỗi buổi đã đủ chưa?” |
| Nhận phản biện | Phúc hỏi Agent hay Workflow; làm rõ Agent phải tự chọn công cụ và điều chỉnh bước theo kết quả. |
| Cluster / OST | Tổng hợp #1/#4/#12; OST tập trung tài liệu, đầu mối và tiến độ onboarding. |
| Chọn candidate | Bổ sung điểm và lý do chọn onboarding; không nhận là biên bản bỏ phiếu. |
| Kiểm chứng / research | Đối chiếu ba nguồn sản phẩm; chưa phỏng vấn thật. |
| Quy trình | Giữ bảy bước; tách 210 phút chủ động, chờ quyền và học nghiệp vụ. |
| Problem Statement | Bổ sung metric đúng nguồn/bước tiếp theo và boundary; không suy giảm ngày từ giảm phút. |
| Mức AI | Chọn Agent hỗ trợ onboarding; checklist/Rule là nền, Workflow là đối chứng. |
| Quyết định | Not Yet vì chưa kiểm chứng nhu cầu, dữ liệu/quyền và hiệu quả Agent. |

**So với CP2:** Giữ hướng Agent nhưng giới hạn quyền và số lượt gọi công cụ. Mục tiêu ≤4 ngày ban đầu chưa đủ cơ sở; nhóm đo tra cứu ≤20 phút và theo dõi toàn trình riêng.

## 5. Dùng AI

| CP | Dùng AI / hữu ích | Điểm yếu | Cách xử lý |
|---|---|---|---|
| CP1 | Gợi thêm bài setup. | Quá hẹp vào Python. | Giữ bài setup cho dev/tester. |
| CP2 | Phát triển card, phản biện. | Phân bổ phút chưa đo. | Ghi ước lượng, tách tra cứu/chờ/học. |
| CP3 | Biên soạn Cluster, OST, shortlist. | Ban đầu gom cả 12. | Chỉ #1/#4/#12, giữ nguyên pitch; không nhận AI là hoạt động phản biện tại lớp. |
| CP4 | Research và snapshot. | Nguồn sản phẩm/case không chứng minh pain thật. | Kiểm link, ghi số mẫu thật bằng 0. |
| CP5 | Sơ đồ, before/after. | Giảm phút không chứng minh giảm ngày. | Giữ 60 →20 và 210 →170, đo phần chờ riêng. |
| CP5–6 | Biên soạn v0/v1 và eval. | Dễ chỉ đo tốc độ. | Thêm đúng nguồn, quyền, bước tiếp theo và fallback. |
| CP6 | So sánh mức can thiệp. | Bản trước thu hẹp thành Workflow tra cứu. | Giữ mục tiêu hỗ trợ tiến độ: Agent tự chọn công cụ; cần so với Workflow. |
| CP7 | Soạn nháp reflection. | AI không biết trải nghiệm riêng. | Ghi rõ hỗ trợ AI; tôi cần rà và tự viết lại trải nghiệm. |

AI hỗ trợ cả biên soạn, rộng hơn giới hạn “chỉ phản biện” của lab; không coi bản nháp là phần tự làm đã được xác nhận.

## 6. Reflection (CP7)

> Bản nháp có AI hỗ trợ để Hoàng rà lại; chưa phải reflection tự viết đáp ứng quy định CP7.

**6.1. Tôi học được gì từ các problem của nhóm?**

Đọc card của nhóm, tôi thấy vấn đề có thời gian, tần suất và đầu ra rõ dễ phân tích hơn. Onboarding cần chỉ ra bước nghẽn, thay vì chỉ nói người mới mất một tuần.

**6.2. Tôi có bị solution-first không?**

Ban đầu tôi nghiêng về Agent vì có nhiều bên tham gia. Điều đó chưa đủ: phải tách việc hành chính cố định khỏi vướng mắc cần tìm hiểu và chọn bước tiếp theo theo kết quả.

**6.3. Tôi thay đổi gì sau phản biện?**

Câu hỏi của Phúc khiến tôi làm rõ lý do chọn Agent. Tôi giữ hướng này cho việc tự chọn công cụ, hỏi thêm và điều chỉnh hỗ trợ; giới hạn quyền, giữ người duyệt và xem Workflow là phương án đối chứng.

**6.4. Research giúp tôi thấy gì?**

Các công cụ có sẵn giải được phần tài liệu và yêu cầu. Phần cần đánh giá là phối hợp chúng theo tình huống. Tôi chưa phỏng vấn thật nên không coi snapshot là bằng chứng nhu cầu.

**6.5. Khó nhất khi viết Problem Statement?**

Khó nhất là metric: 60 phút tra cứu nằm trong 210 phút chủ động; chờ quyền và học dự án khác bản chất. Giảm xuống 20 phút chưa chứng minh giảm ngày onboarding, cũng chưa bảo đảm hướng dẫn đúng.

**6.6. Nếu làm lại, tôi sẽ đổi gì?**

Tôi sẽ đo baseline và hỏi người mới trước. Tôi muốn so Agent với Workflow trên cùng tình huống, kiểm cả thời gian lẫn lỗi, thay vì chỉ bảo vệ giải pháp mình thích. Not Yet nhắc tôi hoàn thành việc này.

**6.7. Chuỗi problem → quy trình → metric → boundary → mức AI → quyết định**

Người mới khó tìm đúng nguồn và biết bước tiếp theo khi onboarding gặp trở ngại. Quy trình gồm bảy bước từ hướng dẫn HR đến nhiệm vụ đầu tiên. Metric chính là giảm thời gian onborading xuống từ 30-50%, kèm đúng tài liệu và bước đề xuất. Chờ quyền và học nghiệp vụ được đo riêng. Agent tự chọn công cụ theo kết quả nhưng không tự gửi yêu cầu, cấp quyền hoặc xác nhận hoàn tất. HR/IT giữ phê duyệt, mentor kiểm tra nhiệm vụ, mỗi lượt hỗ trợ giới hạn năm lần gọi công cụ. Nhóm chọn thiết kế Agent nhưng quyết định Not Yet vì chưa đủ kiểm chứng thực tế.

## 7. Tài liệu tham khảo

- [Báo cáo nhóm](../team/group_report.md): research, quy trình, Agent và quyết định.
- [Worksheet](../../docs/01-worksheet.md), [bài mẫu](../../docs/02-deliverable-example.md), [framework](../../docs/03-international-frameworks.md).
- Ba nguồn sản phẩm chính thức tại mục 3.3 của báo cáo nhóm, kiểm tra 09/11/2026.
