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
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

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

Bài của nhóm nằm ở ô: độ mơ hồ **thấp–trung bình** × độ phức tạp **trung bình** → phù hợp mức **Workflow**.

Vì sao:
- Độ mơ hồ thấp–trung bình: câu hỏi cần trả lời rõ ràng và kiểm chứng được (hàng X đã bán chưa, giá bao nhiêu, còn tồn bao nhiêu). Phần mơ hồ nằm ở dữ liệu đầu vào: ghi chép không đồng nhất, một sản phẩm có nhiều mức giá bán.
- Độ phức tạp trung bình: quy trình có nhiều bước nối nhau (ghi nhận → lưu → tra cứu → đối chiếu → tính tồn → kiểm hàng thực tế), nhưng mỗi bước có quy tắc khá rõ, không cần AI tự lập kế hoạch hay tự ra quyết định.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Dùng phần mềm bán hàng/kho hoặc bảng tính, ghi đầy đủ từng giao dịch nhập, xuất, số lượng, giá bán. | Gia đình ghi chép đều đặn và chỉ cần tra cứu theo bộ lọc cố định. | Phải nhập tay nhiều, dễ bỏ thói quen sau vài tuần; tra cứu vẫn phải thao tác thủ công. | Làm trước (nền bắt buộc) |
| **Rule** | Bảng tính có công thức tự tính tồn, cảnh báo khi tồn dưới ngưỡng, bộ lọc theo mã hàng. | Mã sản phẩm đã chuẩn hóa, câu hỏi lặp lại và cố định. | Cứng nhắc: không hiểu cùng một sản phẩm được gọi tên khác nhau, không đọc được ghi chú tự do. | Một phần |
| **Workflow** | Ghi chép/tin nhắn/ảnh hóa đơn → AI trích xuất thành bản ghi chuẩn → người xác nhận → lưu vào bảng → hỏi đáp tra cứu trên dữ liệu đã lưu. | Có dữ liệu giao dịch ở mức tối thiểu và có người xác nhận ở từng bước. | AI trích sai số lượng hoặc giá; người dùng lười xác nhận. | **Chọn** |
| **Agent** | AI tự theo dõi tồn, tự đề xuất nhập hàng, tự đối chiếu và điều chỉnh giá. | Dữ liệu đầy đủ, ổn định và có cơ chế kiểm soát chặt. | Sai tồn kho hoặc giá gây thiệt hại thật; dữ liệu hiện chưa đủ; quá nặng cho cửa hàng gia đình. | Không |

**Mức chọn:** Workflow, đặt trên nền No AI/Rule (chuẩn hóa ghi chép trước khi ứng dụng AI).

