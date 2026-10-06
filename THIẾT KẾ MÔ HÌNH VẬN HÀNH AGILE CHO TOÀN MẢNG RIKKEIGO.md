# THIẾT KẾ MÔ HÌNH VẬN HÀNH AGILE CHO TOÀN MẢNG RIKKEIGO

## PHẦN 1 – KIẾN TRÚC MÔ HÌNH

### 1. Phạm vi mô hình

Mô hình Agile được áp dụng cho toàn mảng sản phẩm RikkeiGo, gồm 3 đội:

- **Đội Đặt xe:** phát triển và cải tiến các chức năng liên quan đến đặt xe.
- **Đội Thanh toán:** phát triển và cải tiến các chức năng liên quan đến thanh toán, ví, phương thức thanh toán và giao dịch.
- **Đội Đối soát:** xử lý đối soát giao dịch, báo cáo và các yêu cầu liên quan đến thuế, đảm bảo tính chính xác và tuân thủ quy định.

Hai đội Đặt xe và Thanh toán có yêu cầu thay đổi thường xuyên nên áp dụng Scrum đầy đủ với nhịp Sprint cố định. Đội Đối soát cũng áp dụng nền tảng Agile/Scrum chung nhưng có thể điều chỉnh cách lập kế hoạch và ưu tiên công việc để phù hợp với tính ổn định và yêu cầu tuân thủ. Đội này không nên bị ép thay đổi theo nhịp phát triển tính năng chỉ vì hai đội còn lại có tốc độ thay đổi cao.

### 2. Các module trong mô hình vận hành

| Module | Trách nhiệm chính |
|---|---|
| **Product Backlog** | Tập hợp và sắp xếp các nhu cầu, yêu cầu thay đổi, lỗi và cải tiến |
| **Sprint Planning** | Xác định mục tiêu Sprint và lựa chọn các hạng mục có thể hoàn thành |
| **Sprint Execution** | Đội phát triển thực hiện công việc theo Sprint Backlog |
| **Daily Scrum** | Kiểm tra tiến độ và điều chỉnh kế hoạch làm việc trong ngày |
| **Definition of Done (DoD)** | Tiêu chuẩn xác định một hạng mục thực sự hoàn thành |
| **Sprint Review** | Kiểm tra Increment với các bên liên quan và thu nhận phản hồi |
| **Sprint Retrospective** | Đánh giá cách làm việc và xác định cải tiến cho Sprint tiếp theo |
| **Increment** | Kết quả sản phẩm đáp ứng Definition of Done |
| **Feedback & Improvement** | Đưa phản hồi, vấn đề và cơ hội cải tiến trở lại Product Backlog |

### 3. Phân vai

Mỗi đội có 3 vai trò Scrum chính:

**Product Owner**

- Chịu trách nhiệm tối đa hóa giá trị sản phẩm.
- Quản lý và ưu tiên Product Backlog.
- Làm rõ mục tiêu và giá trị của các hạng mục.

**Scrum Master**

- Đảm bảo Scrum được hiểu và thực hiện đúng.
- Hỗ trợ đội loại bỏ trở ngại.
- Thúc đẩy cải tiến liên tục.
- Không đóng vai trò quản lý công việc thay cho đội.

**Developers**

- Chịu trách nhiệm tạo ra Increment đáp ứng Definition of Done.
- Tự tổ chức cách thực hiện công việc.
- Chịu trách nhiệm về chất lượng sản phẩm và Sprint Backlog.

### 4. Ba trụ cột Scrum

Mô hình vận hành dựa trên ba trụ cột:

**Minh bạch (Transparency)**

- Product Backlog, Sprint Backlog và tiêu chuẩn Definition of Done được công khai.
- Trạng thái công việc và kết quả Sprint phải được nhìn thấy bởi các bên liên quan.

**Kiểm tra (Inspection)**

- Daily Scrum kiểm tra tiến độ.
- Sprint Review kiểm tra Increment và nhận phản hồi.
- Sprint Retrospective kiểm tra cách đội đang làm việc.

**Thích nghi (Adaptation)**

- Điều chỉnh Sprint Backlog khi cần thiết.
- Điều chỉnh Product Backlog dựa trên phản hồi.
- Thay đổi cách làm việc sau Retrospective.
- Không thay đổi Sprint chỉ để che giấu việc Sprint không đạt mục tiêu.

