# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Trần Nguyễn Thái Duy
- Mã học viên: 2A202602991
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinh viên năm 4 ngành Kỹ thuật Phần mềm / CNTT, Tech Lead nhóm đồ án môn học & Thực tập sinh Software Engineer
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
  - Quản lý repo GitHub, review Pull Request (PR) và release tính năng cho nhóm đồ án môn học 4-5 người.
  - Viết code backend/frontend, unit test và tích hợp các API bên thứ 3 (payment gateway, authentication, LLM API).
  - Thu thập tiến độ, tổng hợp task và nộp báo cáo Weekly Log cho giảng viên hướng dẫn đồ án.
  - Hỗ trợ setup môi trường phát triển (Docker, node/python venv, .env) và gỡ lỗi kỹ thuật cho các thành viên.
  - Đọc tài liệu công nghệ, viết tài liệu đặc tả (SRS/SDD) và chuẩn bị slide demo tiến độ định kỳ.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Lặp lại | Viết và tổng hợp changelog / release notes mỗi cuối tuần từ 10-15 PR rải rác trên GitHub | Tech Lead nhóm đồ án, các thành viên trong nhóm | Mất 40-50 phút/cuối tuần; 3/4 thành viên thường xuyên để trống PR description khiến lead phải tự click vào diff từng commit để tóm tắt |