**Vì sao không chọn mức đơn giản hơn:** Rule thuần không xử lý được ghi chép không đồng nhất (tên sản phẩm viết nhiều kiểu, nhiều mức giá cho cùng một mặt hàng, ghi chú tự do). No AI giải quyết được việc ghi đầy đủ nhưng chưa giải quyết việc tra cứu nhanh bằng câu hỏi tự nhiên. Vì vậy giữ No AI/Rule làm bước 0 (chuẩn hóa dữ liệu), rồi thêm AI ở bước trích xuất và tra cứu.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Trích xuất ghi chép, tin nhắn, ảnh hóa đơn thành bản ghi có cấu trúc (sản phẩm, số lượng, giá, ngày, loại nhập/xuất); trả lời câu hỏi tra cứu: hàng đã bán chưa, giá bán từng lần, số lượng đã xuất, tồn dự tính. |
| **Judgment** — con người cân nhắc, quyết định gì? | Người trong gia đình xác nhận hoặc sửa bản ghi AI trích xuất; quyết định khi tồn trên sổ lệch với hàng thực tế; quyết định khi cùng một sản phẩm có nhiều mức giá. |
| **Action** — hành động cuối cùng là gì, ai làm? | Lưu bản ghi đã xác nhận vào bảng/phần mềm; kiểm hàng thực tế khi có lệch. Người làm: thành viên gia đình trực tiếp quản lý cửa hàng. |
| **Outcome** — đo kết quả bằng gì? | Thời gian tra cứu mỗi lần (baseline cần đo); % giao dịch được ghi đầy đủ; mức lệch tồn giữa sổ và hàng thực tế; % câu trả lời đúng khi kiểm tra lại. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Ghi chép/sổ sách giao dịch, danh mục sản phẩm, hóa đơn nhập hàng; mỗi lần hỏi cần tên sản phẩm và khoảng thời gian. Hiện chưa có đủ (ghi chép chưa đầy đủ từng giao dịch) nên phải bắt đầu ghi chuẩn trước. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Người dùng bấm đúng/sai hoặc sửa trực tiếp bản ghi; kiểm kê định kỳ so với số liệu AI trả về; nhật ký các câu hỏi AI không trả lời được hoặc trả lời sai. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? **Augment.** Bằng chứng: quy trình hiện tại luôn kết thúc bằng bước kiểm hàng thực tế tại cửa hàng/kho; giá bán thay đổi theo từng giao dịch nên cần người quyết định; dữ liệu chưa đầy đủ nên chưa thể giao hẳn việc cho AI.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? **Bỏ sót tệ hơn.** Vì nếu AI bỏ sót một giao dịch hoặc báo còn hàng trong khi đã bán, sổ sẽ lệch, có thể hứa hàng với khách rồi không có, hoặc mất tiền mà không biết; còn báo nhầm "có lệch" thì chỉ tốn công kiểm lại. Thiết kế đã xử lý: AI chỉ trả lời từ dữ liệu đã lưu và nói rõ "không tìm thấy/không chắc" thay vì đoán; mỗi câu trả lời kèm bản ghi gốc để đối chiếu; không tự ghi vào sổ khi chưa được xác nhận; ưu tiên cảnh báo thừa hơn bỏ sót; kiểm kê định kỳ để bắt các lệch AI không thấy.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Thành viên trong gia đình trực tiếp bán hàng và quản lý cửa hàng điện tử. |
| **Quy trình** | Ghi nhận hàng hóa/giao dịch → tìm lại trong sổ khi cần → đối chiếu hàng nhập và hàng đã bán → tính số lượng còn lại → kiểm hàng thực tế tại cửa hàng/kho. |
| **Bottleneck** | Bước tìm lại và đối chiếu thông tin, vì giao dịch ghi chưa đầy đủ, kết hợp nhiều cách quản lý và một sản phẩm có nhiều mức giá bán. Chưa có số phút cụ thể (cần đo). |
| **Impact** | Khó nắm chính xác hàng đã xuất, giá từng giao dịch và số lượng tồn; gây khó khăn trong kiểm soát hàng hóa và quản lý kinh doanh. |
| **Success Metric** (baseline → target, cách đo) | Baseline (cần đo trong 1–2 tuần): thời gian trung bình mỗi lần tra cứu; % giao dịch có bản ghi đầy đủ; mức lệch giữa tồn sổ và tồn thực tế khi kiểm kê. Target (đề xuất, chốt sau khi có baseline): giảm thời gian tra cứu ít nhất một nửa; ≥ 90% giao dịch mới được ghi đầy đủ; mức lệch tồn giảm so với baseline. Cách đo: bấm giờ vài lần tra cứu mẫu, kiểm kê định kỳ so với sổ, đếm bản ghi đủ/thiếu. |
| **Boundary** | Chỉ làm: tra cứu lịch sử bán, giá bán, số lượng đã xuất và tồn của sản phẩm tại cửa hàng này. Không làm: tự nhập hàng, tự đặt giá, kế toán/thuế, tự ghi sổ khi chưa được xác nhận. |
| **AI intervention point** | (1) Bước trích xuất ghi chép/hóa đơn thành bản ghi chuẩn. (2) Bước tra cứu và tổng hợp thông tin trên dữ liệu đã xác nhận. |
| **Mức chọn** | Workflow |
| **Rủi ro & người kiểm tra** | Rủi ro: AI trích sai số lượng/giá; AI "bịa" khi thiếu dữ liệu; lộ dữ liệu kinh doanh. Người kiểm tra: chủ cửa hàng/thành viên gia đình xác nhận bản ghi và kiểm kê định kỳ. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Success metric | Chưa có số liệu, chỉ ghi "tra cứu nhanh hơn" | Có 3 chỉ số cần đo baseline và target đề xuất | AI phản biện chỉ ra thiếu số liệu; đồng ý và không tự đặt số khi chưa đo. |
| Phạm vi AI | "Tìm kiếm, tổng hợp, trả lời câu hỏi" chung chung | Hai điểm can thiệp rõ: trích xuất và tra cứu, có người xác nhận | Tránh dùng AI cho toàn bộ quy trình quản lý. |
| Điều kiện dữ liệu | Giả định dữ liệu "đã được ghi nhận đầy đủ" | Thêm bước chuẩn hóa ghi chép trước khi ứng dụng AI | Dữ liệu thiếu thì AI không tra cứu chính xác được. |
| Boundary | Chưa có | Thêm danh sách làm / không làm | Giữ phạm vi vừa sức, tránh trượt sang Agent. |
| Mức can thiệp | "Cảm nhận nhanh: Workflow" | Workflow có lý do, so sánh với 3 mức còn lại | Chuyển từ cảm nhận sang quyết định có lập luận. |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đúng dữ liệu | Số lượng, giá, ngày khớp bản ghi gốc trên bộ câu hỏi kiểm tra | Sai số lượng/giá so với bản ghi gốc |
| 2 | Trung thực khi thiếu dữ liệu | Nói rõ "không tìm thấy/không chắc" khi không có bản ghi | Tự suy đoán hoặc bịa thông tin |
| 3 | Truy vết được nguồn | Mỗi câu trả lời kèm bản ghi gốc để đối chiếu | Trả lời không có nguồn, người dùng không kiểm tra được |
| 4 | Dễ sửa | Người dùng sửa một bản ghi sai nhanh, không cần nhập lại từ đầu | Muốn sửa phải làm lại cả quy trình |
| 5 | Tiết kiệm thời gian | Thời gian tra cứu thấp hơn baseline đã đo | Không nhanh hơn cách tra sổ hiện tại |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | TB | Pain có thật (khó tra giá, số lượng đã xuất, tồn kho) và gia đình là người trực tiếp chịu. Nhưng chưa đo tần suất, chưa có số phút, chưa phỏng vấn người nhà nên chưa chắc họ sẽ chủ động dùng. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | TB | Thiết kế có bước xác nhận/sửa và dẫn nguồn bản ghi nên dễ kiểm tra. Rủi ro: người nhà không quen công nghệ, quen cách ghi cũ và có thể bỏ qua bước xác nhận. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Cao | Công cụ có sẵn (AI trích xuất, bảng tính), nhưng dữ liệu là điểm yếu nhất: giao dịch ghi chưa đầy đủ, nhiều cách ghi, chưa có danh mục sản phẩm chuẩn. Chưa chuẩn hóa dữ liệu thì AI không đạt độ chính xác. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | TB | Chi phí thấp với quy mô cửa hàng nhỏ. Cần cân nhắc việc đưa dữ liệu kinh doanh (giá nhập, doanh thu) lên dịch vụ AI và quy định hóa đơn/thuế nếu dùng làm sổ chính thức. Người vận hành hiện là bản thân bạn và gia đình nhập liệu, dễ phụ thuộc vào một người. |

### 8.2. Kết luận

**Quyết định:** Cải thiện thêm sau khi nghe nhận đóng góp

**Lý do:**
- Rủi ro Feasibility đang ở mức Cao: giao dịch ghi chưa đầy đủ, nhiều cách ghi chép, chưa có danh mục sản phẩm chuẩn. Nếu dựng AI ngay, kết quả tra cứu sẽ không đáng tin vì thiếu dữ liệu đầu vào.
- Chưa có baseline (thời gian tra cứu, tần suất lệch tồn, mức độ đầy đủ của dữ liệu) nên chưa chứng minh được vấn đề đủ lớn và chưa có mốc để biết AI có cải thiện hay không.
- Value mới chỉ dựa trên trải nghiệm của bản thân, chưa phỏng vấn hoặc quan sát người nhà, nên chưa biết họ có chịu ghi chép và xác nhận bản ghi hay không.
- Phương án No AI/Rule (chuẩn hóa ghi chép, bảng tính có công thức) rẻ, làm được ngay và là điều kiện bắt buộc cho Workflow, nên nên làm trước.

**Nếu Go — pilot nhỏ nhất:**
Chỉ làm với 1 nhóm hàng (ví dụ phụ kiện điện tử) trong 2 tuần. Gia đình ghi đầy đủ giao dịch nhập/xuất vào một bảng chuẩn. AI chỉ làm hai việc: trích xuất ghi chép/ảnh hóa đơn thành bản ghi và trả lời 3 loại câu hỏi (đã bán chưa, giá bán gần nhất, còn tồn bao nhiêu). Mọi bản ghi đều do người xác nhận. Cuối tuần 2 kiểm kê và đối chiếu với số liệu AI trả về.

**Nếu Not Yet — cần kiểm chứng gì trước:**
1. **Đo baseline** trong 1–2 tuần: bấm giờ các lần tra cứu, đếm số lần phải tìm lại sổ, ghi nhận số lần lệch tồn khi kiểm kê.
2. **Chuẩn hóa dữ liệu:** lập danh mục sản phẩm có mã thống nhất, mẫu ghi chép cố định cho nhập/xuất/bán, và kiểm tra gia đình có duy trì ghi đủ giao dịch không (đo % giao dịch có bản ghi đầy đủ).
3. **Phỏng vấn/quan sát người nhà:** họ thấy bước nào đau nhất, sẵn sàng nhập hoặc xác nhận bản ghi bằng cách nào (gõ, nhắn tin, chụp ảnh).
4. **Thử AI trên dữ liệu mẫu nhỏ** (khoảng 20–30 bản ghi thật) để xem AI trích xuất có đủ đúng không trước khi dựng cả luồng.

**Nếu No-Go — nên làm gì thay AI:**
Dùng phần mềm quản lý bán hàng và kho, hoặc bảng tính có công thức tự tính tồn và bộ lọc theo mã hàng. Đặt quy tắc ghi chép bắt buộc cho mỗi giao dịch (ngày, mã hàng, số lượng, giá, nhập/xuất) và kiểm kê định kỳ hằng tuần/tháng.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):
- Nếu sau **2 tuần** chuẩn hóa mà **dưới 70% giao dịch** được ghi đầy đủ → dừng việc dựng AI, quay về No AI (phần mềm/bảng tính) và tìm hiểu vì sao gia đình khó duy trì ghi chép.
- Nếu sau **2 tuần pilot** mà AI **trích xuất/tra cứu sai quá 10% số câu** trong bộ kiểm tra, hoặc **thời gian tra cứu không nhanh hơn baseline** → quay về Rule (bảng tính có công thức, bộ lọc cố định).

*(Các ngưỡng 70% và 10% là đề xuất ban đầu, cần chỉnh lại sau khi có baseline thực tế.)*

---

## 9. Hạn chế và hướng tiếp theo

- Bài chưa có số liệu đo thực tế (thời gian tra cứu, tần suất lệch tồn, % giao dịch ghi đủ); các target hiện chỉ là đề xuất.
- Value và Usability mới dựa trên trải nghiệm cá nhân, chưa phỏng vấn hay quan sát các thành viên khác trong gia đình.
- Chưa thử AI trên dữ liệu thật nên chưa biết độ chính xác khi trích xuất ghi chép viết tay hoặc ảnh hóa đơn.
- Chưa đánh giá kỹ vấn đề bảo mật dữ liệu kinh doanh (giá nhập, doanh thu) khi dùng dịch vụ AI bên ngoài, và quy định hóa đơn/thuế.
- Hướng tiếp theo: hỗ trợ nhập hàng từ nhiều nguồn ; dùng máy quét hình ảnh để AI hỗ trợ lưu trữ đầu vào của người dùng ; dùng AI để trích suất dữ liệu từ kho

## 10. Tài liệu tham khảo

- Repo nhóm: K5--L3A--DAY02-PhuongHoang-DiscoveryProblemFraming (https://github.com/MHuyHoat/K5--L3A--DAY02-PhuongHoang-DiscoveryProblemFraming)
- Template và hướng dẫn bài tập: docs/01-worksheet.md (trong repo nhóm)
- Google PAIR, *People + AI Guidebook* (augment vs automate, lỗi báo nhầm vs bỏ sót): https://pair.withgoogle.com/guidebook
- Agrawal, Gans, Goldfarb, *Prediction Machines* (khung Prediction – Judgment – Action – Outcome của AI Canvas)
- Marty Cagan, *Inspired* (bốn rủi ro sản phẩm: Value, Usability, Feasibility, Viability)
- Có sử dụng AI hỗ trợ gợi ý và phản biện nội dung; các nhận định cuối cùng do tôi tự kiểm tra và quyết định.
