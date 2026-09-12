# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Trần Nguyễn Thái Duy
- Mã học viên: 2A202602991
- Nhóm: Nhóm 2
- Candidate problem nhóm chọn: Ứng dụng AI Voice-to-Text và Medical NLP tự động soạn thảo hồ sơ bệnh án điện tử (EMR) cho bác sĩ lâm sàng Vinmec sau mỗi ca khám bệnh.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Quét 10 vấn đề thực tế từ bối cảnh Tech Lead / đồ án phần mềm và môi trường doanh nghiệp; chuẩn bị 3 Problem Cards có số đo rõ ràng. | Đóng góp góc nhìn kỹ thuật về độ trễ, cấu trúc dữ liệu và giúp nhóm có nguồn dữ liệu đa dạng để so sánh. |
| Pitch Problem Card | Trình bày Problem Card cá nhân (trích xuất Action Items cuộc họp) và tham gia phân tích sâu Card EMR Vinmec cùng đồng đội. | Giúp nhóm thấy rõ sự khác biệt giữa bài toán nội bộ quy mô nhỏ và bài toán có impact xã hội/vận hành lớn tại Vinmec. |
| Challenge bài của bạn khác | Đặt câu hỏi chất vấn gay gắt về rủi ro pháp lý y tế (bảo mật bệnh án) và nguy cơ hallucination sai tên thuốc hoặc mã bệnh ICD. | Thúc đẩy nhóm phải đưa ra chốt chặn Human Boundary bắt buộc: bác sĩ bắt buộc phải ký số duyệt bản draft EMR. |
| Gom trùng / cluster | Nhóm 12 ý tưởng thành 3 cụm: Tự động hóa tài liệu chuyên môn, Điều phối vận hành thời gian thực, và Xử lý CSKH/ticket. | Giúp nhóm loại bỏ các ý tưởng vụn vặt và tập trung nguồn lực vào cụm tài liệu y tế có giá trị cao nhất. |
| Chọn candidate problem | Tham gia debate sôi nổi để bảo vệ tính khả thi và impact của bài toán EMR Vinmec trước các ý tưởng khác (như điều phối trạm sạc xe Xanh SM). | Thuyết phục cả nhóm đồng thuận chấm điểm cao nhất cho bài toán EMR nhờ nút thắt thời gian (30-40%) cực kỳ rõ ràng. |
| Validation / research | Thu thập dẫn chứng học thuật quốc tế (Arndt 2017, Sinsky 2016) và đối chiếu các giải pháp thương mại như Nuance DAX, Suki AI. | Cung cấp bằng chứng định lượng vững chắc chứng minh đây là nỗi đau có thật toàn cầu, không phải giả định cảm tính. |
| Workflow nhóm | Trực tiếp tham gia chuẩn hóa luồng Current State (23-29 phút, nghẽn 8-12 phút gõ) và Future State (13-15 phút, AI draft song song). | Làm rõ ranh giới xử lý: máy thu âm → AI trích xuất/gợi ý mã → người (bác sĩ) kiểm tra và duyệt ký số. |
| Problem Statement | Cùng nhóm hoàn thiện PS v0 và nâng cấp lên v1 với các tiêu chí metric định lượng và boundary loại trừ nghiêm ngặt. | Chốt chặt ranh giới: AI chỉ draft dữ liệu lâm sàng, tuyệt đối không chẩn đoán thay bác sĩ và không tự ý gửi đơn thuốc. |
| Rule / Workflow / Agent | Phân tích ma trận độ mơ hồ - phức tạp; kiên quyết bảo vệ lựa chọn mức Workflow thay vì chạy theo Agent tự trị. | Giúp nhóm tránh bẫy "Agent-first" nguy hiểm trong ngành y tế, chọn giải pháp vừa sức, an toàn và chi phí hợp lý. |
| Làm slide, thuyết trình & phản biện chéo | Trực tiếp thiết kế toàn bộ Slide Pitch Deck HTML trực quan; tham gia trả lời chất vấn từ nhóm bạn và đặt câu hỏi, chấm bài cho nhóm khác. | Bộ slide được đánh giá rất chuyên nghiệp, bảo vệ thành công ý tưởng của nhóm trước lớp và học hỏi thêm nhiều góc nhìn phản biện mới. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất của tôi là việc trực tiếp xây dựng và trau chuốt toàn bộ bộ Slide Pitch Deck HTML trực quan cho nhóm, đồng thời là người kiên quyết thiết lập chốt chặn Human Boundary bắt buộc (bác sĩ phải trực tiếp ký số duyệt bản draft EMR) và đại diện nhóm trả lời các câu hỏi chất vấn kỹ thuật từ các nhóm bạn.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Mở rộng góc nhìn theo 4 lăng kính cho môi trường doanh nghiệp y tế và công nghệ. | Gợi ý các tác vụ hành chính dễ phát sinh bottleneck như nhập liệu hồ sơ, đối soát. | Đưa ra các ý tưởng viển vông, chung chung kiểu "AI tự động chẩn đoán bệnh", "AI điều trị từ xa" không có căn cứ số liệu. | Gạt bỏ các ý tưởng ảo tưởng, chỉ giữ lại pain point hành chính gõ EMR có số đo thời gian và bối cảnh thực tế. |
| Problem Card | Đóng vai một Product Manager khó tính để phản biện điểm yếu của Problem Card. | Phát hiện thiếu sót về giải pháp thay thế phi AI (Non-AI alternative) và cảnh báo rủi ro dữ liệu bệnh án nhạy cảm. | Gợi ý các workflow quá cồng kềnh (10-12 bước) mang nặng tính lý thuyết sách vở. | Rút gọn workflow về 4-5 bước nghiệp vụ cốt lõi và bổ sung quy trình fallback thủ công rõ ràng nếu AI gặp lỗi. |
| Workflow | Sinh cú pháp Mermaid để vẽ sơ đồ trực quan hóa luồng công việc trước và sau tối ưu. | Viết code Mermaid chuẩn cú pháp, chia rõ subgraph Current và Future State đẹp mắt để đưa vào slide. | Để luồng AI tự động ghi đè dữ liệu thẳng vào cơ sở dữ liệu EMR mà không qua bước duyệt của con người. | Tách riêng bước "Bác sĩ review & ký số" thành Human Boundary độc lập, bắt buộc 100% ca khám phải qua chốt chặn này. |
| Research | Tìm kiếm các tài liệu, bài báo khoa học và giải pháp thương mại tương tự trên thế giới. | Tổng hợp nhanh các tên tuổi lớn như Nuance DAX (Microsoft), Suki AI và các trích dẫn y khoa quốc tế. | Tự suy diễn và bịa ra số liệu thống kê riêng về các bệnh viện tại Việt Nam mà không có trích nguồn xác thực. | Gạch bỏ toàn bộ các số liệu không kiểm chứng được, chỉ giữ lại các nghiên cứu chuẩn peer-reviewed và đối chiếu link gốc. |
| Problem Statement | Soát lỗi diễn đạt và kiểm tra tính định lượng của Problem Statement v0. | Chỉ ra các câu chữ cảm tính, định tính như "giúp bác sĩ làm việc năng suất hơn", "giảm tải đáng kể". | Viết lại câu định nghĩa bài toán quá dài dòng, biến thành bài quảng cáo tính năng hơn là đặc tả vấn đề. | Viết lại PS v1 súc tích, lượng hóa rõ ràng mục tiêu (giảm từ 8-12 phút xuống ≤ 2 phút) và boundary phạm vi không làm. |
| Rule / Workflow / Agent | Lập bảng so sánh ưu nhược điểm kỹ thuật giữa 3 mức Rule, Workflow và Agent. | Phân tích rõ sự tốn kém tài nguyên và rủi ro mất kiểm soát khi để LLM tự lập kế hoạch trong môi trường y tế. | Có xu hướng thiên vị Agent, khuyên nên tích hợp Agent tự trị đa bước cho hiện đại và "ngầu". | Giữ vững lập trường chọn mức Workflow (AI hỗ trợ draft + người kiểm tra), kiên quyết không dùng Agent tự trị. |
| Decision | Giả lập các câu hỏi chất vấn để chuẩn bị phương án pilot và điều kiện Go/No-Go. | Gợi ý kịch bản thử nghiệm pilot thu hẹp ở một khoa phòng cụ thể để kiểm soát rủi ro ban đầu. | Cho rằng giải pháp có thể Go toàn diện ngay lập tức mà bỏ qua rào cản đào tạo bác sĩ và tinh chỉnh phương ngữ. | Bổ sung điều kiện Go có kiểm soát: chỉ chạy thử nghiệm tại 1 chuyên khoa nội trú với bác sĩ hạt nhân trước khi nhân rộng. |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Quá trình làm việc nhóm hôm nay đã mang lại cho tôi nhiều trải nghiệm thực chiến đáng giá, đặc biệt là giai đoạn tranh luận gay gắt để lựa chọn giữa bài toán điều phối trạm sạc xe Xanh SM và bài toán gõ EMR của bác sĩ Vinmec. Ban đầu nhóm có xu hướng muốn dựng một hệ thống Agent tự trị phức tạp cho hoành tráng, nhưng qua phân tích ma trận phức tạp - mơ hồ, tôi đã chủ động thuyết phục đồng đội hạ xuống mức Workflow kết hợp Human-in-the-loop để ưu tiên tuyệt đối tính an toàn y khoa. Đóng góp rõ nét nhất của tôi vào artifact cuối chính là việc tự tay thiết kế toàn bộ bộ Slide Pitch Deck HTML chuyên nghiệp, làm nổi bật sơ đồ workflow trực quan và các bằng chứng số liệu định lượng đã được xác thực cẩn thận. Khi thuyết trình trước lớp, nhóm bạn đã đặt câu hỏi chất vấn rất hóc búa về việc liệu giọng nói đặc trưng vùng miền và tiếng ồn phòng khám có khiến AI bắt sai liều lượng thuốc hay không. Tôi đã tự tin đại diện nhóm giải thích rằng hệ thống chỉ dừng lại ở vai trò trợ lý soạn thảo nháp, luôn có micro định hướng khử ồn và chốt chặn an toàn tối thượng là chữ ký số của bác sĩ trước khi lưu vào EMR. Không chỉ bảo vệ bài làm của nhóm mình, tôi còn tích cực đặt câu hỏi phản biện xoáy sâu vào ranh giới trách nhiệm cho các nhóm khác và thực hiện chấm điểm công tâm dựa trên bằng chứng thay vì ý tưởng hào nhoáng. Điều khó nhất mà tôi thấm thía sau buổi học chính là việc xác định Boundary: dũng cảm gạt bỏ những kỳ vọng viển vông để vạch rõ những gì AI không được phép làm quan trọng hơn nhiều so với việc cố vẽ ra một giải pháp toàn năng. Nếu có cơ hội làm lại từ đầu, tôi sẽ challenge nhóm mạnh hơn nữa ngay từ khâu phỏng vấn thực tế với bác sĩ lâm sàng để có thêm các bản ghi âm mẫu kiểm chứng độ chính xác của mô hình tiếng Việt.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