### 5. Nhịp Sprint

Mô hình sử dụng **Sprint 2 tuần** làm nhịp chung.

Lý do:

- Đủ ngắn để nhận phản hồi thường xuyên.
- Đủ dài để các đội tạo ra Increment có giá trị.
- Tạo nhịp vận hành thống nhất giữa các đội.
- Đội Đối soát vẫn giữ nhịp 2 tuần nhưng ưu tiên sự chính xác, kiểm soát và tuân thủ thay vì cố tạo ra nhiều tính năng.

Sprint là một **time-box cố định**, không kéo dài khi công việc chưa hoàn thành.

### 6. Luồng giá trị của mô hình

Luồng vận hành được thiết kế khép kín:

**Nhu cầu người dùng / yêu cầu kinh doanh**

↓  

**Product Backlog**

↓  

**Product Owner ưu tiên**

↓  

**Sprint Planning**

↓  

**Sprint Backlog + Sprint Goal**

↓  

**Developers thực hiện**

↓  

**Daily Scrum + kiểm tra và điều chỉnh**

↓  

**Increment đạt Definition of Done**

↓  

**Sprint Review**

↓  

**Phản hồi từ người dùng / bên liên quan**

↓  

**Product Backlog được cập nhật**

↓  

**Sprint Retrospective**

↓  

**Cải tiến cách làm việc**

↓  

**Sprint tiếp theo**

→ **Quay lại Product Backlog**

### 7. Áp dụng 4 giá trị Agile

Mô hình không chỉ sử dụng Scrum theo hình thức mà dựa trên 4 giá trị Agile:

**Cá nhân và sự tương tác hơn quy trình và công cụ**

Các đội được quyền trao đổi trực tiếp để giải quyết vấn đề thay vì phụ thuộc hoàn toàn vào quy trình hoặc công cụ.

**Phần mềm hoạt động hơn tài liệu đầy đủ**

Ưu tiên tạo ra Increment có thể sử dụng và kiểm chứng được thay vì chỉ hoàn thành tài liệu.

**Cộng tác với khách hàng hơn đàm phán hợp đồng**

Sprint Review được sử dụng để lấy phản hồi thực tế và điều chỉnh sản phẩm.

**Phản hồi với thay đổi hơn bám theo kế hoạch**

Product Backlog có thể thay đổi dựa trên phản hồi và nhu cầu mới. Tuy nhiên, thay đổi không có nghĩa là tùy ý phá vỡ Sprint đang chạy.

### 8. Đội Đối soát có áp dụng mô hình chung không?

**Có áp dụng nền tảng Agile/Scrum chung**, vì đội Đối soát vẫn cần minh bạch, kiểm tra thường xuyên, phản hồi và cải tiến liên tục. Tuy nhiên, đội này được điều chỉnh cách lựa chọn công việc và tiêu chuẩn hoàn thành để phù hợp với đặc thù ổn định và yêu cầu tuân thủ thuế; không áp dụng máy móc cách phát triển tính năng của Đội Đặt xe và Thanh toán.

### 9. Vai trò của 3 Artifacts

**Product Backlog**

Là danh sách duy nhất các nhu cầu và công việc cần thực hiện, được Product Owner sắp xếp theo mức độ ưu tiên.

**Sprint Backlog**

Là tập hợp các hạng mục được lựa chọn cho Sprint cùng kế hoạch thực hiện để đạt Sprint Goal.

**Increment**

Là kết quả của Sprint đáp ứng Definition of Done và có giá trị sử dụng/kiểm chứng được.

Ba Artifacts giúp mô hình đảm bảo tính minh bạch từ nhu cầu → công việc → kết quả.

---

# PHẦN 2 – XỬ LÝ TÌNH HUỐNG NGOÀI DỰ KIẾN

## Tình huống 1: Đến Sprint Review nhưng không có hạng mục nào đạt Definition of Done

### Mô hình phát hiện ở đâu?

Vấn đề được phát hiện trong quá trình **kiểm tra Increment tại Sprint Review**.

Trước đó, Definition of Done phải được thống nhất và công khai. Vì vậy, một hạng mục chưa đáp ứng DoD không được coi là Increment hoàn thành.

### Ai xử lý?

