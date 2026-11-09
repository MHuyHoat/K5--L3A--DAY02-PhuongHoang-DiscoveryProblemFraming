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

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Người bán hàng mất thời gian hằng tuần để tra giá đã bán, hỏi lại giá và đếm tồn kho | Value | 5 | 3 | Đã kiểm chứng (3.2): xảy ra hằng tuần ở cả 4 vai trò, nhưng mỗi lần tra giá chỉ 1–5 phút |
| 2 | Nguyên nhân gốc nằm ở bước **ghi nhận** giao dịch (ghi muộn, ghi sót, ghi rải rác), không phải ở bước **tra cứu** | Value | 5 | 4 | Đã kiểm chứng (snapshot #2, #3) |
| 3 | Người đứng quầy không kịp gõ hoặc ghi tay từng giao dịch lúc đông khách | Usability | 5 | 3 | Đã kiểm chứng (snapshot #2: "Lúc đông khách thì bán xong mới ghi, đôi khi quên mất") |
| 4 | Người bán sẵn sàng **nói một câu ngắn** ("bán 2 tai nghe Sony 350 nghìn") hoặc **chụp ảnh giấy ghi tạm** thay cho việc gõ tay, và chịu bấm xác nhận trước khi lưu | Usability | 5 | 1 | Kiểm chứng tiếp |
| 5 | AI nhận diện đúng tên hàng, số lượng và giá từ giọng nói hoặc ảnh tiếng Việt với danh mục hàng điện tử (tên model dài, viết tắt, cùng một món nhiều mức giá) | Feasibility | 5 | 2 | Kiểm chứng tiếp |
| 6 | Khi AI ghi sai, người bán phát hiện và sửa được ngay ở bước xác nhận, nên sai sót không lọt vào số liệu tồn kho; chi phí công cụ nằm trong mức cửa hàng chấp nhận | Viability | 4 | 2 | Sau |

**Đã kiểm chứng trong buổi:** #1, #2, #3 (phỏng vấn 4 người, mục 3.2).

**Cần kiểm chứng tiếp:** #4 và #5. Đây là hai giả định quan trọng cao, bằng chứng thấp, quyết định có nên đưa AI vào bước ghi nhận hay không. Cách kiểm chứng: lấy 10 giao dịch thật của cửa hàng, cho người đứng quầy đọc thử vào một công cụ ghi đơn bằng giọng nói (ví dụ Knote ở 3.3), đếm số đơn AI nhận đúng tên hàng, số lượng và giá; hỏi người bán có chịu dùng cách này lúc đông khách không.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn (4 người tại cửa hàng điện tử của gia đình Long; người được hỏi không phải thành viên nhóm)

**Snapshot #1: Chủ cửa hàng**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Chủ cửa hàng |
| Câu nói đáng nhớ nhất (nguyên văn) | "Có hôm khách hỏi giá hàng nhập tháng trước mà phải tìm lại sổ mới nhớ được." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Khách hỏi lại giá bán của một mặt hàng đã bán trước đó, chủ cửa hàng phải tìm sổ ghi chép. |
| Hiện đang xử lý bằng cách nào (workaround)? | Tra sổ, hỏi nhân viên hoặc kiểm tra tin nhắn đặt hàng. |
| Mất bao lâu, bao lần? | Khoảng 3–5 phút/lần, 3–4 lần/tuần. |
| Insight / opportunity rút ra | Lịch sử giao dịch nằm rải rác ở sổ, tin nhắn và trí nhớ của nhân viên, chưa tập trung một chỗ. |

**Snapshot #2: Nhân viên đứng quầy**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Nhân viên bán hàng |
| Câu nói đáng nhớ nhất (nguyên văn) | "Lúc đông khách thì bán xong mới ghi, đôi khi quên mất." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Bỏ sót một số giao dịch nhỏ trong lúc cửa hàng đông khách. |
| Hiện đang xử lý bằng cách nào (workaround)? | Ghi tạm ra giấy rồi tổng hợp vào cuối ngày. |
| Mất bao lâu, bao lần? | Khoảng 10–15 phút tổng hợp mỗi ngày. |
| Insight / opportunity rút ra | Ghi nhận bằng tay ngay lúc bán gây gián đoạn công việc, nhất là giờ cao điểm. Đây là nguồn gốc của dữ liệu thiếu. Cơ hội: giảm thao tác ghi nhận xuống mức người bán làm được ngay cả khi đang bận. |

**Snapshot #3: Người phụ trách kho**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Thành viên gia đình phụ trách kho |
| Câu nói đáng nhớ nhất (nguyên văn) | "Muốn biết còn bao nhiêu thì nhiều lúc vẫn phải ra đếm." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Số lượng hàng trên sổ không khớp với hàng thực tế. |
| Hiện đang xử lý bằng cách nào (workaround)? | Kiểm đếm trực tiếp và ghi lại số lượng. |
| Mất bao lâu, bao lần? | 20–30 phút/lần, khoảng 2 lần/tuần. |
| Insight / opportunity rút ra | Tồn kho không được cập nhật theo từng giao dịch nên sổ không phản ánh đúng thực tế. |

**Snapshot #4: Người hỗ trợ bán hàng**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Thành viên gia đình hỗ trợ bán hàng |
| Câu nói đáng nhớ nhất (nguyên văn) | "Nhiều mặt hàng phải hỏi lại người nhà vì không nhớ giá nhập hoặc giá bán." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Không chắc giá bán của một mặt hàng khi chủ cửa hàng vắng mặt. |
| Hiện đang xử lý bằng cách nào (workaround)? | Gọi điện hoặc nhắn tin hỏi chủ cửa hàng. |
| Mất bao lâu, bao lần? | 1–3 phút/lần, khoảng 3 lần/tuần. |
| Insight / opportunity rút ra | Thông tin giá nhập và giá bán chỉ nằm trong đầu chủ cửa hàng, chưa được chia sẻ cho những người cùng bán. |

**Tổng hợp:**

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn tại cửa hàng | 4 người (4 vai trò khác nhau) | 4/4 người gặp vấn đề hằng tuần. Thời gian mất mỗi tuần: tra giá (chủ) 9–20 phút; hỏi lại giá (người hỗ trợ) 3–9 phút; tổng hợp sổ cuối ngày 10–15 phút/ngày; kiểm đếm kho 40–60 phút | Mỗi lần **tra giá chỉ mất 1–5 phút**, ngắn hơn nhóm nghĩ. Phần tốn thời gian nhất là **tổng hợp sổ và đếm kho**, không phải tra cứu. Nhân viên không kịp ghi tay lúc đông khách, nên giải pháp nào đòi gõ nhiều thao tác tại quầy cũng có rủi ro |
| Research công cụ có sẵn (3.3) | 5 công cụ | Phần mềm bán hàng (KiotViet, Sapo, MISA eShop) đã tự trừ tồn kho và lưu lịch sử giá. Đã có công cụ AI tạo đơn từ giọng nói và ảnh (Knote, MISA AMIS CRM) | Công cụ AI giọng nói hiện tối ưu cho món ăn có tên ngắn; chưa có bằng chứng chạy tốt với tên model hàng điện tử |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

- **Đổi bottleneck:** từ "tra cứu thông tin trong sổ" sang **"giao dịch không được ghi ngay và ghi đủ lúc bán, vì ghi tay quá chậm khi đông khách"**. Tra giá chỉ là triệu chứng (1–5 phút/lần). Nguyên nhân là dữ liệu ghi muộn, ghi sót, nằm rải rác, dẫn tới phải tổng hợp cuối ngày (10–15 phút/ngày) và đếm kho bằng tay (40–60 phút/tuần).
- **Mở rộng actor:** từ "gia đình chủ cửa hàng" thành **4 vai trò cùng bán hàng**: chủ cửa hàng, nhân viên đứng quầy, người phụ trách kho, người hỗ trợ bán.
- **Xác định cơ hội cho AI:** bước có độ mơ hồ cao nhất là chuyển **lời nói hoặc ảnh giấy ghi tạm** (đầu vào tự do, viết tắt, nhiều cách nói) thành **giao dịch có cấu trúc** (tên hàng, số lượng, giá). Đây là điểm AI hỗ trợ có cơ sở từ bằng chứng. Các bước còn lại (trừ tồn kho, lưu lịch sử giá, báo cáo) là logic cố định, phần mềm bán hàng có sẵn đã làm được.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Knote** (app ghi đơn bằng AI của KiotViet) | https://apps.apple.com/us/app/knote/id6738162895 | **Ghi nhận giao dịch** bằng giọng nói hoặc tin nhắn: nói "2 phở 50k" là AI tự lên đơn | Nhận diện giọng nói tiếng Việt; gõ tắt cũng tự gợi ý đúng sản phẩm; có dùng thử miễn phí 300 đơn | Thiết kế cho quán ăn, tên món ngắn; chưa rõ độ chính xác với tên model điện tử dài; trả phí sau dùng thử | Đã có tiền lệ AI giải đúng bottleneck "ghi nhận lúc bận" ở Việt Nam. Nhóm cần **kiểm chứng với danh mục hàng điện tử** (giả định #5) trước khi tự xây |
| **MISA AMIS CRM — Thêm đơn hàng bằng AI** | https://amis.misa.vn/274495/them-don-hang-bang-ai-tren-misa-amis-crm-nhanh-hon-chinh-xac-hon-tiet-kiem-80-thoi-gian/ | **Ghi nhận giao dịch** từ ngôn ngữ tự nhiên, ảnh hoặc file PDF | AI trích xuất thông tin và tạo sẵn đơn đầy đủ dữ liệu; sửa đơn bằng cách nhập yêu cầu | Dành cho nhân viên kinh doanh doanh nghiệp (CRM), quá nặng cho cửa hàng nhỏ; con số "tiết kiệm 80%" là của bên bán | Pattern "**ảnh hoặc câu nói → đơn nháp → người xác nhận**" áp dụng được cho giấy ghi tạm cuối ngày (snapshot #2) |
| **KiotViet** (phần mềm quản lý bán hàng) | https://apps.apple.com/vn/app/kiotviet/id1146695068 | Lưu giao dịch → tự trừ tồn kho → tra lịch sử bán và giá | Phổ biến ở Việt Nam; cảnh báo hàng tồn; chạy trên điện thoại và máy tính | Có phí hằng tháng; nhiều tính năng nên người mới dễ bối rối; vẫn cần người nhập giao dịch | Phần tra giá và tính tồn đã giải được bằng logic cố định. **AI không cần làm lại phần này**, chỉ cần đưa dữ liệu vào đúng và đủ |
| **Sapo POS** | https://www.sapo.vn/blog/hang-ton-kho-la-gi | Theo dõi xuất – nhập – tồn từng sản phẩm | Hơn 20 báo cáo kho; app Android và iOS; nhiều người dùng chung một dữ liệu | Có phí sau dùng thử; phải nhập danh mục hàng và giá ban đầu | Dữ liệu dùng chung giải pain của người hỗ trợ bán ("phải hỏi lại người nhà vì không nhớ giá") |
| **MISA eShop** | https://www.misaeshop.vn/?p=50457 | Ghi nhận tại quầy (quét mã vạch, tính tiền, in hóa đơn) → báo cáo doanh thu, tồn kho | Bản mobile miễn phí trọn đời cho hộ kinh doanh doanh thu ≤ 1 tỷ/năm | Hộ doanh thu trên 1 tỷ/năm trả phí sau 3 tháng; hàng không có mã vạch vẫn phải chọn tay | Quét mã vạch là phương án **không dùng AI** để so sánh ở CP6: nếu đa số hàng có mã vạch, có thể không cần AI ở bước ghi nhận |

**Kết luận research:**

- Phần **lưu trữ, trừ tồn kho, tra lịch sử giá** đã được phần mềm bán hàng có sẵn giải bằng logic cố định, nên nhóm không xây lại.
- Khoảng trống thật là **bước ghi nhận lúc đông khách**. Thị trường đã có công cụ AI chuyển giọng nói hoặc ảnh thành đơn hàng (Knote, MISA AMIS CRM), nghĩa là điểm can thiệp AI này **khả thi và có tiền lệ**.
- Hướng đề xuất cho CP5–6: **trợ lý AI ở bước ghi nhận**. Người bán nói một câu hoặc chụp ảnh giấy ghi tạm → AI tạo giao dịch nháp → người bán xác nhận → phần mềm bán hàng lưu và tự trừ tồn kho. Trước khi chốt, nhóm phải so sánh với phương án quét mã vạch (No AI) và kiểm chứng giả định #4, #5.

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