| 2 | Lặp lại | Thu thập tiến độ task từ Git log/Trello của 4 thành viên để lập Weekly Log nộp giảng viên hướng dẫn | Trưởng nhóm (Duy), giảng viên hướng dẫn môn học | 1 lần/tuần vào tối Chủ Nhật, mất 45 phút nhắn tin giục 4 người update task và format lại vào Notion/Google Docs trước 23h |
| 3 | Tốn thời gian | Setup môi trường local và gỡ lỗi phụ thuộc (.env, Node/Python version mismatch, Docker port collision) cho thành viên mới | Thành viên mới tham gia nhóm, Tech Lead hỗ trợ | Mất 2-3 tiếng/người mỗi đầu kỳ hoặc khi re-setup; trung bình có 4-6 tin nhắn hỏi lỗi "chạy npm start bị văng", "docker container exited with code 1" |
| 4 | Tốn thời gian | Đọc hiểu và phân loại các endpoint trong tài liệu API bên thứ ba (VNPay, ZaloPay, OpenAI API) không có code mẫu tiếng Việt cụ thể | Developer tích hợp hệ thống trong nhóm | Mất 60-90 phút/lần tích hợp; phải mở 8-10 tab Chrome đối chiếu mã lỗi HTTP 400/422 và thử đi thử lại trên Postman 15-20 lần |
| 5 | Tốn thời gian | Bóc tách thủ công thông tin hóa đơn, ảnh chụp biên lai chuyển khoản ngân hàng (VietQR/MoMo) vào Google Sheets để quyết toán quỹ nhóm | Thủ quỹ nhóm đồ án (1 người), cả nhóm 4-5 người | 1-2 lần/tháng, mất 45-60 phút ngồi soi từng bill ảnh chuyển khoản server cloud/API token, nhập tay 25-30 dòng; từng bị lệch 45.000đ do gõ sót |
| 6 | AI có thể tốt hơn | Đọc và trích xuất action items, người phụ trách, deadline từ chuỗi 100+ tin nhắn thảo luận tự do trong kênh Discord/Zalo sau mỗi buổi họp nhóm | Cả nhóm đồ án (5 người), đặc biệt là nhóm trưởng | Mất 25-30 phút sau mỗi buổi tối chat dài; tháng trước có 2 lần thành viên bị miss task do tin nhắn giao việc bị trôi và không ghim kịp thời |
| 7 | AI có thể tốt hơn | Gợi ý và sinh danh sách các edge cases / boundary test cases cho các hàm xử lý logic nghiệp vụ phức tạp trước khi viết unit test | Backend developer, tester đồ án | Mất 35-45 phút ngồi vắt óc nghĩ kịch bản kiểm thử cho mỗi feature; từng lọt 3 bug logic vào buổi demo giữa kỳ do sót case chuỗi rỗng và vượt quá giới hạn số ký tự |
| 8 | AI có thể tốt hơn | Tóm tắt và phát hiện xung đột yêu cầu nghiệp vụ giữa tài liệu đặc tả SRS cũ và các ghi chú điều chỉnh mới từ giảng viên hướng dẫn | Người viết tài liệu (Duy), nhóm phản biện đồ án | Mất 50-70 phút/lần soát lại doc 30-40 trang; tuần trước sót 1 thay đổi về quy tắc hủy đơn hàng dẫn đến backend code lệch spec frontend |
| 9 | Pain từ người khác | Thành viên trong nhóm liên tục hỏi lại cấu trúc thư mục, quy ước nhánh Git và quy tắc đặt tên Git commit dù đã có file README/CONTRIBUTING | Tech Lead (người review PR) và các thành viên khác | Bị ngắt quãng 3-4 lần/tuần bởi câu hỏi: "commit này ghi prefix gì?", "merge vào staging hay develop?"; mất 15-20 phút/PR để yêu cầu sửa lại commit message |
| 10 | Pain từ người khác | Giảng viên/Mentor nhận xét slide thuyết trình báo cáo tiến độ quá dày chữ, thiếu tính trực quan và không làm bật được kết quả định lượng | Nhóm thuyết trình đồ án (4 người), giảng viên hướng dẫn | Nhận 2 lần góp ý gay gắt từ mentor: "Slide 6-9 toàn gạch đầu dòng, không thấy số đo cụ thể"; cả nhóm phải thức đến 1h30 sáng làm lại 12 slide (mất 2.5 tiếng) |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: `Tôi là sinh viên năm 4 ngành Kỹ thuật Phần mềm kiêm Tech Lead nhóm đồ án tốt nghiệp 5 người. Công việc hằng tuần gồm: review PR, quản lý GitHub repo, code backend/API, viết weekly report cho giảng viên, hỗ trợ thành viên fix lỗi môi trường. Hãy gợi ý thêm problem theo 4 lăng kính: lặp lại, tốn thời gian, AI có thể tốt hơn, pain từ người khác. Với mỗi gợi ý, ghi actor, workflow sơ bộ và cách đo. Đừng đưa ý tưởng quá rộng kiểu "xây trợ lý AI toàn năng".`
- Ý dùng được: Gợi ý về việc bóc tách edge cases cho unit test từ user story/hàm nghiệp vụ và trích xuất action items từ kênh chat trao đổi tự do (Discord/Zalo).
- Ý bỏ vì không phải pain thật: Ý tưởng "tự động sinh toàn bộ code từ mô tả tiếng Việt" (bỏ vì quá rộng, không thực tế cho buổi lab, khó kiểm soát chất lượng) và "tự động dịch tài liệu tiếng Anh sang tiếng Việt" (bỏ vì không phải pain thật sự do sinh viên CNTT đều đọc doc tiếng Anh bình thường).

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính (Đã dùng đủ cả 4/4 lăng kính)
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Đọc và trích xuất action items, người phụ trách, deadline từ chuỗi 100+ tin nhắn thảo luận tự do trong kênh Discord/Zalo sau mỗi buổi họp nhóm | - Actor rất rõ (Nhóm trưởng & 4 thành viên đồ án)<br>- Workflow lặp lại 1-2 lần/tuần, bottleneck rõ ở bước lội tin nhắn<br>- Impact đo được bằng số task bị sót và thời gian lội chat | Nhóm hay chat tiếng Việt không dấu, dùng từ lóng ("ông làm cái này nha", "mai tui đẩy") nên AI có thể hiểu sai ngữ cảnh cam kết |
| 2 | Gợi ý và sinh danh sách các edge cases / boundary test cases cho các hàm xử lý logic nghiệp vụ phức tạp trước khi viết unit test | - Actor rõ (Backend Dev/Tester)<br>- Bottleneck cụ thể ở bước vắt óc nghĩ kịch bản biên<br>- Giúp ngăn ngừa bug trực tiếp trước khi demo | AI có thể sinh quá nhiều test case thừa/vô nghĩa hoặc thiếu hiểu biết về business constraints sâu của hệ thống |
| 3 | Viết và tổng hợp changelog / release notes mỗi cuối tuần từ 10-15 PR rải rác trên GitHub | - Trải nghiệm thực tế mỗi tối Chủ Nhật của Tech Lead<br>- Dễ đo lường thời gian (giảm từ 45' xuống 10')<br>- Scope vừa vặn trong 1 buổi lab | Một số PR lớn có diff quá dài vượt context window của model hoặc PR description bị viết sai lệch |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Trích xuất Action Items từ tin nhắn thảo luận Discord/Zalo nhóm đồ án

