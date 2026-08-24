# 4.10.6. Hoá đơn điện tử MISA

**MISA meInvoice** là phần mềm hoá đơn điện tử. Nối nó với website để **mỗi đơn khách thanh toán xong là hoá đơn tự phát hành**, và email hoá đơn tự gửi tới khách.

**Vì sao hữu ích?** Bình thường kế toán phải mở phần mềm meInvoice, gõ lại từng đơn: tên khách, mã số thuế, từng dòng dịch vụ, tiền thuế… Mỗi hoá đơn mất vài phút, mùa cao điểm là cả buổi. Nối rồi thì website làm hết, kế toán chỉ vào kiểm tra.

> **Đường dẫn:** Menu bên trái > **Tích hợp** > **Hoá đơn điện tử MISA**

> **Cần chuẩn bị trước:** tài khoản meInvoice của công ty (chính tài khoản kế toán vẫn dùng để vào meinvoice.vn), và **ClientID + ClientSecret** — hai mã này phải liên hệ MISA xin riêng cho website, không tự lấy được trong phần mềm.

---

## 1. Nối tài khoản MISA

Điền 5 ô ở mục **Kết nối MISA meInvoice**:

| Ô | Lấy ở đâu |
| --- | --- |
| **ClientID** | MISA cấp khi bạn đăng ký kết nối website |
| **ClientSecret** | MISA cấp kèm ClientID |
| **Mã số thuế** | Mã số thuế công ty. Có đuôi chi nhánh thì gõ đủ, ví dụ `0101243150-996` |
| **Tài khoản meInvoice** | Email kế toán vẫn dùng để đăng nhập meinvoice.vn |
| **Mật khẩu meInvoice** | Mật khẩu của tài khoản đó |

Điền xong bấm **\[Kiểm tra kết nối]** — **chưa cần bấm Lưu**. Nút này thử ngay thông tin bạn vừa gõ.

**Đọc kết quả:**

| Hiện ra | Nghĩa là | Làm gì |
| --- | --- | --- |
| Khung **xanh** kèm mã số thuế, tên đơn vị | Đúng hết | Đi tiếp bước 2 |
| *"Sai thông tin đăng nhập"* | Sai tài khoản hoặc mật khẩu meInvoice | Thử đăng nhập meinvoice.vn bằng chính tài khoản đó xem có vào được không |
| *"Sai thông tin ClientID, ClientSecret"* | Hai mã kia sai | Hỏi lại MISA |
| *"User chưa được phân quyền"* | Mã số thuế không thuộc tài khoản này | Kiểm tra lại mã số thuế, nhất là phần đuôi chi nhánh |

> **Lỗi hay gặp nhất:** dán mã bị **dính dấu cách thừa** ở đầu hoặc cuối khi copy từ email. Mắt thường không thấy. Mẹo: dán xong bấm vào cuối ô, nhấn phím **End** rồi **Backspace** vài lần cho chắc.

---

## 2. Chọn mẫu hoá đơn

Bấm **\[Tải danh sách mẫu từ MISA]**. Website kéo về toàn bộ ký hiệu hoá đơn mà kế toán đã đăng ký với cơ quan thuế, rồi bạn chọn một mẫu ở ô **Mẫu hoá đơn**.

Mỗi dòng trong danh sách trông như: `1C26MAA — Hoá đơn GTGT (mẫu số 1)`

> **Không chắc chọn mẫu nào?** **Hỏi kế toán.** Đây là bước dễ sai nhất và hậu quả nặng nhất: chọn nhầm mẫu là hoá đơn xuất ra sai ký hiệu, mà hoá đơn phát hành rồi thì không sửa được.

**Mẫu số** không cần điền — website tự lấy theo mẫu bạn chọn.

Có ba loại nhãn phụ bạn có thể thấy trong danh sách:

* **không mã CQT** — hoá đơn không có mã của cơ quan thuế
* **chưa phát hành** — mẫu chưa đăng ký xong với thuế, thường **không nên chọn**
* Danh sách rất dài thì **gõ để tìm** ngay trong ô chọn

> **Khi nào cần tải lại danh sách?** Khi kế toán vừa đăng ký thêm ký hiệu hoá đơn mới với cơ quan thuế. Bình thường vài tháng mới có một lần, không cần tải thường xuyên.

---

