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
| 1 | Gia đình Long mất đáng kể thời gian mỗi lần tra lại giá đã bán, số lượng đã xuất hoặc hàng tồn, và việc này xảy ra nhiều lần mỗi tuần | Value | 5 | 1 | Có |
| 2 | Nguyên nhân gốc nằm ở bước **ghi nhận** giao dịch (ghi thiếu, ghi không đều), chứ không phải ở bước **tra cứu** | Value | 5 | 2 | Có |
| 3 | Người đứng quầy sẵn sàng nhập đủ từng giao dịch vào phần mềm hoặc app ngay lúc bán | Usability | 5 | 1 | Có |
| 4 | Tra sai giá hoặc lệch tồn kho đã gây thiệt hại thật (bán lỗ, báo khách sai còn hàng, mất hàng không biết) | Value | 4 | 1 | Sau |
| 5 | Phần mềm bán hàng có sẵn (KiotViet, Sapo, MISA eShop) đã đủ để tra cứu nhanh, không cần AI | Feasibility | 4 | 3 | Sau (đã có research ở 3.3) |
| 6 | Cửa hàng chấp nhận chi phí và thời gian chuyển đổi (phí phần mềm, nhập danh mục hàng ban đầu) | Viability | 3 | 3 | Sau |

Giả định nhóm kiểm chứng trong buổi này: #1, #2, #3. Đây là ba giả định quan trọng cao, bằng chứng thấp. Nếu #2 sai (tức là dữ liệu đã ghi đủ, chỉ khó tìm), bài toán chuyển hẳn sang hướng tra cứu. Nếu #3 sai, mọi giải pháp kể cả không dùng AI đều không chạy được.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn

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
| Insight / opportunity rút ra | Ghi nhận ngay lúc bán gây gián đoạn công việc, nhất là giờ cao điểm. Đây là nguồn gốc của dữ liệu thiếu. |

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

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn tại cửa hàng | 4 người (4 vai trò khác nhau) | 4/4 người gặp vấn đề hằng tuần. Thời gian mất cộng dồn mỗi tuần: tra giá (chủ) 9–20 phút; hỏi lại giá (người hỗ trợ) 3–9 phút; tổng hợp sổ cuối ngày 10–15 phút/ngày; kiểm đếm kho 40–60 phút | Mỗi lần **tra giá chỉ mất 1–5 phút**, ngắn hơn nhóm nghĩ. Phần tốn thời gian nhất là **tổng hợp sổ và đếm kho**, không phải tra cứu. Nhân viên ngại ghi ngay lúc đông khách, nên giải pháp nào đòi nhập liệu tại quầy cũng có rủi ro |
| Research công cụ có sẵn (3.3) | 3 công cụ | KiotViet, Sapo POS, MISA eShop đều ghi nhận bán hàng, lưu lịch sử giá và tự trừ tồn kho theo từng giao dịch | Không công cụ nào giải được việc người bán không ghi kịp lúc đông khách |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

- **Đổi bottleneck:** từ "tra cứu thông tin trong sổ" sang **"giao dịch không được ghi ngay và ghi đủ lúc bán"**. Tra giá là triệu chứng (1–5 phút/lần). Nguyên nhân là dữ liệu ghi muộn, ghi sót, nằm rải rác, dẫn tới phải tổng hợp cuối ngày (10–15 phút/ngày) và đếm kho bằng tay (40–60 phút/tuần).
- **Mở rộng actor:** từ "gia đình chủ cửa hàng" thành **4 vai trò cùng bán hàng**: chủ cửa hàng, nhân viên đứng quầy, người phụ trách kho, người hỗ trợ bán.
- **Sửa Job Story:** *Khi bán một món hàng, kể cả lúc đông khách, người bán muốn ghi lại giao dịch thật nhanh vào một nơi chung, để mọi người trong cửa hàng tra được giá và tồn kho mà không phải hỏi nhau hay ra đếm.*

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **KiotViet** (phần mềm quản lý bán hàng) | https://apps.apple.com/vn/app/kiotviet/id1146695068 | Ghi nhận giao dịch tại quầy → tự trừ tồn kho → tra lịch sử bán và giá | Phổ biến ở Việt Nam; có cảnh báo hàng tồn, thống kê hàng bán chạy; chạy trên điện thoại và máy tính | Có phí hằng tháng; nhiều tính năng nên người mới dễ bối rối; vẫn phải có người nhập giao dịch | Việc tra giá và tính tồn (đúng 2 pain của chủ cửa hàng và người phụ trách kho) đã được giải bằng **Rule**, không cần AI |
| **Sapo POS** | https://www.sapo.vn/blog/hang-ton-kho-la-gi | Ghi nhận bán hàng → theo dõi xuất – nhập – tồn từng sản phẩm | Hơn 20 báo cáo kho; có app trên Android và iOS; nhiều người cùng dùng chung một dữ liệu | Có phí sau thời gian dùng thử; phải nhập danh mục hàng và giá ban đầu | Dữ liệu dùng chung giải được pain của người hỗ trợ bán ("phải hỏi lại người nhà vì không nhớ giá"). Chi phí lớn nhất là **công nhập danh mục ban đầu**, không phải tiền phần mềm |
| **MISA eShop** | https://www.misaeshop.vn/?p=50457 · https://www.misaeshop.vn/7511/phan-mem-in-hoa-don-ban-hang/ | Ghi nhận tại quầy bằng **quét mã vạch, tính tiền, in hóa đơn từ điện thoại** → báo cáo doanh thu, tồn kho | Bản mobile miễn phí trọn đời cho hộ kinh doanh doanh thu ≤ 1 tỷ/năm; quét mã vạch giúp ghi nhanh hơn ghi tay | Hộ doanh thu trên 1 tỷ/năm phải trả phí sau 3 tháng; hàng không có mã vạch vẫn phải chọn tay | Quét mã vạch trực tiếp nhắm vào tín hiệu phản bác ở 3.2 ("lúc đông khách thì bán xong mới ghi"): **ghi nhận chỉ mất vài giây** thay vì ghi giấy rồi tổng hợp cuối ngày |
| **Bối cảnh chính sách** | https://www.misaeshop.vn/?p=35679 | Toàn bộ quy trình | Hộ kinh doanh đang chuyển từ thuế khoán sang kê khai; nhiều nơi được hỗ trợ phần mềm bán hàng miễn phí | Nguồn là trang của MISA (bên bán phần mềm), cần đối chiếu với văn bản của cơ quan thuế | Cửa hàng có thể **sắp phải số hóa giao dịch dù sao đi nữa**. Nên tận dụng việc đó thay vì xây công cụ riêng |

**Kết luận research:** 
- Cả 3 công cụ đều giải được 3 pain đã kiểm chứng ở 3.2 (tra giá đã bán, biết tồn kho không cần đếm, giá dùng chung cho mọi người bán) bằng logic cố định, không cần AI.
- Khoảng trống còn lại là **thói quen ghi nhận lúc đông khách**, đây là vấn đề quy trình và Usability.
- Hướng đề xuất cho CP5–6: **No AI / Rule**, tức là dùng phần mềm bán hàng có sẵn, dán mã vạch cho hàng chưa có mã, và quy định ghi nhận ngay tại quầy.
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
