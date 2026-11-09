# Báo cáo cá nhân — CP1 & CP2

**Học viên:** Nguyễn Gia Bảo

---

## CP1 — Scan vấn đề

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Lặp lại | Khi chuẩn bị đi học mỗi sáng, tôi muốn biết ngay hôm nay học giờ nào, phòng nào, để không đến muộn hay đi sai phòng | Sinh viên | 2–3 phút/lần, hằng ngày |
| 2 | Tốn thời gian | Khi ứng tuyển một vị trí mới, tôi muốn biết CV cần sửa chỗ nào cho khớp JD, để tăng cơ hội qua vòng lọc CV | Người tìm việc | 2 lần/tuần, khoảng 30–45 phút mỗi lần xem và sửa |
| 3 | Lặp lại | Khi người bán hoặc người mua phế liệu hỏi về giá, cách đăng tin hay thu gom, nhân viên GRAC muốn trả lời đúng và nhanh, để không mất giao dịch ngoài giờ | Nhân viên GRAC | Hằng ngày, 3–5 phút mỗi lần research vấn đề và trả lời |
| 4 | Tốn thời gian | Khi ôn luyện thi chứng chỉ tiếng Anh, tôi muốn biết đề nào mình chưa làm, để không làm trùng đề và tập trung vào dạng bài còn yếu | Người học | 8 phút/ngày cho mỗi lần tìm đề mới phù hợp |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi sắp bán rau củ quả, tôi muốn có tổng hợp, báo cáo giá từ nhiều nguồn, để buôn bán đúng giá thị trường | Nông dân | 2 tháng/lần, mỗi lần 10–15 phút để tổng hợp và xác thực thông tin |
| 6 | Pain từ người khác | Khi nhóm chia việc qua chat, tôi muốn biết task của mình là gì, hạn khi nào, đầu ra cần gì, để không làm trùng hoặc làm sai việc | Cả team | 10–12 câu hỏi về phân công/deadline/link mỗi tuần |

---

## CP2 — Top 3 Problem Cards

### Chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Sửa CV (#2) | Tốn nhiều thời gian nhất, quy trình rõ ràng, nghẽn ở bước sửa bullet | Bước nghẽn thật là sửa CV hay quyết định có nộp không? |
| 2 | Phân công trong nhóm (#6) | Bằng chứng đếm được, pain thật, nhiều người gặp | Số liệu mới đếm trong 1 nhóm, 1 tuần |
| 3 | CSKH GRAC (#3) | Actor là doanh nghiệp thật, xảy ra hằng ngày | Dữ liệu khó truy cập và phạm vi dễ bị quá rộng |

### Problem Card #1 — Sửa CV

| Trường | Nội dung |
|---|---|
| Job Story | Khi ứng tuyển một vị trí mới, tôi muốn biết CV cần sửa chỗ nào cho khớp JD, để tăng cơ hội qua vòng lọc CV |
| Actor | Sinh viên năm 3, năm 4 và những người đang tìm việc |
| Thời điểm / bối cảnh | Khi thấy JD mới trên các nền tảng tuyển dụng, thường vào buổi tối, trước hạn nộp |
| Quy trình hiện tại | 1. Đọc JD · 2. Đối chiếu yêu cầu với kỹ năng/project của mình · 3. Chọn project, viết lại bullet, thêm keyword · 4. Chỉnh layout, xuất PDF · 5. Nộp |
| Bottleneck | Bước 3, viết lại bullet: khoảng 15–20 phút, phải viết lại từ đầu cho mỗi JD |
| Impact | 2 lần/tuần × 30–45' ≈ 60–90 phút/tuần; khoảng 10 vị trí đã đánh giá hoặc nộp trong 3 tháng |
| Success metric | Thời gian mỗi JD từ 30–45 phút xuống dưới 15 phút, tỷ lệ được gọi phỏng vấn không giảm |
| Phương án không dùng AI | CV gốc + kho bullet viết sẵn theo nhóm (RAG, Agent, Web) + checklist keyword: rút ngắn bước 3, nhưng vẫn phải tự đối chiếu JD |
| Giả thuyết về AI | AI đối chiếu JD với kho bullet, đề xuất bullet và keyword còn thiếu; tôi tự chọn và sửa trước khi nộp |
| Cảm nhận nhanh | Workflow |

**Quy trình nháp**

```text
HIỆN TẠI — 30–45 phút/JD

[1 Đọc JD: 10'] → [2 Đối chiếu kỹ năng: 10']
→ [3 Viết lại bullet: 15–20'] ← BOTTLENECK
→ [4 Layout + PDF: 5'] → [5 Nộp: 1']
```

### Card #2 và #3 (tóm tắt)

| Card | Actor | Bottleneck | Metric | Cảm nhận nhanh |
|---|---|---|---|---|
| Phân công trong nhóm | Cả team (người hỏi và người trả lời) | Thông tin trôi trong chat, phải chờ người khác tìm lại | 10–12 câu hỏi lại/tuần → dưới 3 | No AI hoặc Rule |
| CSKH GRAC | Nhân viên GRAC | Tra giá/chính sách mỗi lần 3–5 phút; ngoài giờ không ai trả lời | Thời gian phản hồi: ___ → dưới 5 phút | Workflow |

### AI phản biện card #1

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 30–45 phút chỉ dựa trên trí nhớ | Đồng ý | Bấm giờ thật ở lần sửa CV tiếp theo: ___ phút |
| Bottleneck thật có thể là bước quyết định có nộp hay không, chứ chưa chắc là bước sửa CV | Đồng ý một phần | Đưa vào danh sách giả định cần kiểm chứng ở CP4 |
| Gợi ý để AI tự viết toàn bộ CV rồi tự nộp | Không đồng ý | Giữ boundary: tôi duyệt trước khi nộp, AI không được thêm kỹ năng mà tôi không có |