```text
Problem 1 câu:
Sau mỗi buổi thảo luận không chính thức trên Discord/Zalo, nhóm trưởng mất 25-30 phút đọc lại hơn 100 tin nhắn rời rạc để nhặt ra ai làm gì, hạn chót khi nào, dẫn đến việc thường xuyên bỏ sót task và thành viên quên deadline.

Actor:
Trưởng nhóm đồ án (Thái Duy) và 4 thành viên trong nhóm công nghệ thông tin.

Thời điểm / bối cảnh:
Ngay sau các buổi họp voice/chat tối (thường vào 21h-23h thứ Ba và thứ Sáu hàng tuần) khi cả nhóm thống nhất giải pháp tính năng mới.

Current workflow 3-7 bước:
1. Nhóm trao đổi tự do bằng text/voice, các quyết định và cam kết nằm rải rác trong luồng chat 100+ tin.
2. Nhóm trưởng mở lại kênh chat, lội từng tin nhắn từ trên xuống dưới để tìm các câu thỏa thuận công việc.
3. Ghi chép nháp ra giấy/Notion danh sách task, đoán người nhận việc và deadline dựa trên nội dung chat.
4. Mở board Trello/Jira của nhóm, tạo từng thẻ công việc tương ứng.
5. Gán nhãn, chọn Assignee, set Due date và gửi 1 tin nhắn tổng hợp tóm tắt vào nhóm để mọi người xác nhận.

Bottleneck:
Bước 2 — Lội ngược và đọc thủ công hơn 100 tin nhắn không cấu trúc, dễ mỏi mắt, sót ý kiến chốt hạ ngầm hoặc hiểu nhầm người nhận task (mất 15-20 phút).

Impact:
Mất 50-60 phút/tuần cho 1 nhóm trưởng; trung bình mỗi tháng có 2-3 task bị quên hoặc làm trùng lặp do không được ghi nhận kịp thời vào Trello; gây căng thẳng trong nhóm khi gần tới ngày demo.

Success metric:
- Giảm thời gian trích xuất và tạo task từ 25 phút xuống dưới 5 phút mỗi buổi họp.
- Tỷ lệ task bị sót hoặc nhầm lẫn người phụ trách giảm về 0%.

Non-AI alternative:
Quy tắc hành vi bắt buộc: Bắt thành viên tự tạo task ngay trong lúc họp hoặc có 1 người thư ký gõ live meeting notes. (Đã thử nhưng thất bại vì ai cũng mải tranh luận kỹ thuật, không ai chịu ghi chép).

AI hypothesis:
LLM có khả năng đọc hiểu ngữ cảnh hội thoại tự nhiên tiếng Việt, lọc bỏ tin nhắn tán gẫu, trích xuất chính xác bộ thông tin cấu trúc: [Task Name, Assignee, Deadline, Context Link, Priority]. Nhóm trưởng chỉ cần copy đoạn chat vào, AI sinh danh sách task dạng bảng/JSON để duyệt trong 1 phút.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid):

```text
CURRENT STATE — 28 phút

