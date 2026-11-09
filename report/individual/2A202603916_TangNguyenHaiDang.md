# Báo cáo cá nhân — 2A202603916_TangNguyenHaiDang

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Tăng Nguyễn Hải Đăng
- MSSV: 2A202603916
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomAI
- Link repo nhóm: https://github.com/haidangwork1411/K5-L3B-DAY02-NhomAI-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi theo dõi các thông báo môn học và lịch trình tại VinUni, tôi muốn nắm bắt được toàn bộ thông báo quan trọng và deadline sắp tới (trong 1–2 ngày), để không bỏ lỡ các mốc quan trọng như điểm danh standup hay chọn nhóm. | Học viên VinUni (bản thân tôi và các bạn cùng khóa) | Thông tin phân mảnh trên 4 kênh: Email cá nhân, Discord, Phoenix, VinUni Outlook. Khi rà nhiều kênh thường dành khoảng 10–20 phút; kiểm tra nhanh khoảng 5–10 phút/lần (theo lượt rà soát đầy đủ). Bằng chứng từ trải nghiệm cá nhân: Suýt lỡ deadline Daily Standup và từng bị trễ hạn chọn nhóm dẫn đến bị hệ thống xếp ngẫu nhiên. |
| 2 | Lặp lại | Khi nhóm làm việc độc lập trên các phần việc riêng lẻ, tôi muốn biết mỗi người đã hoàn thành đến đâu và đang vướng ở bước nào, để chủ động sắp xếp những công việc còn phụ thuộc vào nhau. | Nhóm trưởng và các thành viên nhóm (kênh Telegram) | Kênh trao đổi chính là Telegram. Tôi phải chủ động nhắn tin hỏi tiến độ 2 lần/ngày; việc thu thập, tổng hợp và theo dõi tiến độ mất khoảng 30–60 phút (chưa xác nhận đây là tổng thời gian mỗi ngày hay mỗi lần). |
| 3 | Tốn thời gian | Khi tiếp nhận một dự án phần mềm có sẵn (legacy codebase) với nhiều kho mã nguồn và dịch vụ nhỏ (microservices), tôi muốn hiểu nhanh kiến trúc hệ thống, quy trình nghiệp vụ và cách thiết lập môi trường chạy thử cục bộ, để có thể bắt đầu đóng góp mã nguồn mà không gây lỗi ngoài ý muốn. | Kỹ sư phần mềm mới tham gia dự án (bản thân tôi tại nơi làm việc) | Hệ thống phân tán nhiều repo, microservices, hướng dẫn cài đặt chưa rõ ràng, nhiều logic nghiệp vụ cũ. Phải liên tục hỏi đồng nghiệp cũ và sửa thử cục bộ. Chưa có số liệu định lượng đáng tin cậy về thời gian thiết lập hoặc số lần cần hỏi đồng nghiệp. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị hoàn thiện và nộp bài lab (như Day 01, Day 02), tôi muốn có một danh mục đối soát tập trung toàn bộ yêu cầu từ quy cách kỹ thuật đến quy định nộp, để không bị thiếu sót tiêu chí hoặc nhầm lẫn giữa việc push mã nguồn lên Git và nộp đường dẫn trên LMS. | Học viên khóa AI Thực Chiến (bản thân tôi) | Tài liệu hướng dẫn phân tán ở nhiều nguồn: README, RULES, CHECKPOINTS, RUBRIC, SUBMISSION, slide bài giảng và hướng dẫn của giảng viên. Mỗi lần kiểm tra đối soát trước khi nộp mất khoảng 30–60 phút. Bằng chứng thực tế: Từng push code lên Git nhưng sau đó vẫn phải tốn thời gian xác nhận lại quy trình nộp trên LMS. |
| 5 | Pain từ người khác | Khi gặp lỗi trong quá trình sử dụng hệ thống nội bộ, tôi muốn mô tả rõ tình huống và các thao tác gây ra lỗi, để người phụ trách kỹ thuật hiểu đúng vấn đề và hạn chế việc phải trao đổi nhiều lần. | Người dùng nội bộ và nhân viên kỹ thuật tiếp nhận yêu cầu hỗ trợ. | Tình huống cần kiểm chứng: Người dùng báo lỗi nhưng thiếu ảnh chụp màn hình, thao tác tái hiện hoặc thông báo lỗi cụ thể, khiến bộ phận kỹ thuật phải hỏi lại nhiều lần. Chưa có số liệu xác nhận về tần suất và thời gian xử lý. |

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | P1 — Thông tin môn học VinUni phân mảnh | Tần suất gặp hằng ngày, quy trình rõ, ảnh hưởng trực tiếp đến deadline thật. | Khả năng gom dữ liệu từ nhiều nền tảng (Discord, Phoenix, Outlook). |
| 2 | P4 — Phân tán tài liệu hướng dẫn Lab | Xảy ra đều đặn trước mỗi deadline nộp bài, tốn nhiều thời gian đối soát lặp lại. | Mức độ khác biệt giữa các bài lab có làm khó việc chuẩn hóa checklist không. |
| 3 | P3 — Tiếp nhận legacy codebase phức tạp | Nỗi đau thực tế khi đi làm, tác động lớn đến năng suất và chất lượng code. | Chưa có số liệu đo lường cụ thể và phạm vi có thể quá rộng so với 1 buổi lab. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi theo dõi các thông báo môn học và lịch trình tại VinUni, tôi muốn nắm bắt được toàn bộ thông báo quan trọng và deadline sắp tới (trong 1–2 ngày) tại một nơi tập trung, để không bỏ lỡ các mốc quan trọng như điểm danh standup hay chọn nhóm. |
| Actor | Học viên VinUni (bản thân tôi) |
| Thời điểm / bối cảnh | Hằng ngày, trước buổi học hoặc trước các mốc hạn nộp (23h59 / 11h59). |
| Quy trình hiện tại (3–7 bước) | 1. Mở Discord kiểm tra kênh chung và kênh lớp · 2. Vào Phoenix xem lịch học và bài tập · 3. Mở VinUni Outlook xem thông báo trường · 4. Mở Email cá nhân lọc tin nhắn liên quan · 5. Tự tổng hợp và ghi chú các deadline trong 1–2 ngày tới |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5: Đọc, đối chiếu và tổng hợp deadline từ 4 kênh (khoảng 10–15 phút/lần khi cần đối chiếu kỹ; tổng lượt rà soát ước tính 10–20 phút). |
| Impact (nếu không giải thì sao) | Suýt lỡ deadline Daily Standup; từng bị trễ hạn chọn nhóm và bị hệ thống xếp ngẫu nhiên. |
| Success metric (baseline → target) | Từ 10–20 phút/lượt rà soát (baseline theo trải nghiệm) xuống dưới 3 phút/lượt (mục tiêu dự kiến). |
| Phương án không dùng AI | Dùng bộ lọc chuyển tiếp (email forwarding/webhook) dồn thông báo về một kênh chat duy nhất. |
| Giả thuyết về AI (nếu có) | Trích xuất ngày, giờ, hành động cần làm từ văn bản thông báo thô và tóm tắt thành to-do list. |
| Cảm nhận nhanh | Rule / Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 10–20 phút/lượt (ước lượng tổng; thời gian các bước dưới đây chỉ để hình dung quy trình)
[Mở Discord: 3'] → [Mở Phoenix: 3'] → [Mở Outlook: 3'] → [Mở Email cá nhân: 2'] → [Đọc & đối chiếu deadline: 10'] ← BOTTLENECK
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị hoàn thiện và nộp bài lab (như Day 01, Day 02), tôi muốn có một danh mục đối soát tập trung toàn bộ yêu cầu từ quy cách kỹ thuật đến quy định nộp, để không bị thiếu sót tiêu chí hoặc nhầm lẫn giữa việc push mã nguồn lên Git và nộp đường dẫn trên LMS. |
| Actor | Học viên khóa AI Thực Chiến (bản thân tôi) |
| Thời điểm / bối cảnh | Cuối buổi lab, trước giờ đóng cổng nộp bài. |
| Quy trình hiện tại (3–7 bước) | 1. Mở README, RULES, CHECKPOINTS kiểm tra việc cần làm · 2. Mở RUBRIC và SUBMISSION rà soát lỗi trừ điểm · 3. Kiểm tra file và kết quả trên máy cục bộ · 4. Chạy Git commit và push lên GitHub · 5. Vào LMS dán link repo và nộp bài |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 1 & Bước 2: Đọc và đối soát chéo giữa nhiều tài liệu (khoảng 20–30 phút). |
| Impact (nếu không giải thì sao) | Bị trừ điểm do sai quy cách (sai tên file, quên xóa template) hoặc quên nộp link LMS dù đã push Git. |
| Success metric (baseline → target) | Từ 30–60 phút mỗi lần đối soát giảm xuống dưới 10 phút. |
| Phương án không dùng AI | Lập bảng checklist tổng hợp cố định tất cả quy định nộp bài cho từng buổi lab. |
| Giả thuyết về AI (nếu có) | Script hoặc AI đọc rubric và tự động quét cấu trúc repo để báo các lỗi sai quy cách trước khi nộp. |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 35-50 phút/lần
[Mở README & CHECKPOINTS: 10'] → [Đối soát chéo RUBRIC & SUBMISSION: 20'] ← BOTTLENECK → [Kiểm tra file cục bộ: 10'] → [Push Git: 3'] → [Nộp link LMS: 5']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận một dự án phần mềm có sẵn (legacy codebase) với nhiều kho mã nguồn và dịch vụ nhỏ (microservices), tôi muốn hiểu nhanh kiến trúc hệ thống, quy trình nghiệp vụ và cách thiết lập môi trường chạy thử cục bộ, để có thể bắt đầu đóng góp mã nguồn mà không gây lỗi ngoài ý muốn. |
| Actor | Kỹ sư phần mềm mới tham gia dự án (bản thân tôi tại nơi làm việc) |
| Thời điểm / bối cảnh | Những tuần đầu khi mới nhận dự án hoặc chuyển module mới. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc tài liệu kiến trúc và hướng dẫn cài đặt · 2. Clone repo và cài thư viện phụ thuộc · 3. Chạy thử cục bộ và gỡ lỗi cấu hình · 4. Hỏi đồng nghiệp cũ để xin mẫu cấu hình/tài khoản · 5. Đọc mã nguồn để lần theo luồng nghiệp vụ |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & Bước 4: Gỡ lỗi môi trường và chờ giải đáp từ đồng nghiệp (Chưa đo). |
| Impact (nếu không giải thì sao) | Kéo dài thời gian onboard, chậm tiến độ công việc, làm phiền đồng nghiệp cũ. |
| Success metric (baseline → target) | Baseline: Chưa đo → Target: Chưa đo. |
| Phương án không dùng AI | Chuẩn hóa tài liệu, đóng gói môi trường bằng Docker Compose hoặc script cài đặt 1 lệnh. |
| Giả thuyết về AI (nếu có) | AI hỗ trợ tóm tắt kiến trúc từ code và giải thích các luồng nghiệp vụ phức tạp. |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — Chưa đo tổng thời gian
[Đọc tài liệu: Chưa đo] → [Clone repo & cài phụ thuộc: Chưa đo] → [Chạy thử & gỡ lỗi môi trường: Chưa đo] ← BOTTLENECK → [Hỏi đồng nghiệp: Chưa đo] → [Đọc code hiểu luồng: Chưa đo]
```

### Card muốn pitch nhất

- Card số: Problem Card #1 (P1 — Thông tin môn học VinUni phân mảnh)
- Vì sao: Vấn đề xảy ra thường xuyên, có số liệu thời gian đo được thật, đã từng gây sự cố thực tế (trễ hạn chọn nhóm) và phạm vi vừa vặn để giải quyết trong lab.
- Câu hỏi muốn nhóm phản biện: Nếu gom thông tin bằng rule/webhook đơn giản đã giải quyết được phần lớn vấn đề thì bài toán này có thực sự cần đến AI không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1 dễ rơi vào bẫy kỹ thuật gom API/token của các nền tảng đóng hơn là bài toán cần AI xử lý. | Đồng ý | Hạ mức cảm nhận nhanh từ Agent xuống Rule/Workflow; tập trung vào bước đọc hiểu và tóm tắt deadline thay vì chỉ gom dữ liệu. |
| Card #3 thiếu hoàn toàn số liệu thời gian định lượng và phạm vi quá rộng so với thời lượng một buổi lab. | Đồng ý | Đánh dấu "Chưa đo" trung thực ở các ô số liệu; xếp ở vị trí Rank 3 để ưu tiên hai bài toán gọn hơn. |
| Card #2 giải pháp thuần Rule (checklist) có thể đã giải quyết được 80% vấn đề mà chưa cần tới AI. | Đồng ý | Xác định cảm nhận nhanh là Rule; giữ bài toán ở góc độ tối ưu quy trình đối soát trước khi nghĩ đến công cụ. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Đề xuất D1 (thông báo học tập phân tán), D2 (đối chiếu quy định lab), D3 (tiếp nhận legacy codebase); lựa chọn D1 để pitch. | Ba vấn đề xuất hiện trong bảng pitch Mục 2.1; D1 được chọn làm đề tài của nhóm. |
| Phản biện bài của bạn khác | Đối chiếu D1 với M1 của Minh về mức độ cụ thể của pain, hạn chế dữ liệu doanh nghiệp và khả năng tiếp cận người dùng. | Lý do chọn D1 thay vì M1 được trình bày ở Mục 2.4. Các câu hỏi cụ thể của Minh chỉ ghi theo trao đổi đã xác nhận. |
| Nhận phản biện | Tự phân tích và xác nhận 7 câu hỏi Q1–Q7 về mức độ phổ biến, nguyên nhân, Calendar, nhu cầu AI, đo lường, tích hợp và so sánh M1. | Thu hẹp bài toán vào thông báo/deadline bắt buộc; ưu tiên kiểm tra No AI/Rule thay vì xây AI Agent. |
| Gom cluster / cây OST | Tổng hợp sáu ứng viên thành ba cụm và tổ chức OST với một outcome, năm opportunity cho D1. | Mục 2.2–2.3 báo cáo nhóm; tách pain khỏi giải pháp. |
| Chọn candidate problem | Đưa ra lập luận chọn D1; sử dụng bảng bảy tiêu chí để đối chiếu các ứng viên. | D1 đạt 33/35 điểm trong bảng đánh giá đề xuất; nhóm ghi quyết định nghiên cứu D1 ở Mục 2.4. |
| Kiểm chứng / research | Cung cấp trải nghiệm thật về việc suýt lỡ standup, bỏ lỡ hạn chọn nhóm, khó theo dõi nhiều kênh và bất tiện trên điện thoại; hỗ trợ đối chiếu vấn đề với giải pháp sẵn có. | CP4 có Assumption Map, ba kịch bản phân tích và bốn hướng giải pháp; chưa có phỏng vấn độc lập do giới hạn thời gian. |
| Quy trình nhóm | Phụ trách diễn giải quy trình hiện tại qua bốn nguồn và đề xuất quy trình tương lai No AI/Rule, có con người kiểm tra và fallback. | Mục 4 có sơ đồ, bảng Before/After và ranh giới trách nhiệm. |
| Problem Statement | Phụ trách Problem Statement v0, tham gia đối chiếu v0/v1 theo actor, bottleneck, impact, metric, boundary. | Mục 5 và Mục 7: nhất quán mục tiêu 10–20 phút/lượt xuống dưới 3 phút/lượt (target). |
| Mức can thiệp AI | Phân tích vì sao chuẩn hóa quy trình và Rule phù hợp trước Workflow/Agent. | Mục 6 đề xuất No AI kết hợp Rule, giữ quyền quyết định ở học viên. |
| Quyết định | Cùng nhóm xem xét Go cho thử nghiệm No AI/Rule quy mô nhỏ và Not Yet cho hệ thống AI mới. | Mục 8 nêu rủi ro, tiêu chí đánh giá, fallback và ngưỡng dừng pilot. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Rà soát 5 Job Stories do tôi tự viết từ trải nghiệm cá nhân; kiểm tra xem câu văn có bị bẫy "solution trá hình" hay không. | Nhắc nhở cấu trúc chuẩn của Job Story theo 4 lăng kính và lưu ý không đưa tên công cụ/giải pháp vào phần mô tả vấn đề. | AI từng gợi ý một số ý tưởng thiên về công nghệ AI chung chung thay vì dựa trên các dấu hiệu thực tế đo lường được. | Giữ nguyên 5 bài toán thật của bản thân, tự điền số liệu thời gian (10–20 phút/lượt, 2 lần/ngày) và ghi rõ "Chưa đo" ở những chỗ chưa có số liệu. |
| CP2 Problem Card | Đóng vai phản biện cho 3 Problem Cards (P1, P4, P3) và hỗ trợ chuẩn hóa bảng biểu, sơ đồ quy trình nháp. | Chỉ ra điểm nghẽn của Card #1 dễ rơi vào việc gom API kỹ thuật thay vì giải quyết khâu đọc hiểu deadline; Card #3 thiếu dữ liệu định lượng. | AI có xu hướng mặc định giải pháp cần dùng AI/Workflow ngay từ đầu mà chưa xem xét kỹ tính khả thi của quy trình thủ công. | Đổi cảm nhận nhanh từ Agent xuống Rule/Workflow cho Card #1; xếp Card #3 xuống Rank 3 và chọn Card #1 làm bài toán pitch chính. |
| CP4 Research | Tìm kiếm tài liệu, giải pháp sẵn có (Google Calendar, Webhook Discord, Outlook Rules, Google PAIR) và kiểm tra link chính thức. | Tổng hợp nhanh các tài liệu kỹ thuật và mô hình thiết kế giải pháp (People + AI Guidebook). | AI từng trình bày 3 kịch bản hành vi A/B/C với văn phong dễ gây nhầm lẫn là kết quả phỏng vấn người thật. | Yêu cầu ghi rõ ràng: Nhóm chưa phỏng vấn độc lập do hạn chế thời gian; 3 tình huống chỉ là kịch bản giả định phân tích, không phải dữ liệu phỏng vấn thật. |
| CP5 Quy trình | Hỗ trợ chuyển đổi mô tả quy trình hiện tại và tương lai sang cú pháp sơ đồ Mermaid và bảng Before/After. | Dựng sơ đồ trực quan nhanh, chuẩn hóa cấu trúc actor, input, output, thời gian từng bước. | Trộn lẫn đơn vị thời gian (phút/ngày với phút/lượt); đặt target kỳ vọng mà chưa phân biệt rõ với baseline có số liệu thật. | Thống nhất đơn vị thời gian là phút/lượt; phân định rõ baseline 10–20 phút/lượt (thật) với target < 3 phút/lượt (kỳ vọng); bổ sung bước con người xác nhận (HITL) và phương án fallback. |
| CP5–6 Problem Statement | Soạn thảo và đối chiếu các trường trong Problem Statement v0 và v1, kiểm tra rubric về tính đo lường của metric và boundary. | Giúp làm rõ ranh giới an toàn: AI không được tự ý xóa tin nhắn hay quyết định thay học viên. | AI từng đưa ra những nhận định mang tính tuyệt đối chưa có cơ sở thực chứng ("chi phí bằng 0", "giải quyết triệt để", "khớp 100%"). | Hạ tông khẳng định, chỉnh thành "hạn chế đáng kể", làm rõ trường "AI intervention point" là "Không có" vì nhóm thống nhất chọn No AI / Rule. |
| CP6 Mức can thiệp / quyết định | Hỗ trợ phân tích ma trận Ambiguity × Complexity, gợi ý câu hỏi Google PAIR, bảng 4 rủi ro và khung ngưỡng dừng. | Cung cấp framework chuẩn của Anthropic và Marty Cagan để so sánh 4 mức can thiệp và 4 rủi ro một cách bài bản. | AI từng đánh giá cả 4 rủi ro đều ở mức "Thấp" (quá lạc quan) thiếu căn cứ; để trống khoảng cách giữa 5 phút và 30 phút trong tiêu chí đánh giá độ trễ. | Đánh giá lại rủi ro: Value (Trung bình), Usability (Thấp–TB), Viability (Trung bình); chốt quyết định GO cho micro-pilot No AI/Rule và NOT YET cho hệ thống AI mới; lấp khoảng trống trong tiêu chí độ trễ. |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi xem ba vấn đề Minh đưa ra, tôi thấy cùng là một công việc nhưng có thể có nhiều điểm gây mất thời gian khác nhau. Minh tập trung vào việc viết testcase, đối chiếu checklist, nhập kết quả vào Excel và chỉnh log đúng mẫu. Các vấn đề này khá cụ thể, có bước xử lý rõ ràng và nhiều chỗ có thể cải thiện bằng bảng mẫu hoặc script đơn giản. Tôi học được rằng khi chọn vấn đề, không nên chỉ nhìn vào việc nó nghe có vẻ hay hay liên quan đến AI, mà phải xem có xác định được người gặp vấn đề, bước bị vướng và cách đo kết quả hay không.

**6.2. Nhóm có lúc nào bị “solution-first” không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Lúc đầu, khi thấy thông báo của chương trình nằm ở Discord, Phoenix, Outlook và email cá nhân, tôi nghĩ ngay đến việc làm một hệ thống AI gom và tóm tắt thông báo. Nhưng khi phân tích lại quy trình, tôi nhận ra vấn đề chính là học viên khó theo dõi các deadline quan trọng, chứ không phải thiếu một ứng dụng AI. Vì vậy, nhóm chuyển sang xem xét cách thống nhất kênh thông báo, dùng quy tắc lọc và Google Calendar trước. Cách này đơn giản hơn và cũng dễ thử nghiệm hơn.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có. Với vấn đề D1, ban đầu tôi nghiêng về việc dùng AI để đọc thông báo và rút ra ngày giờ cần nhớ. Sau khi tự xem lại các câu hỏi phản biện, nhất là câu hỏi liệu chỉ cần chuẩn hóa thông báo và dùng rule có đủ hay không, tôi đổi hướng. Nếu thông báo có cách ghi rõ ràng và học viên biết lưu lịch, nhiều thao tác không cần AI xử lý. Tôi thấy việc chọn giải pháp ít phức tạp hơn không có nghĩa là bài làm kém đi, mà là phù hợp hơn với vấn đề đã xác định.

**6.4. Kết quả kiểm chứng có làm tôi bất ngờ không? Điều gì?**

Điều làm tôi chú ý nhất khi nghiên cứu là những công cụ quen thuộc như Google Calendar, Outlook Rules hay Discord đã hỗ trợ được nhiều bước trong việc theo dõi thông báo. Trước đó tôi chỉ nghĩ đến việc gom tất cả vào một nơi, nhưng chưa tính kỹ đến thói quen ghi lịch của người dùng. Nhóm cũng chưa có thời gian phỏng vấn độc lập các học viên khác, nên tôi hiểu rằng trải nghiệm của bản thân chưa đủ để kết luận mọi người đều gặp khó khăn giống mình. Ba tình huống A, B, C chỉ giúp nhóm đặt câu hỏi và nhìn vấn đề từ nhiều phía, chưa phải kết quả kiểm chứng thực tế.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Với tôi, khó nhất là viết cho đúng phạm vi và đưa ra chỉ số có thể đo được. Nếu chỉ ghi rằng học viên khó theo dõi thông báo thì vẫn quá chung chung. Tôi phải chỉ ra các kênh đang dùng, bước phải tự đối chiếu thông tin và hậu quả có thể xảy ra. Tôi từng suýt lỡ Daily Standup và đã trễ hạn chọn nhóm, nhưng cũng không thể lấy hai việc đó để khẳng định cả khóa học đều gặp vấn đề. Nhóm dùng mốc 10–20 phút mỗi lượt rà soát làm cơ sở ban đầu và đặt mục tiêu dưới 3 phút, đồng thời ghi rõ đây mới là mục tiêu, chưa có kết quả thử nghiệm.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ dành thời gian phỏng vấn vài học viên ngay từ đầu thay vì chỉ phân tích từ trải nghiệm của mình và nghiên cứu công cụ. Như vậy nhóm sẽ biết rõ vấn đề phổ biến đến đâu và nguyên nhân chính là do nhiều kênh thông tin hay do cách mỗi người tự quản lý deadline. Tôi cũng sẽ đặt câu hỏi về giải pháp không dùng AI sớm hơn, để tránh mất thời gian nghĩ đến một hệ thống phức tạp khi chưa thật sự cần. Tôi nghĩ đây là bài học quan trọng nhất của buổi lab: hiểu vấn đề cho rõ rồi mới chọn cách giải quyết.

**6.7. Hiểu bài:**

Vấn đề nhóm tôi chọn là học viên có thể bỏ lỡ thông báo hoặc deadline vì phải theo dõi nhiều nền tảng khác nhau. Trong quy trình hiện tại, học viên tự mở Discord, Phoenix, Outlook và email rồi đọc, đối chiếu và ghi nhớ những mốc quan trọng. Nhóm lấy khoảng 10–20 phút cho một lượt rà soát làm mốc ban đầu và đặt mục tiêu giảm xuống dưới 3 phút mỗi lượt trong thử nghiệm. Giải pháp đề xuất chỉ hỗ trợ phân loại, chuyển tiếp và nhắc lịch, còn học viên vẫn phải kiểm tra nguồn gốc và tự quyết định việc cần làm. Vì bài toán có thể xử lý phần lớn bằng cách chuẩn hóa thông báo và các quy tắc đơn giản, nhóm ưu tiên No AI kết hợp Rule thay vì dùng AI Agent. Nhóm quyết định Go đối với thử nghiệm nhỏ trong một tuần nhưng Not Yet đối với việc xây dựng hệ thống AI mới. Sau thử nghiệm, nhóm sẽ dựa vào thời gian kiểm tra và số thông báo bị bỏ sót để quyết định có cần thay đổi cách làm hay không.

---

## 7. Tài liệu tham khảo

### Tài liệu nội bộ dự án
1. Hướng dẫn thực hành Lab Day 02: [`docs/01-worksheet.md`](../../docs/01-worksheet.md)
2. Bài mẫu tham khảo chuẩn mực (Case PM Minh): [`docs/02-deliverable-example.md`](../../docs/02-deliverable-example.md)
3. Báo cáo nhóm NhomAI: [`report/team/group_report.md`](../team/group_report.md)
4. Phân công vai trò & đóng góp thành viên: [`TEAM.md`](../../TEAM.md)

### Phương pháp luận & Framework
5. Design Council (UK). *The Double Diamond design process*. https://www.designcouncil.org.uk/our-resources/the-double-diamond/
6. Alan Klement. *Designing Features using Job Stories*. Intercom Blog. https://www.intercom.com/blog/accidentally-invented-job-stories/
7. Rob Fitzpatrick. *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*. https://www.momtestbook.com/
8. Teresa Torres. *Continuous Discovery Habits: Discover Products that Create Customer Value and Business Value*. Product Talk LLC.
9. Jeff Gothelf, Josh Seiden. *Lean UX: Designing Great Products with Agile Teams*. O'Reilly Media.
10. Google PAIR. *People + AI Guidebook: User Needs + Defining Success*. https://pair.withgoogle.com/chapter/user-needs/
11. Anthropic. *Building Effective Agents*. Anthropic Research, 2024. https://www.anthropic.com/research/building-effective-agents
12. Marty Cagan. *Inspired: How to Create Tech Products Customers Love (The Four Big Risks)*. Silicon Valley Product Group. https://www.svpg.com/four-big-risks/

### Công cụ & Tài liệu kỹ thuật
13. Discord Developer Portal. *Intro to Webhooks*. https://discord.com/developers/docs/resources/webhook
14. Microsoft Support. *Use rules to manage your email in Outlook*. https://support.microsoft.com/en-us/office/use-rules-to-manage-your-email-c24f5dea-9465-4df4-ad17-a50704d66c59
