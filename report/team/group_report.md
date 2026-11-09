# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

> **Trạng thái: bản chuẩn bị theo hướng onboarding do Nguyễn Phi Hoàng đề xuất; chưa có kết quả phỏng vấn/survey và chưa ghi nhận đồng thuận CP3.** Research bên dưới đã mở nguồn chính thức ngày 09/11/2026. Không xem tính năng của công cụ là bằng chứng rằng nhân viên công ty đang gặp pain này.

### Phạm vi kiểm chứng đề xuất

Xuất phát từ CP1 #5: nhân viên mới cần tài khoản/tài nguyên, tài liệu dự án và nội quy để bắt đầu làm việc; người viết ghi khoảng 1 tuần. CP1 #2 (thiết lập dự án 2 giờ) là nhánh kỹ thuật liên quan, không cộng hai số để tính tổng impact.

Candidate để kiểm chứng: **Khi bắt đầu tuần làm việc đầu tiên, nhân viên mới muốn biết việc cần hoàn thành, tài liệu phù hợp và người hỗ trợ đúng, để có đủ điều kiện bắt đầu nhiệm vụ đầu tiên.**

Giới hạn khảo sát ban đầu đề xuất: dev/tester mới vào công ty. Ghi nhận HR, IT và buddy là bên bàn giao. Không bao gồm toàn bộ tuyển dụng, thử việc hay đánh giá năng lực. Nếu người được hỏi thuộc vai trò khác, ghi rõ để không trộn các quy trình khác nhau.

### 3.1. Assumption Map

Điểm quan trọng là đề xuất phân tích; điểm bằng chứng 1 = chưa có kiểm chứng trực tiếp. CP1 là tự ghi nhận của một người, chưa phải mẫu phỏng vấn.

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| A1 | Nhiều người mới trong phạm vi khảo sát bị chậm nhiệm vụ đầu tiên do vướng onboarding, không chỉ một trải nghiệm cá nhân | Value | 5 | 1 | Có — hỏi 2 người mới ngoài nhóm |
| A2 | Tìm đúng tài liệu và đúng người hỗ trợ là phần mất thời gian đáng kể hơn chờ cấp quyền hoặc học nghiệp vụ | Value | 5 | 1 | Có — phân rã lần gần nhất theo bước |
| A3 | Tài liệu cần thiết thực sự tồn tại, còn đúng và có người chịu trách nhiệm cập nhật | Feasibility | 5 | 1 | Có — nhờ đầu mối kiểm mẫu tài liệu được phép xem |
| A4 | Người mới có thể tự hoàn thành phần lớn việc với checklist theo vai trò và danh bạ hỗ trợ | Usability | 4 | 1 | Có — cho thực hiện một việc cụ thể trên hướng dẫn hiện có |
| A5 | Công ty cho phép sử dụng công cụ lưu/tìm tài liệu với quyền truy cập phù hợp | Viability | 5 | 1 | Hỏi HR/IT trước khi thử công cụ; không tự đưa dữ liệu nội bộ ra ngoài |
| A6 | HR/IT/buddy có thể duy trì danh sách đầu việc, trạng thái và owner qua các đợt tuyển mới | Viability | 4 | 1 | Hỏi người phụ trách về lần cập nhật và bàn giao gần nhất |

Ưu tiên A1–A3 để xác định pain và nguyên nhân. A5 là điều kiện trước khi thử giải pháp có dữ liệu nội bộ. Không mặc định tìm kiếm tài liệu là bottleneck chỉ vì muốn dùng công cụ hỏi đáp.

### 3.2. Kiểm chứng

**Cách đã dùng:** Chưa phỏng vấn/survey. Đã research tài liệu công khai, chưa kiểm chứng pain tại công ty.

**Kế hoạch:** phỏng vấn 2 nhân viên đã onboarding gần đây và 1 HR/IT/buddy từng hỗ trợ, tất cả ngoài nhóm làm bài và có trải nghiệm thật. Ghi ngày, kênh hỏi và vai trò; không ghi danh tính hoặc thông tin nội bộ vào repo.

Câu hỏi cho nhân viên mới (hỏi một lần onboarding cụ thể):

1. Lần gần nhất bạn vào công ty hoặc được onboarding là khi nào, với vai trò gì? Bạn bắt đầu nhận hướng dẫn từ đâu?
2. Kể lại từng bước từ ngày đầu đến lúc bạn bắt đầu nhiệm vụ đầu tiên. Thế nào được xem là đủ điều kiện bắt đầu?
3. Lần gần nhất bạn cần một tài khoản hoặc quyền truy cập, bạn hỏi ai, gửi qua đâu và được xử lý khi nào? Trong lúc chờ bạn có làm được việc khác không?
4. Lần gần nhất cần tìm nội quy hoặc tài liệu dự án, bạn đã tìm ở đâu, mất bao lâu và biết đó là bản đúng bằng cách nào?
5. Có việc nào bạn phải hỏi lại hoặc chuyển qua người khác không? Kể lại việc đó và số lượt chuyển.
6. Việc nào thực sự chặn nhiệm vụ đầu tiên? Việc nào vẫn hoàn thành nhanh nhờ hướng dẫn hiện có?
7. Bạn đã tự tạo ghi chú/checklist hay nhờ ai hỗ trợ thế nào? Nếu được phép, có thể cho xem một ví dụ đã che thông tin nhạy cảm không?

Câu hỏi cho HR/IT/buddy:

1. Ở đợt nhân viên mới gần nhất, các đầu việc được phân công, theo dõi và xác nhận hoàn tất thế nào?
2. Yêu cầu nào bị chậm hoặc phải hỏi lại? Mốc gửi, nhận, xử lý là khi nào? Nguyên nhân cụ thể là gì?
3. Lần gần nhất tài liệu onboarding được cập nhật là khi nào, ai sửa và ai xác nhận?
4. Có trường hợp người mới tự hoàn thành nhanh không? Họ đã dùng hướng dẫn nào?
5. Với công cụ đang có, ai được xem tài liệu nào và ai duyệt quyền? Trước đây có hạn chế nào khiến một cách làm không dùng được?

#### Interview Snapshot — điền sau mỗi cuộc phỏng vấn

Copy bảng này cho từng người; trích nguyên văn chỉ khi thực sự ghi được.

| Trường | Nội dung |
|---|---|
| Mã mẫu / vai trò | PV01 / __ |
| Ngày và kênh hỏi | __ |
| Thời điểm onboarding được kể lại | __ |
| Câu nói đáng nhớ nhất (nguyên văn) | __ |
| Lần gần nhất: chuyện gì đã xảy ra? | __ |
| Các bước và thời gian từng bước | __ |
| Workaround hiện tại | __ |
| Thời gian chờ / thời gian chủ động / số lượt chuyển đầu mối | __ / __ / __ |
| Điều gì chặn nhiệm vụ đầu tiên? | __ |
| Tín hiệu xác nhận / phản bác | __ / __ |
| Nguồn đối chiếu được phép sử dụng | __ |
| Insight rút ra | __ |

#### Nhật ký đo một lượt onboarding

| Bước | Đầu mối | Mốc gửi/bắt đầu | Mốc nhận/kết thúc | Phút làm chủ động | Phút chờ | Có chặn việc đầu tiên? | Nguồn |
|---|---|---|---|---:|---:|---|---|
| Nhận hướng dẫn và xác định đầu việc | HR/người mới | __ | __ | __ | __ | __ | __ |
| Yêu cầu và nhận tài khoản/tài nguyên | IT/HR/người duyệt | __ | __ | __ | __ | __ | __ |
| Tìm tài liệu đúng vai trò, đúng phiên bản | Người mới/buddy | __ | __ | __ | __ | __ | __ |
| Đọc, hỏi lại và xác nhận hoàn tất | Người mới/buddy | __ | __ | __ | __ | __ | __ |

Đo thời gian theo lịch từ mốc bắt đầu tới mốc kết thúc; không cộng các khoảng chờ chồng nhau. Nếu số liệu chỉ từ trí nhớ, ghi rõ “ước lượng hồi tưởng”. Với 2–3 người, báo từng trường hợp, không suy rộng thành tỷ lệ của toàn công ty.

#### Tổng hợp bằng chứng

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| CP1 của người viết | 1 ghi nhận, chưa đối chiếu | Ghi onboarding khoảng 1 tuần | Chưa biết 1 tuần là chậm bất thường hay thời lượng học việc dự kiến |
| Phỏng vấn nhân viên mới | 0 — chưa thực hiện | Chưa có | Chưa có |
| Phỏng vấn HR/IT/buddy | 0 — chưa thực hiện | Chưa có | Chưa có |