[1 Chat tự do: 0']
→ [2 Lội 100+ tin nhắn tìm việc: 15']  <-- bottleneck (sót việc, mỏi mắt)
→ [3 Ghi nháp ra giấy/Notion: 5']
→ [4 Tạo thẻ thủ công trên Trello: 5']
→ [5 Nhắn tin recap vào nhóm: 3']

FUTURE STATE — 6 phút

[1 Copy log chat vào tool: 1']
→ [2 AI trích xuất bảng Action Items (Task, Assignee, Deadline): 1']
→ [3 Nhóm trưởng review & chỉnh sửa nhanh: 3']  <-- human boundary
→ [4 1-click sync sang Trello & post Discord recap: 1']

Fallback: nếu AI nhận diện sai người hoặc thiếu deadline → Nhóm trưởng sửa tay trực tiếp trên bảng preview trước khi bấm đồng bộ.
```

---

#### Problem Card #2 — Gợi ý Edge Cases & Boundary Test Cases cho hàm logic nghiệp vụ

```text
Problem 1 câu:
Khi viết unit test cho các module logic phức tạp, developer mất 35-45 phút tự suy nghĩ kịch bản kiểm thử nhưng vẫn thường xuyên bỏ sót các trường hợp biên (boundary/edge cases), dẫn đến phát sinh bug tiềm ẩn khi demo sản phẩm.

Actor:
Backend Developer và Tester trong nhóm đồ án môn học.

Thời điểm / bối cảnh:
Sau khi hoàn thành viết xong một hàm/module xử lý dữ liệu (ví dụ: tính voucher giảm giá, phân quyền RBAC, validate form đăng ký) và chuẩn bị viết Unit Test trước khi tạo Pull Request.

Current workflow 3-7 bước:
1. Developer đọc lại code hàm và tài liệu yêu cầu tính năng.
2. Ngồi vắt óc suy đoán các trường hợp đặc biệt (chuỗi rỗng, số âm, overflow, null, định dạng sai).
3. Ghi danh sách kịch bản test nháp ra comment trong code.
4. Viết các block test case cụ thể (Jest/Pytest).
5. Chạy test suite và điều chỉnh assertions khi fail.

Bottleneck:
Bước 2 — Suy nghĩ các edge case; dev thường có thiên kiến xác nhận (confirmation bias) chỉ test theo "happy path" hoặc các case hiển nhiên, rất khó tự nghĩ ra các kịch bản biên hiếm gặp (mất 20-25 phút).

Impact:
Tốn 40 phút/feature; đợt demo giữa kỳ vừa qua đã lọt 3 bug nghiêm trọng (crash server do chuỗi UTF-8 quá dài và số tiền thanh toán là số thập phân) khiến nhóm bị trừ 1.5 điểm chất lượng mã nguồn.

Success metric:
- Giảm thời gian lên kịch bản test từ 25 phút xuống dưới 5 phút/hàm.
- Tăng độ bao phủ nhánh kiểm thử (branch coverage) từ 60% lên trên 85%.
- Không còn bug biên lọt vào buổi review code của Tech Lead.

Non-AI alternative:
Sử dụng checklist kiểm thử cố định (Boundary Value Analysis checklist: min-1, min, min+1, max, null). Tuy nhiên checklist tĩnh không hiểu được logic nghiệp vụ cụ thể của hàm (ví dụ: "chỉ áp dụng mã giảm giá khi user đã xác thực email").

AI hypothesis:
LLM đọc mã nguồn hàm và docstring, phân tích luồng điều kiện (if/else, guard clauses), từ đó tự động suy luận ra bảng kịch bản kiểm thử gồm: [Tên kịch bản, Phân loại (Happy/Edge/Error), Input mẫu, Kết quả mong đợi, Rủi ro tiềm ẩn]. Developer kiểm tra tính hợp lý rồi mới sinh mã test.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 38 phút

[1 Đọc lại code hàm: 3']
→ [2 Vắt óc nghĩ edge cases: 20']  <-- bottleneck (thiên kiến, sót case dị)
→ [3 Ghi kịch bản nháp: 5']
→ [4 Viết code test Jest: 8']
→ [5 Chạy & sửa assertions: 2']

FUTURE STATE — 10 phút

[1 Dán code hàm vào prompt template: 1']
→ [2 AI phân tích AST/logic & sinh bảng Test Matrix (Happy + Edge + Error): 1']
→ [3 Dev review kịch bản, chọn lọc & bổ sung rule nghiệp vụ riêng: 4']  <-- human boundary
→ [4 AI generate test code Jest theo kịch bản đã chọn: 2']
→ [5 Chạy test suite: 2']

Fallback: nếu AI gợi ý các test case vô nghĩa hoặc ảo giác logic → Dev bấm bỏ chọn (uncheck) test case đó trước khi sinh code.
```

---

#### Problem Card #3 — Tự động tổng hợp Changelog và Release Notes từ GitHub Pull Requests

```text
Problem 1 câu:
Mỗi cuối tuần Tech Lead mất 40-50 phút mở từng Pull Request trên GitHub để đọc git diff do thành viên không ghi PR description, dẫn đến việc tổng hợp release notes bị trễ và dễ bỏ sót các thay đổi quan trọng.

Actor:
Tech Lead nhóm đồ án (Thái Duy) và các thành viên phụ trách kiểm thử (Tester).

Thời điểm / bối cảnh:
Tối Chủ Nhật hàng tuần, trước khi đóng nhánh sprint và deploy phiên bản mới lên môi trường Staging.

Current workflow 3-7 bước:
1. Mở danh sách 10-15 PR đã merged trong tuần trên GitHub repo.
2. Mở từng PR để kiểm tra nội dung; nhận thấy đa số PR description bị để trống hoặc chỉ ghi 1-2 từ sơ sài ("fix bug", "update ui").
3. Phải click vào tab "Files changed" để đọc từng đoạn code diff nhằm hiểu xem PR đó thực sự thay đổi gì.
4. Tự viết tóm tắt từng tính năng/bugfix vào file Markdown CHANGELOG.md theo chuẩn Keep a Changelog.
5. Copy nội dung release notes gửi vào kênh Discord #announcements và tạo GitHub Release tag.

Bottleneck:
Bước 3 — Đọc và suy luận ý nghĩa của 10-15 PR từ raw code diff mất 25-30 phút, gây mệt mỏi và dễ tóm tắt sai tính năng nghiệp vụ.

Impact:
Tốn ~45 phút mỗi cuối tuần của Tech Lead; tester không nắm rõ các màn hình vừa sửa đổi để kiểm thử hồi quy; 1 lần deploy thiếu release notes dẫn đến lỗi conflict trên Staging mà không rõ do commit nào gây ra.

Success metric:
- Giảm thời gian soạn Changelog từ 45 phút xuống dưới 8 phút.
- 100% PR được phân loại chính xác theo nhóm (Features / Fixes / Performance / Dependencies).

Non-AI alternative:
Đặt GitHub PR Template bắt buộc điền và cài GitHub Action chặn merge nếu PR description dưới 50 từ. (Nhược điểm: thành viên đối phó bằng cách copy-paste chữ vô nghĩa vào template).

AI hypothesis:
Một script CLI hoặc GitHub Action tự động trích xuất diff tóm lược của các PR đã merge, gửi vào LLM kèm context tên branch/commit để sinh bản nháp Release Notes bằng tiếng Việt ngắn gọn, súc tích, phân loại theo mục. Tech Lead chỉ cần đọc lướt và xác nhận.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 45 phút

[1 Mở GitHub PR list: 3']
→ [2 Soát description trống: 5']
→ [3 Đọc code diff từng PR: 25']  <-- bottleneck (rất mệt, tốn thì giờ)
→ [4 Viết Changelog Markdown: 8']
→ [5 Tạo Tag & gửi Discord: 4']

FUTURE STATE — 8 phút

[1 Chạy CLI command / trigger Action: 1']
→ [2 AI phân tích diffs & sinh bản nháp Changelog phân loại: 2']
→ [3 Tech Lead review và chỉnh sửa câu từ: 4']  <-- human boundary
→ [4 1-click Publish GitHub Release & thông báo Discord: 1']

Fallback: nếu AI hiểu sai ý nghĩa của một PR phức tạp → Tech Lead sửa nhanh dòng mô tả đó trên bản nháp Markdown trước khi push.
```

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card #1 — Trích xuất Action Items, Người phụ trách và Deadline từ tin nhắn thảo luận Discord/Zalo nhóm đồ án.
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Đây là nỗi đau nhức nhối diễn ra đều đặn 1-2 lần mỗi tuần của mọi nhóm sinh viên làm đồ án: thảo luận rất hăng say nhưng sau đó các cam kết bị chìm nghỉm trong hàng trăm tin nhắn chat. Việc biến văn bản tự nhiên lộn xộn thành dữ liệu có cấu trúc (Task, Assignee, Deadline) là thế mạnh cốt lõi của LLM mà các công cụ Rule-based hay checklist truyền thống hoàn toàn bó tay. Về mặt số đo, nó giúp cắt giảm thời gian từ 28 phút xuống dưới 6 phút và loại bỏ triệt để tình trạng trễ hạn hoặc quên task trong nhóm.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Trong nhóm chat sinh viên, mọi người hay dùng từ lóng, viết tắt, không dấu và câu cụt ("ông push chưa", "tối mai tui làm cho") — làm sao đảm bảo AI không gán nhầm người hoặc hiểu sai thời gian hẹn (ví dụ: "mai" là ngày hôm sau hay ngày deadline của môn học)?
2. Liệu việc bắt buộc nhóm gõ lệnh bot hoặc copy-paste log chat có tạo thêm gánh nặng thao tác (friction) khiến người ta ngại dùng sau 1-2 tuần đầu không?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
  1. *Actor & Context:* Nhóm chat thường trộn lẫn chuyện cá nhân, tán gẫu, meme với việc học; nguy cơ rò rỉ dữ liệu riêng tư nếu quăng cả đoạn chat vào LLM bên ngoài.
  2. *False commitment:* Nhiều câu chat chỉ là thảo luận thăm dò ("chắc để tui xem thử", "hay là làm cách này?") chứ chưa phải cam kết chốt hạ; AI dễ sinh ra hàng loạt task "rác".
- Tôi sửa gì:
  1. Bổ sung bước tiền xử lý lọc tin nhắn theo khung giờ họp hoặc người dùng bôi đen đoạn chat muốn trích xuất thay vì ném cả lịch sử trò chuyện.
  2. Thiết kế giao diện Review nhanh (Human boundary): AI chỉ đưa ra dạng danh sách gợi ý kèm độ tin cậy (Confidence score), nhóm trưởng tick chọn những task thực sự đã chốt trước khi sync lên Trello.

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge

