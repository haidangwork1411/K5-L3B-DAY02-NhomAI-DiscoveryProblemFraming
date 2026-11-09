# Báo cáo cá nhân — 2A202603898_NguyenDinhMinh


## 1. Thông tin học viên

- Họ tên: Nguyễn Đình Minh
- MSSV: 2A202603898
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomAI
- Link repo nhóm: https://github.com/haidangwork1411/K5-L3B-DAY02-NhomAI-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

Bối cảnh: Khoảng 6 tháng tham gia dự án chuyển một hệ thống quản lý dự án của một doanh nghiệp Nhật Bản từ JDK8 lên JDK21.

Vai trò của tôi: Viết testcase cho các điểm sửa trong source code, đảm bảo testcase thỏa viewpoint và checklist có sẵn, có comment giải thích, log chạy đúng mẫu; kết quả và điểm sửa được track và review trên các file Excel của dự án. Giao tiếp qua meeting, chat Teams và trao đổi nhanh.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi nhận một điểm sửa mới trong source, tôi muốn biết ngay những viewpoint và mục checklist nào áp dụng cho điểm sửa đó, để viết testcase không thiếu trường hợp | Tester viết testcase, reviewer | Mỗi điểm sửa mất khoảng 10–15 phút chỉ để dò viewpoint/checklist hoặc 5-10 phút để dò pattern dẫn đến chỉ có thể làm được khoảng 7 đến 9 điểm sửa/ngày |
| 2 | Tốn thời gian | Khi chạy xong testcase, tôi muốn đưa kết quả, log và trạng thái tương ứng vào file Excel để track tiến độ | Tester, reviewer, leader | Khoảng 5 phút/testcase copy tay ID, kết quả, đường dẫn log vào Excel; cuối ngày còn mất thêm 15–20 phút rà lại cho khớp |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi đọc một điểm sửa do chuyển JDK8 lên JDK21, tôi muốn hiểu vì sao code phải đổi và hành vi nào có thể khác đi, để biết cần test cái gì | Tester, developer | Phải đọc diff, ghi chú của dev và tài liệu thay đổi của JDK; điểm sửa lạ mất 20–30 phút tìm hiểu |
| 4 | Pain từ người khác | Khi reviewer comment trên Excel rằng testcase thiếu comment giải thích hoặc log sai mẫu, tôi muốn sửa xong trong một lần, để không bị trả lại nhiều vòng | Tester, reviewer | Testcase bị trả lại 1–2 vòng mới qua review; lỗi hay gặp là comment thiếu, log sai format, chưa phủ đủ viewpoint |
| 5 | Lặp lại | Khi chạy testcase, tôi muốn log đầu ra đúng mẫu của dự án ngay từ đầu, để không phải chỉnh tay hoặc chạy lại | Tester | Khoảng 5–10 phút/testcase chỉnh log hoặc chạy lại khi log sai mẫu |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Tôi tự liệt kê 4 ý trước (#1–#4) từ việc làm hằng ngày ở dự án, sau đó hỏi AI gợi ý thêm theo 4 lăng kính.
- **Giữ** ý #5 vì test case được AI sinh ra chưa đảm bảo được việc theo đúng mẫu được cung cấp từ trước.
- **Bỏ:** "Lệch trạng thái giữa nhiều file Excel", vì tài liệu excel được lưu trên Microsoft 365 nên session làm việc được tự động reset giúp đảm bảo thông tin tôi có được là mới nhất
- **Bỏ:** "Khi tài liệu viết bằng tiếng Nhật, tôi muốn hiểu đúng ý từng mục, để testcase không bị lệch yêu cầu", trong công việc của tôi thì tài liệu đã được dịch toàn bộ sang tiếng Việt nên không cần thiết.
- **Bỏ:** "tự động migrate code từ JDK8 lên JDK21", vì không phải việc của tôi (việc của developer), tôi không có dấu hiệu thật về quy trình đó.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Đối chiếu điểm sửa với pattern/viewpoint/checklist khi viết testcase (#1) | Lặp lại cho mọi điểm sửa, bottleneck là một bước cụ thể, đang giới hạn năng suất ở 7–9 điểm sửa/ngày | Bị trả lại do thiếu viewpoint, hay do hiểu sai điểm sửa ngay từ đầu (#3)? |
| 2 | Cập nhật kết quả, log và trạng thái vào Excel tracking (#2) | Việc thủ công, lặp lại cho mọi testcase, thời gian đo dễ | Có thể chỉ cần macro hoặc template là đủ, không có gì để bàn thêm |
| 3 | Log và comment giải thích đúng mẫu ngay từ đầu (#5) | Là nguyên nhân trực tiếp của các vòng review bị trả lại; testcase sinh bằng AI cũng chưa theo đúng mẫu | Lỗi sai mẫu chiếm bao nhiêu phần trong số lần bị trả lại? Chưa đếm |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận một điểm sửa mới trong source, tôi muốn biết ngay điểm sửa đó thuộc pattern nào và những viewpoint, mục checklist nào áp dụng, để viết testcase không thiếu trường hợp và qua review ngay vòng đầu |
| Actor | Tester (junior) viết testcase cho các điểm sửa trong dự án chuyển JDK8 lên JDK21 |
| Thời điểm / bối cảnh | Hằng ngày, mỗi khi developer bàn giao điểm sửa; deadline theo đợt bàn giao cho khách hàng Nhật |
| Quy trình hiện tại (3–7 bước) | 1. Mở điểm sửa trong Excel tracking và đọc diff source · 2. Dò xem điểm sửa có khớp pattern đã gặp không · 3. Nếu không khớp, dò từng viewpoint/mục checklist xem cái nào áp dụng · 4. Viết testcase kèm comment giải thích · 5. Chạy testcase, lấy log đúng mẫu · 6. Ghi kết quả vào Excel, gửi review · 7. Sửa theo comment của reviewer |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3, xác định pattern và viewpoint/checklist áp dụng: 5–10 phút nếu khớp pattern đã gặp, 10–15 phút nếu phải dò viewpoint/checklist; phải lật qua lại giữa diff và file checklist, dễ bỏ sót mục |
| Impact (nếu không giải thì sao) | Chỉ làm được khoảng 7–9 điểm sửa/ngày; riêng bước dò chiếm khoảng 35–135 phút/ngày (7 × 5' đến 9 × 15'); sót viewpoint làm testcase bị trả lại 1–2 vòng, tốn thêm thời gian của cả tester và reviewer |
| Success metric (baseline → target) | Thời gian dò từ 5–15 phút xuống dưới 5 phút/điểm sửa; số điểm sửa/ngày từ 7–9 lên 10–12; tỉ lệ testcase qua review ngay vòng đầu: chưa đo chính xác (sẽ đếm từ cột review trong Excel tracking), target ít nhất 80% |
| Phương án không dùng AI | Lập bảng "pattern điểm sửa → viewpoint/checklist bắt buộc" dùng chung cho team (ví dụ: API bị xóa/deprecated, đổi thư viện, thay đổi định dạng ngày giờ); thêm cột chọn pattern và cột checkbox viewpoint trong Excel tracking; pattern mới gặp thì bổ sung vào bảng |
| Giả thuyết về AI (nếu có) | Gợi ý pattern và danh sách viewpoint có thể áp dụng từ diff + mô tả điểm sửa, tester xác nhận từng mục; không tự viết testcase thay tester. Ràng buộc: source code của khách hàng không được đưa ra công cụ bên ngoài nếu chưa được phép |
| Cảm nhận nhanh | Rule (bảng pattern → viewpoint) trước, Workflow nếu pattern quá đa dạng |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 50–65 phút/điểm sửa (7–9 điểm sửa/ngày, chưa tính vòng review lại)

[1 Đọc điểm sửa + diff: 10']
→ [2 Dò pattern đã gặp: 5–10'] ──khớp──────────────────────┐
→ [3 Không khớp: dò viewpoint/checklist: 10–15'] ← BOTTLENECK (bước 2–3)
→ [4 Viết testcase + comment: 15'] ◀───────────────────────┘
→ [5 Chạy + lấy log đúng mẫu: 5–10'] → [6 Ghi Excel, gửi review: 5']
→ [7 Sửa theo comment: 10–15'/vòng, 1–2 vòng]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi chạy xong testcase, tôi muốn đưa kết quả, log và trạng thái tương ứng vào file Excel tracking, để reviewer và leader thấy đúng tiến độ mà không phải hỏi lại |
| Actor | Tester; người đọc kết quả là reviewer và leader |
| Thời điểm / bối cảnh | Sau mỗi lượt chạy testcase và cuối ngày trước khi báo tiến độ; file Excel lưu trên Microsoft 365 nên luôn là bản mới nhất, cái tốn là nhập tay |
| Quy trình hiện tại (3–7 bước) | 1. Chạy testcase · 2. Mở file log · 3. Copy ID testcase, kết quả, đường dẫn log vào Excel · 4. Cập nhật trạng thái điểm sửa tương ứng · 5. Cuối ngày rà lại các dòng đã nhập cho khớp với log |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, copy tay ID, kết quả, đường dẫn log vào Excel: khoảng 5 phút/testcase, dễ dán nhầm dòng |
| Impact (nếu không giải thì sao) | Với ít nhất 7–9 testcase/ngày (mỗi điểm sửa ít nhất 1 testcase): khoảng 35–45 phút/ngày copy tay, cộng 15–20 phút rà cuối ngày → khoảng 50–65 phút/ngày cho việc không tạo ra testcase mới |
| Success metric (baseline → target) | Thời gian ghi kết quả từ khoảng 5 phút xuống dưới 1 phút/testcase; thời gian rà cuối ngày từ 15–20 phút xuống dưới 5 phút; số dòng nhập sai reviewer phát hiện: chưa đo (sẽ đếm 2 tuần), target 0 |
| Phương án không dùng AI | Đặt tên file log theo ID testcase; macro Excel hoặc script đọc thư mục log và điền kết quả, đường dẫn log vào đúng dòng theo ID |
| Giả thuyết về AI (nếu có) | Không cần: dữ liệu đã có cấu trúc (ID, kết quả, đường dẫn log), rule/script là đủ |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 8 phút/testcase + 15–20 phút rà cuối ngày

[1 Chạy testcase: 2'] → [2 Mở file log: 1']
→ [3 Copy ID, kết quả, đường dẫn log vào Excel: 5'] ← BOTTLENECK
→ [4 Cập nhật trạng thái điểm sửa: 1'] → [5 Rà lại cuối ngày: 15–20']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi chạy testcase, tôi muốn log đầu ra và comment giải thích đúng mẫu của dự án ngay từ đầu, để không phải chỉnh tay, chạy lại hay bị reviewer trả lại vì lỗi format |
| Actor | Tester viết và chạy testcase; reviewer kiểm format trên Excel |
| Thời điểm / bối cảnh | Mỗi testcase, trước khi gửi review; đặc biệt khi testcase được sinh nháp bằng công cụ AI, vì bản sinh ra chưa theo đúng mẫu dự án đã cung cấp |
| Quy trình hiện tại (3–7 bước) | 1. Viết testcase (có lúc sinh nháp bằng AI rồi sửa) · 2. Thêm comment giải thích · 3. Chạy testcase · 4. So log với mẫu của dự án · 5. Chỉnh log hoặc chạy lại nếu sai mẫu · 6. Gửi review · 7. Nếu reviewer báo thiếu comment hoặc log sai format, sửa và gửi lại |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5, chỉnh log hoặc chạy lại khi log sai mẫu: khoảng 5–10 phút/testcase |
| Impact (nếu không giải thì sao) | Với 7–9 testcase/ngày: khoảng 35–90 phút/ngày chỉ để chỉnh format; lỗi lọt qua thì bị trả lại thêm 1–2 vòng review, tốn thời gian của reviewer |
| Success metric (baseline → target) | Thời gian chỉnh log từ 5–10 phút xuống dưới 2 phút/testcase; số lần bị trả lại vì comment thiếu hoặc log sai format: chưa đo (sẽ đếm từ comment review trong Excel 2 tuần), target 0 |
| Phương án không dùng AI | Một hàm/lớp ghi log dùng chung đã đặt sẵn format của dự án; snippet comment mẫu trong IDE; checklist format 5 mục tự kiểm trước khi gửi review |
| Giả thuyết về AI (nếu có) | Nếu vẫn dùng AI sinh nháp testcase thì phải đưa mẫu log và mẫu comment vào đầu vào, và vẫn kiểm bằng rule (so log với mẫu) trước khi gửi review; AI không được tự quyết testcase đạt hay không |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 30–40 phút/testcase (chưa tính vòng review lại)

[1 Viết testcase (có lúc sinh nháp bằng AI): 15'] → [2 Thêm comment: 3']
→ [3 Chạy testcase: 2'] → [4 So log với mẫu: 2']
→ [5 Chỉnh log / chạy lại: 5–10'] ← BOTTLENECK
→ [6 Gửi review: 1'] → [7 Sửa vì thiếu comment / sai format: 10'/vòng]
```

### Card muốn pitch nhất

- Card số: 1 — Đối chiếu điểm sửa với pattern/viewpoint/checklist khi viết testcase.
- Vì sao: Đây là bước đang giới hạn năng suất của tôi ở 7–9 điểm sửa/ngày, bottleneck là một bước cụ thể (bước 2–3), impact thấy được qua cả thời gian lẫn số vòng review bị trả lại, và so sánh rõ được No AI / Rule / Workflow: bảng pattern → viewpoint có thể đã giải được phần lớn. Card #2 và #3 thì gần như chắc chắn chỉ cần Rule, ít chỗ để nhóm tranh luận.
- Câu hỏi muốn nhóm phản biện: "Testcase bị trả lại chủ yếu vì sót viewpoint, hay vì tôi hiểu sai điểm sửa ngay từ bước 1? Nếu là vế sau thì bottleneck thật nằm ở bước đọc hiểu điểm sửa chứ không phải bước dò viewpoint."

### AI đã phản biện card thế nào

Prompt: dán Problem Card #1 và nhờ AI đóng vai "PM hoài nghi" theo 6 câu hỏi trong worksheet, chỉ nói điểm yếu.

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 5–15 phút và "trả lại 1–2 vòng" đang dựa vào trí nhớ | Đồng ý | Ghi rõ tỉ lệ qua review vòng đầu là "chưa đo chính xác" và cách đo: đếm từ cột review trong Excel tracking |
| Gộp "dò pattern" (5–10') và "dò viewpoint/checklist" (10–15') làm một con số thì không biết nên cải thiện bước nào | Đồng ý | Tách thành bước 2 (dò pattern) và bước 3 (dò viewpoint khi không khớp pattern) trong quy trình nháp |
| Bottleneck có thể nằm ở bước 1 (hiểu điểm sửa) chứ không phải bước 2–3 | Đồng ý một phần | Giữ bước 2–3 là bottleneck vì tôi có số thời gian cho bước này, nhưng đưa nghi ngờ thành câu hỏi muốn nhóm phản biện |
| Đã có pattern lặp lại thì một bảng "pattern → viewpoint" có thể đã đủ | Đồng ý | Thêm phương án không dùng AI cụ thể; cảm nhận nhanh là "Rule trước, Workflow nếu pattern quá đa dạng" |
| Gợi ý để công cụ tự viết luôn testcase từ diff | Không đồng ý | Chính tôi đã thấy testcase do AI sinh ra không theo đúng mẫu (card #3); giữ boundary "chỉ gợi ý viewpoint, tester xác nhận và tự viết testcase" |
| Chưa nói gì về bảo mật source code của khách hàng | Đồng ý | Thêm ràng buộc bảo mật vào "Giả thuyết về AI" của card #1; sẽ đưa vào giả định Viability nếu nhóm chọn bài này |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Nội dung liên quan đến phần việc của tôi | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Chuẩn bị M1 (pattern/viewpoint/checklist), M2 (Excel tracking), M3 (log/comment); đề xuất M1 làm ứng viên ưu tiên. | Cả ba problem cards có trong bảng Pitch tại Mục 2.1; M1 được so sánh với D1. |
| Phản biện bài của bạn khác | Các câu hỏi cần thảo luận với D1: pain có phổ biến không; Calendar hoặc notifications đã đủ chưa; có thật sự cần AI không? | Bộ lập luận Q1–Q7 của Đăng được tổng hợp trong Mục 2.1. Chưa gán các câu hỏi này là lời tôi đã trực tiếp nói. |
| Nhận phản biện | Với M1, cần xem xét quyền sử dụng dữ liệu doanh nghiệp và khả năng tiếp cận người dùng để kiểm chứng. | Nhóm ưu tiên D1 vì thuận lợi kiểm chứng hơn; phản hồi trực tiếp của tôi sẽ được ghi theo trao đổi thật. |
| Gom cluster / cây OST | Hỗ trợ theo phân công: đối chiếu nhóm B (D3, M1), nhóm C (M2, M3), đồng thời xem xét OST cho D1. | Bảng Cluster và OST được trình bày tại Mục 2.2–2.3 báo cáo nhóm. |
| Chọn candidate problem | Tham chiếu 7 tiêu chí shortlist, đối chiếu D1 và M1. | D1 có 33/35 và M1 có 28/35 theo bảng điểm đề xuất tại Mục 2.4; quyết định chung chọn D1. |
| Kiểm chứng / research | Phụ trách CP4 theo TEAM.md: Assumption Map, câu hỏi The Mom Test, nghiên cứu giải pháp hiện có. | Mục 3 trình bày 5 giả định, 5 câu hỏi, 3 tình huống giả định và 4 hướng giải pháp; chưa có phỏng vấn độc lập. |
| Quy trình nhóm | Hỗ trợ rà soát mô tả quy trình trước/sau theo TEAM.md. | Mục 4 có hai sơ đồ Mermaid, bảng trước/sau, boundary và fallback. |
| Problem Statement | Hỗ trợ đối chiếu yêu cầu, metric và rủi ro cho v0/v1. | Mục 5 và Mục 7 có hai phiên bản Problem Statement, mục tiêu dưới 3 phút/lượt và bảng thay đổi. |
| Mức can thiệp AI | Hỗ trợ so sánh No AI, Rule, Workflow, Agent và làm rõ ranh giới giữa tự động hóa và quyết định của học viên. | Mục 6 đề xuất ưu tiên No AI/Rule; chưa có căn cứ cần Agent. |
| Quyết định | Phụ trách CP6 theo TEAM.md: xem xét Value, Usability, Feasibility, Viability và đề xuất Go/Not Yet. | Mục 8 khuyến nghị Go cho thử nghiệm quy trình nhỏ, Not Yet đối với hệ thống AI mới; có fallback và ngưỡng dừng. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Đọc đề, rubric, bài mẫu; viết nháp bảng scan theo dạng Job Story; gợi ý thêm ý theo 4 lăng kính | Viết đúng format Job Story, nhắc kiểm cột Job Story không có chữ "AI"; gợi ý thêm các ý như lệch trạng thái file Excel, tài liệu tiếng Nhật | Bản nháp đầu lấy bối cảnh "học viên làm lab", không phải trải nghiệm thật của tôi; số liệu là ước lượng AI tự đặt; 2 ý gợi ý không đúng với dự án: Excel lưu trên Microsoft 365 nên không lệch bản, tài liệu đã được dịch sang tiếng Việt | Đổi bối cảnh sang dự án chuyển JDK8 lên JDK21 tôi đã tham gia; sửa số theo trải nghiệm (dò viewpoint 10–15', dò pattern 5–10', 7–9 điểm sửa/ngày); bỏ các ý không đúng thực tế, giữ 5 ý |
| CP2 Problem Card | Soạn nháp 3 Problem Card + quy trình nháp từ 5 ý đã sửa; đóng vai "PM hoài nghi" phản biện card #1 | Gộp #4 vào card #1 và #3 theo đúng loại lỗi review; tách bước "dò pattern" và "dò viewpoint" thành 2 bước; chỉ ra card #2 và #3 chỉ cần Rule; nhắc ràng buộc bảo mật source code của khách hàng | Tự suy ra số không có trong scan (mỗi điểm sửa ít nhất 1 testcase, thời gian từng bước, target 10–12 điểm sửa/ngày); bản đầu có card dựa trên ý "tìm lại quyết định trên Teams" mà tôi đã bỏ; gợi ý để công cụ tự viết luôn testcase từ diff | Yêu cầu làm lại CP2 chỉ dựa trên 5 ý tôi đã sửa; rà lại các số AI tự suy ra; không đồng ý để công cụ tự viết testcase vì chính tôi thấy testcase do AI sinh ra không theo đúng mẫu dự án, giữ boundary "tester xác nhận và tự viết testcase" |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Cách bạn khác trình bày đặc điểm bài toán, hướng tiếp cận và cách giải bài toán đó.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Không. Cả nhóm đều phân tích kỹ vấn đề trước rồi mới tiến đến bước tìm hiểu về giải pháp

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Không.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Không

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

**Tài liệu của lab (trong repo):**

- [README.md](../../README.md) — mục tiêu, lịch lab, thuật ngữ.
- [CHECKPOINTS.md](../../CHECKPOINTS.md) — yêu cầu và checklist tự kiểm của CP1, CP2, CP7.
- [RULES.md](../../RULES.md) — quy định dùng AI cho từng checkpoint.
- [RUBRIC.md](../../RUBRIC.md) — tiêu chí chấm C1, C2, C4, C5.
- [docs/01-worksheet.md](../../docs/01-worksheet.md) — 4 lăng kính, mẫu Job Story, Problem Card, prompt phản biện.
- [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md) — bài mẫu, dùng để tham khảo cấu trúc (không sao chép nội dung).
- [docs/03-international-frameworks.md](../../docs/03-international-frameworks.md) — nguồn gốc các framework bên dưới.

**Framework được áp dụng trong CP1–CP2:**

- Job Story (Jobs-to-be-Done), Intercom: [How we accidentally invented Job Stories](https://www.intercom.com/blog/accidentally-invented-job-stories/) — dạng "Khi…, tôi muốn…, để…" ở mục 2 và 3.
- Double Diamond, Design Council (UK): [Framework for Innovation](https://www.designcouncil.org.uk/resources/framework-for-innovation/) — scan rộng ở CP1, thu hẹp về top 3 ở CP2.
- Building effective agents, Anthropic: [Building effective agents](https://www.anthropic.com/research/building-effective-agents) — cách phân loại No AI / Rule / Workflow / Agent ở dòng "Cảm nhận nhanh" của các card.

**Nguồn dữ liệu thật của bài:** trải nghiệm cá nhân khi viết testcase cho dự án chuyển JDK8 lên JDK21 (khoảng 6 tháng). Các con số thời gian là ước lượng của tôi, chưa có log hay số liệu chính thức; thông tin khách hàng không được đưa vào báo cáo.

**Công cụ AI đã dùng:** Claude (Claude Code), để gợi ý bản nháp scan, Problem Card và phản biện; chi tiết ở mục 5.