**Cách đọc kết quả sau phỏng vấn — quy tắc đề xuất:**

- Nếu chờ cấp quyền chặn công việc lâu nhất: thu hẹp vào bàn giao yêu cầu, người duyệt và trạng thái xử lý; kiểm tra checklist/Rule trước.
- Nếu tài liệu thiếu, cũ hoặc không có owner: ưu tiên sửa và giao trách nhiệm nội dung; chưa đủ cơ sở làm hỏi đáp tự động.
- Nếu tài liệu đúng đã có nhưng người mới vẫn khó tìm/hiểu: tiếp tục khảo sát tra cứu theo vai trò, so sánh wiki và hỗ trợ trả lời có nguồn.
- Nếu checklist hiện tại đã đủ và không chặn công việc: ghi tín hiệu phản bác; cân nhắc đổi phạm vi hoặc candidate.

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Chưa có kết quả để ghi. Bản nháp hiện chỉ tách “onboarding 1 tuần” thành các nguyên nhân cần kiểm tra; đây là điều chỉnh sau phân tích, không phải insight phỏng vấn.

### 3.3. Research giải pháp đã có

Nguồn chính thức đã mở ngày 09/11/2026. Tính năng dưới đây theo tài liệu nhà cung cấp; cột hạn chế và bài học là suy luận áp dụng cho candidate, chưa phải thử nghiệm tại công ty. Chưa đánh giá giá/gói, tích hợp hay mức giảm thời gian.

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh theo nguồn | Khoảng trống / rủi ro khi áp dụng (phân tích) | Bài học cho nhóm |
|---|---|---|---|---|---|
| Confluence — mẫu kế hoạch 90 ngày | [Atlassian HR templates](https://www.atlassian.com/software/confluence/templates/collections/hr) | Nhận hướng dẫn, xác định tài nguyên/đầu mối và mốc cần hoàn thành | Mẫu hướng người mới tới người liên quan, tài nguyên, mục tiêu và cột mốc | Một mẫu hướng dẫn chưa chứng minh đã xử lý được phê duyệt tài khoản hoặc nội dung cũ; cần người điền và duy trì | Thử checklist và trang bắt đầu trước; phạm vi pilot chỉ lấy các đầu việc tuần đầu |
| Notion — wiki, owner và xác minh trang | [Wikis & verified pages](https://www.notion.com/help/wikis-and-verified-pages) | Tìm tài liệu và xác định nội dung được ai phụ trách | Wiki tập trung trang; có owner, trạng thái xác minh và thông báo khi xác minh hết hạn | Dấu xác minh không thay thế việc chuyên gia kiểm nội dung; trang ngoài wiki và database có điều kiện Business/Enterprise theo tài liệu | Mỗi tài liệu onboarding cần owner và lịch rà soát, không chỉ một thư mục chứa link |
| Guru — quản trị xác minh tri thức | [How Content is Verified in Guru](https://help.getguru.com/docs/verifying-and-unverifying-cards) | Kiểm độ tin cậy tài liệu trước khi người mới tra cứu | Card có verifier, thời điểm xác minh và chu kỳ rà soát; có cơ chế tự động kiểm chất lượng | Tài liệu nêu nội dung chưa xác minh vẫn có thể xuất hiện trong tìm kiếm/câu trả lời; cần xem cấu hình giới hạn nguồn, không mặc định mọi kết quả đã duyệt | Nếu thử hỏi đáp, kiểm tra nguồn, trạng thái xác minh và quy trình chuyển người phụ trách khi thiếu căn cứ |

**Điều research làm thay đổi trong hướng khảo sát:** không bắt đầu bằng “xây chatbot onboarding”. Đã có cách tổ chức đầu việc và tài liệu bằng công cụ sẵn có. Cần dùng bằng chứng CP4 để quyết định vấn đề còn lại nằm ở bàn giao, chất lượng tài liệu hay đọc hiểu. Research này chưa đủ để chốt Go/Not Yet/No-Go hoặc mức AI của CP6.

**Phần còn thiếu để hoàn tất CP4:** 2–3 cuộc phỏng vấn thật hoặc survey 5–10 người, snapshot có nguồn/thời điểm, ít nhất một tín hiệu phản bác và cập nhật candidate sau khi xem bằng chứng. Nhóm tự kiểm lại các link trước khi nộp.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