- **Developers:** chịu trách nhiệm về trạng thái và chất lượng của hạng mục.
- **Product Owner:** đánh giá giá trị và quyết định thứ tự ưu tiên tiếp theo.
- **Scrum Master:** hỗ trợ đội phân tích nguyên nhân và cải thiện quy trình.

### Cách xử lý

Không cố tình tuyên bố các hạng mục chưa đạt DoD là "đã hoàn thành".

Các hạng mục chưa hoàn thành được đưa trở lại **Product Backlog** để Product Owner đánh giá và sắp xếp lại.

Sau đó, trong **Sprint Retrospective**, đội phân tích nguyên nhân, ví dụ:

- Sprint Planning chọn quá nhiều công việc.
- Ước lượng chưa phù hợp.
- Có trở ngại chưa được xử lý.
- Definition of Done chưa được tuân thủ.
- Công việc có phạm vi quá lớn.

Đội thống nhất một hoặc một số hành động cải tiến cụ thể cho Sprint tiếp theo.

Như vậy, mô hình không che giấu việc Sprint không tạo ra Increment mà sử dụng sự minh bạch và kiểm tra để tạo ra thích nghi.

---

## Tình huống 2: Đội Thanh toán muốn kéo dài Sprint thêm 1 tuần để "làm cho xong"

### Mô hình phát hiện ở đâu?

Vấn đề được phát hiện trong quá trình **Daily Scrum**, khi đội nhận thấy công việc có nguy cơ không hoàn thành Sprint Goal.

Đồng thời, đây là vấn đề cần được xử lý thông qua nguyên tắc **Sprint là một time-box cố định**.

### Ai xử lý?

- **Developers:** chủ động điều chỉnh cách thực hiện và phạm vi công việc.
- **Product Owner:** hỗ trợ điều chỉnh phạm vi dựa trên giá trị và ưu tiên.
- **Scrum Master:** bảo vệ nguyên tắc Scrum và hỗ trợ đội xử lý trở ngại.

### Cách xử lý

**Không kéo dài Sprint thêm 1 tuần.**

Sprint của Đội Thanh toán vẫn kết thúc đúng thời điểm đã thống nhất, giống nhịp Sprint chung của mô hình.

Đội có thể:

1. Xem lại Sprint Goal.
2. Điều chỉnh phạm vi Sprint Backlog nếu cần, với sự phối hợp của Product Owner.
3. Ưu tiên hoàn thành những hạng mục có giá trị cao nhất.
4. Những hạng mục chưa đạt Definition of Done không được tính là hoàn thành.
5. Đưa phần còn lại về Product Backlog để tiếp tục ưu tiên trong Sprint sau.
6. Phân tích nguyên nhân tại Sprint Retrospective.

Nếu phát hiện Sprint Goal **không còn phù hợp hoặc đã lỗi thời**, Product Owner có thể xem xét việc hủy Sprint theo quy tắc Scrum. Tuy nhiên, việc "chưa làm xong" tự nó không phải lý do để kéo dài Sprint.

### Kết quả

Đội Thanh toán vẫn giữ được nhịp Sprint chung với Đội Đặt xe và Đội Đối soát.

Điều này giúp toàn mảng có một nhịp phản hồi ổn định, đồng thời vẫn cho phép từng đội tự tổ chức công việc và điều chỉnh phạm vi bên trong Sprint.

---

# KẾT LUẬN

Mô hình vận hành Agile cho RikkeiGo được xây dựng trên một nhịp Sprint 2 tuần, với ba đội Đặt xe, Thanh toán và Đối soát cùng sử dụng nền tảng Scrum nhưng có quyền điều chỉnh cách thực hiện phù hợp với đặc thù.

Luồng giá trị được khép kín từ **nhu cầu → Product Backlog → Sprint → Increment → Review → Feedback → cải tiến → Sprint tiếp theo**.

Mô hình đảm bảo ba trụ cột **Minh bạch – Kiểm tra – Thích nghi**, đồng thời giữ đúng tinh thần bốn giá trị Agile.

Quan trọng nhất, khi xảy ra tình huống ngoài dự kiến, mô hình không phá vỡ nguyên tắc để "làm cho xong", mà sử dụng phản hồi, minh bạch và cải tiến liên tục để xử lý vấn đề và nâng cao khả năng vận hành của đội.