## 3. Đặt thuế suất

Bảng **Thuế suất theo loại dịch vụ** cho phép mỗi loại một mức khác nhau — ví dụ tour 8%, khách sạn 10%.

Loại nào để **"— Theo mức mặc định —"** thì lấy mức ở ô **Thuế suất mặc định** ngay bên dưới bảng.

### Ô quan trọng nhất trang này

**"Giá bán trên website đã bao gồm VAT"** — kiểm cho đúng thực tế công ty bạn:

| | **Bật** (mặc định) | **Tắt** |
| --- | --- | --- |
| Giá khách thấy trên web | Là giá cuối cùng | Là giá **chưa** thuế |
| Website làm gì | Tách ngược ra tiền thuế | Cộng thêm tiền thuế |
| Tổng trên hoá đơn | **Đúng bằng** số khách đã trả | **Lớn hơn** số khách đã trả |

> **Chọn sai ô này là hoá đơn sai tiền hàng loạt.** Nếu không chắc, hỏi kế toán: *"Giá niêm yết trên web là giá đã gồm VAT hay chưa?"*

---

## 4. Chạy thử trước khi bật

**Đừng bật tự động ngay.** Làm một lần thử trước:

1. Vào **Đặt chỗ**, mở chi tiết một đơn **đã thanh toán**
2. Kéo xuống cuối, tới mục **Hoá đơn điện tử MISA**
3. Bấm **\[Xem trước hoá đơn]**

Nút này **không gửi gì sang MISA**, chỉ cho bạn xem hoá đơn sẽ trông thế nào: từng dòng dịch vụ, thuế suất, tổng tiền, số tiền bằng chữ.

**Kiểm ba thứ:**

* Dòng cuối có báo **"Khớp đúng tổng đơn hàng"** không?
* Thuế suất có đúng như kế toán muốn không?
* Tên khách / tên công ty có đúng không?

Ổn cả ba thì mới sang bước 5.

---

## 5. Bật lên

Tích ô **"Bật tích hợp hoá đơn điện tử MISA"**, rồi chọn:

* **Tự động xuất hoá đơn** — tick thì đơn đạt trạng thái là website tự xuất. Không tick thì bạn phải bấm tay từng đơn.
* **Xuất hoá đơn khi đơn chuyển sang** — thường chọn *Đã thanh toán*.
* **Áp dụng cho loại dịch vụ** — **không tích loại nào = áp dụng cho tất cả**. Chỉ tích khi bạn muốn giới hạn.
* **Gửi hoá đơn cho khách qua email** — xem mục 7 bên dưới.

Cuối cùng bấm **\[Lưu integrations]** màu xanh ở góc trên bên phải.

---

## 6. Dùng hằng ngày

### Xuất tự động

Không phải làm gì. Khách thanh toán xong là hoá đơn tự lên MISA.

### Xuất bằng tay

Vào **Đặt chỗ** > mở chi tiết đơn > kéo xuống **Hoá đơn điện tử MISA** > **\[Xem trước hoá đơn]** > **\[Xuất hoá đơn]**.

Trước khi bấm, panel này cho bạn biết đơn đó sẽ ra hoá đơn loại nào:

* **"Khách yêu cầu hoá đơn công ty"** kèm tên công ty và mã số thuế — khách đã tick *Xuất hoá đơn VAT* lúc thanh toán
* **"Khách không yêu cầu hoá đơn VAT"** — hoá đơn cho cá nhân, để trống mã số thuế

### Xem lại hoá đơn đã xuất

Menu bên trái > **Hoá đơn điện tử** > **Nhật ký hoá đơn**.

Ở đây tra được theo **mã đơn, số hoá đơn, mã tra cứu**, lọc theo **trạng thái** và **dịch vụ**. Mở một hoá đơn ra xem được số hoá đơn, mã tra cứu, và nhật ký các lần gửi email.

---

## 7. Gửi hoá đơn cho khách

Ô **"Gửi hoá đơn cho khách qua email"**:

* **Tắt** — website **chỉ xuất hoá đơn lên MISA**, không gửi gì cho khách. Kế toán tự gửi sau.
* **Bật** — xuất xong là gửi luôn email tra cứu hoá đơn tới địa chỉ khách ghi trên đơn.

Hai ô phụ:

* **Gửi thêm bản sao tới (CC)** — thường điền email kế toán để nhận bản sao mọi hoá đơn
* **Email nhận thư trả lời** — khách bấm *Trả lời* trên mail hoá đơn thì thư về địa chỉ này

> **MISA chỉ cho gửi mỗi phút một email.** Nhiều đơn thanh toán cùng lúc thì các hoá đơn sau xếp hàng gửi lần lượt, mỗi phút một cái. Đây là giới hạn của MISA, không phải lỗi website.

> **Cần bật cron của website** thì việc gửi lần lượt mới tự chạy. Nhờ bên kỹ thuật kiểm giúp. **Chưa có cron thì hoá đơn vẫn xuất bình thường**, chỉ là email nằm chờ và bạn phải vào Nhật ký bấm gửi tay.

### Gửi lỗi thì làm gì

Hoá đơn **vẫn còn nguyên**, không mất. Vào **Nhật ký hoá đơn**, cột **Email** sẽ hiện đỏ. Mở hoá đơn đó ra, sửa lại địa chỉ email nếu cần, bấm **\[Gửi lại]**.

> Nút **\[Gửi lại]** dùng được cả khi bạn đang tắt ô gửi email tự động — tiện khi chỉ muốn gửi riêng một hoá đơn.

---

## Ba điều nhất định phải nhớ

> ### ⚠️ Hoá đơn phát hành rồi thì KHÔNG rút lại được
>
> Không có nút xoá, không có nút sửa. Sai thì chỉ còn cách lập **hoá đơn điều chỉnh** bên phần mềm MISA — việc này kế toán phải làm thủ công.
>
> Vì vậy: **luôn Xem trước trước khi Xuất.**

> ### Một đơn chỉ xuất được một hoá đơn
>
> Website tự chặn xuất lần hai cho cùng một đơn, kể cả khi bạn bấm nút. Đây là chốt an toàn cố ý, không phải lỗi.

> ### Đổi mật khẩu meInvoice thì vào đây bấm Lưu một lần
>
> Website giữ phiên đăng nhập với MISA trong 30 ngày. Đổi mật khẩu bên MISA mà không bấm Lưu lại ở đây thì tới lúc phiên cũ hết hạn, hoá đơn sẽ báo lỗi đăng nhập.

---

## Xử lý sự cố

**Thanh toán xong mà không thấy hoá đơn đâu.** Kiểm theo thứ tự:

1. Ô **"Bật tích hợp hoá đơn điện tử MISA"** còn tích không?
2. Ô **"Tự động xuất hoá đơn"** có tích không?
3. Mục **"Áp dụng cho loại dịch vụ"** — có tích loại nào không? Nếu có mà loại đơn đó không nằm trong danh sách thì website cố ý bỏ qua.
4. Mục **"Xuất hoá đơn khi đơn chuyển sang"** — đơn đã tới trạng thái đó chưa?
5. Vào **Nhật ký hoá đơn** xem có dòng nào màu đỏ không — nếu có, thông báo lỗi ghi ngay trên đó.

**Hoá đơn báo đỏ trong Nhật ký.** Mở ra đọc dòng lỗi. Hay gặp nhất:

| Lỗi | Nguyên nhân |
| --- | --- |
| *Chưa chọn mẫu hoá đơn* | Quay lại bước 2 |
| *Chưa nhập đủ thông tin kết nối* | Thiếu ô nào đó ở bước 1 |
| *Sai thông tin đăng nhập* | Mật khẩu meInvoice đã đổi — vào bấm Lưu lại |
| *Mã số thuế không hợp lệ* | Khách khai sai mã số thuế lúc thanh toán |

**Trước khi gọi hỗ trợ, chuẩn bị:** mã đơn hàng, **ảnh chụp màn hình đầy đủ dòng báo lỗi** trong Nhật ký hoá đơn (đừng cắt), và cho biết đơn đó xuất tự động hay bạn bấm tay.

---

## Xem thêm

* [4.10. Tích hợp](../tich-hop.md) — cách làm việc chung với mọi tích hợp
* [3.16. Đơn hàng](../../khoi-san-pham/don-hang.md) — nơi bấm xuất hoá đơn cho từng đơn
* [4.9. Cài đặt](../cai-dat.md) — tiền tệ và thông tin công ty hiện trên hoá đơn
