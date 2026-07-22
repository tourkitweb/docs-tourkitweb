# 1.3. Quản lý Affiliate

## 1.3. Quản lý Affiliate

Cách hoạt động của tính năng này rất đơn giản:

1. Một người đăng ký làm **cộng tác viên (CTV)** trên website của bạn.
2. Họ nhận được một **đường link riêng** để chia sẻ lên Facebook, Zalo, blog…
3. Khách nào bấm vào link đó rồi đặt dịch vụ và **trả tiền thành công** → CTV được hưởng hoa hồng.
4. CTV tích lũy đủ tiền thì gửi yêu cầu rút, bạn chuyển khoản cho họ.

Điểm khác với đại lý: CTV **không cần nạp tiền trước**, không cần vốn, chỉ cần chia sẻ link. Đây là cách mở rộng bán hàng nhẹ nhàng nhất — bạn chỉ trả tiền khi đã thực sự có doanh thu.

![](../.gitbook/assets/pg023-0.png)

> **Lưu ý:** Tính năng này có thể chưa được bật trên website của bạn. Nếu không thấy mục này trong menu, hãy liên hệ đơn vị triển khai. Menu cũng hiển thị theo phân quyền — nếu đồng nghiệp thấy mà bạn không thấy, tài khoản của bạn chưa được cấp quyền.

Trang này chia làm **hai phần**, dành cho hai đối tượng khác nhau:

* **Phần A — Dành cho CTV**: hướng dẫn người đi giới thiệu. Bạn có thể copy phần này gửi cho CTV của mình.
* **Phần B — Dành cho quản trị viên (QTV)**: hướng dẫn bạn — người vận hành chương trình.

***

## Phần A — Hướng dẫn cho Cộng tác viên (CTV)

### a. Đăng ký tham gia

Trước khi kiếm được đồng hoa hồng nào, bạn phải được admin duyệt cho vào chương trình.

**Bước 1:** Đăng nhập tài khoản người dùng trên website. Nếu chưa có tài khoản, hãy đăng ký một tài khoản thường trước.

**Bước 2:** Vào **Tài khoản** → **Affiliate**.

**Bước 3:** Điền **lý do tham gia** (không bắt buộc, nhưng nên viết vài dòng), rồi nhấn nút **"Đăng ký ngay"**.

> **Mẹo được duyệt nhanh:** admin đọc lý do tham gia để quyết định. Đừng để trống hoặc gõ "abc". Hãy viết ngắn gọn bạn sẽ giới thiệu ở đâu, ví dụ: _"Mình quản trị nhóm Facebook Phượt Miền Bắc 20.000 thành viên, muốn giới thiệu tour cho các bạn trong nhóm."_ Câu này khiến bạn nổi bật hơn hẳn.

**Bước 4:** Chờ admin duyệt. Sau khi được duyệt, bạn nhận **mã giới thiệu riêng** (ví dụ: `affABCD12`). Mã này là danh tính của bạn trong hệ thống — mọi hoa hồng đều được tính dựa trên nó.

### b. Tạo link giới thiệu

Được duyệt rồi, giờ bạn cần link để chia sẻ.

Vào **Dashboard** → **Quản lý link**, rồi làm 3 bước:

**Bước 1:** Mở trang tour hoặc khách sạn bạn muốn quảng bá, copy địa chỉ trên thanh trình duyệt và **dán URL** đó vào ô.

**Bước 2:** Nhấn **"Tạo link"**. Hệ thống trả về một **link ngắn** dạng `/go/abc1234`.

**Bước 3:** Chia sẻ link ngắn này lên mạng xã hội, Zalo, blog…

![](../.gitbook/assets/pg024-0.png)

> **Cẩn thận — sai lầm khiến bạn mất trắng hoa hồng:** phải chia sẻ **đúng link ngắn** hệ thống tạo ra. Nếu bạn tiện tay copy địa chỉ tour từ thanh trình duyệt rồi gửi cho khách, link đó **không mang mã giới thiệu của bạn** — khách có đặt tour thì bạn cũng không được đồng nào. Hãy luôn quay lại Quản lý link để lấy đúng link ngắn.
>
> **Mẹo:** hãy tự bấm thử link mình vừa tạo xem nó có mở đúng trang tour không, trước khi đăng cho hàng nghìn người xem.

### c. Theo dõi hoa hồng

* Khi khách bấm vào link của bạn, hệ thống **ghi nhận trong 30 ngày**. Nghĩa là khách bấm hôm nay, đắn đo cả tháng rồi mới đặt — bạn vẫn được tính hoa hồng.
* Nếu khách đặt và **hoàn tất thanh toán** trong thời gian đó → hoa hồng được tạo tự động, bạn không cần báo cho ai.
* Xem toàn bộ hoa hồng của mình tại **Dashboard** → **Hoa hồng**.

**Hai điều cần nhớ rõ:**

* **Booking chưa thanh toán thì chưa tính hoa hồng.** Khách mới đặt chỗ mà chưa trả tiền thì bạn chưa có gì. Phải đợi tiền về.
* **Bạn không nhận hoa hồng khi tự đặt cho chính mình.** Hệ thống nhận ra điều này. Đừng mất công thử.

![](../.gitbook/assets/pg025-0.png)

> **Vì sao hoa hồng chưa hiện dù khách đã đặt?** Ba lý do theo thứ tự phổ biến: (1) khách chưa thanh toán xong; (2) khách bấm link của bạn nhưng lại đặt trên một trình duyệt/thiết bị khác nên hệ thống mất dấu; (3) đã quá 30 ngày kể từ lúc khách bấm link.

### d. Rút tiền

**Bước 1 — Khai báo tài khoản nhận tiền.** Vào **Dashboard** → **Tài khoản ngân hàng** → **Thêm tài khoản nhận tiền**.

![](../.gitbook/assets/pg025-1.png)

> **Cẩn thận:** hãy kiểm tra số tài khoản **hai lần** trước khi lưu. Gõ sai một chữ số là tiền chuyển nhầm người, và lấy lại rất khó khăn. Tên chủ tài khoản phải viết **không dấu, in hoa**, đúng như trên thẻ ngân hàng.

**Bước 2 — Gửi yêu cầu rút.** Vào **Dashboard** → **Rút tiền** → nhập số tiền muốn rút (**tối thiểu 100.000₫**).

![](../.gitbook/assets/pg026-0.png)

**Bước 3 — Chờ xử lý.** Gửi yêu cầu xong, admin sẽ kiểm tra và chuyển khoản cho bạn. Việc này thường mất vài ngày làm việc, không phải ngay lập tức.

**Hai khái niệm về tiền bạn cần hiểu:**

* **Tiền đang giữ** — Khi bạn gửi yêu cầu rút, số tiền đó bị **đóng băng tạm thời**. Bạn không rút thêm phần đó được nữa cho tới khi yêu cầu được xử lý xong. Cơ chế này để tránh việc bạn vô tình gửi hai yêu cầu rút cùng một khoản tiền.
* **Số dư khả dụng = Tổng ví − Tiền đang giữ.** Đây mới là số tiền bạn **thực sự có thể rút** lúc này.

> **Vì sao ví hiện 2 triệu mà không rút được 2 triệu?** Vì một phần đang là **Tiền đang giữ** từ một yêu cầu rút trước đó bạn chưa nhớ ra. Hãy nhìn con số **Số dư khả dụng**, đó mới là con số thật.

***

## Phần B — Hướng dẫn cho Quản trị viên (QTV)

Đây là phần dành cho bạn — người vận hành chương trình. Có 4 việc, làm theo đúng thứ tự.

### Bước 1: Thiết lập ban đầu

> Phần này chỉ làm **một lần** trước khi chạy chương trình. Sau đó bạn hầu như không cần quay lại.

#### 1a. Cài đặt chung

Vào **Admin** → **Affiliate** → **Cài đặt**.

Có hai thiết lập cần quan tâm:

| Cài đặt                   | Mặc định    | Ý nghĩa                                                                                                                                          |
| ------------------------- | ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Thời hạn tracking**     | 30 ngày     | Sau khi khách click link, hệ thống ghi nhận trong bao nhiêu ngày. Khách đặt trong khoảng thời gian này thì CTV nhận hoa hồng. Quá hạn thì không. |
| **Số tiền rút tối thiểu** | 100.000 VND | CTV phải tích lũy đạt mức này mới được gửi yêu cầu rút tiền.                                                                                     |

![](../.gitbook/assets/pg027-0.png)

> **Nên đặt Thời hạn tracking bao nhiêu?** Cân nhắc theo loại hàng bạn bán. Tour giá trị lớn khách thường đắn đo hàng tháng — để 30 ngày hoặc dài hơn thì công bằng với CTV. Để quá ngắn (7 ngày chẳng hạn) sẽ khiến CTV mất hoa hồng oan và họ sẽ bỏ chương trình của bạn.
>
> **Vì sao cần Số tiền rút tối thiểu?** Nếu để 0đ, sẽ có người rút 5.000đ. Mỗi lệnh rút bạn đều tốn công chuyển khoản và đối soát thủ công. Mức tối thiểu giúp gom lại, đỡ tốn công cho cả hai bên.

#### 1b. Cấu hình hoa hồng

Vào **Admin** → **Affiliate** → **Cấu hình hoa hồng** → **Thêm mới**.

Đây là nơi bạn quyết định trả cho CTV bao nhiêu. Bạn có thể đặt nhiều cấu hình cùng lúc, và hệ thống **áp dụng theo thứ tự ưu tiên** — cái nào cụ thể hơn thì thắng:

1. **Danh mục cụ thể** (ví dụ: Tour miền Bắc) — **ưu tiên cao nhất**.
2. **Loại dịch vụ** (ví dụ: tất cả Tour) — ưu tiên vừa.
3. **Mặc định chung** — áp dụng khi không có cấu hình nào ở trên khớp.

Hãy xem bảng ví dụ để hiểu rõ cách các mức chồng lên nhau:

| Loại dịch vụ | Danh mục      | Hoa hồng             | Kết quả thực tế                                      |
| ------------ | ------------- | -------------------- | ---------------------------------------------------- |
| (để trống)   | (để trống)    | 5%                   | Mặc định: mọi dịch vụ không khớp gì khác đều được 5% |
| Tour         | (để trống)    | 8%                   | Tất cả tour được 8% (đè lên mức mặc định 5%)         |
| Tour         | Tour miền Bắc | 10%                  | Riêng tour miền Bắc được 10% (đè lên cả mức 8%)      |
| Khách sạn    | (để trống)    | 50.000 VND (cố định) | Mỗi booking khách sạn trả cố định 50.000đ            |

![](../.gitbook/assets/pg028-0.png)

> **Cách đọc bảng trên:** một tour miền Bắc khớp cả 3 dòng đầu, nhưng hệ thống chọn dòng **cụ thể nhất** → CTV được 10%. Một tour miền Nam chỉ khớp dòng 1 và 2 → được 8%. Một vé máy bay không khớp dòng nào riêng → được 5% theo mặc định.
>
> **Cẩn thận:** hãy **luôn tạo một dòng Mặc định chung**. Nếu không, các dịch vụ không có cấu hình riêng sẽ không sinh hoa hồng, và CTV sẽ tưởng hệ thống bị lỗi.
>
> **Mẹo:** dùng **số tiền cố định** cho các dịch vụ có giá dao động mạnh. Khách sạn 5 sao và nhà nghỉ bình dân chênh nhau chục lần — trả % sẽ khiến CTV chỉ chăm chăm đẩy hàng đắt tiền.

### Bước 2: Duyệt đơn đăng ký CTV

Vào **Admin** → **Affiliate** → **Danh sách Affiliate**.

Đây là nơi bạn quyết định ai được vào chương trình. Mỗi CTV có một trong bốn trạng thái:

| Trạng thái         | Ý nghĩa                                                                      |
| ------------------ | ---------------------------------------------------------------------------- |
| **Chờ duyệt**      | Người dùng vừa đăng ký, chưa được tạo link. Đây là những người đang đợi bạn. |
| **Đang hoạt động** | Được phép tạo link và nhận hoa hồng bình thường.                             |
| **Từ chối**        | Không được tham gia chương trình.                                            |
| **Tạm khóa**       | Vi phạm — bị tạm dừng, nhưng dữ liệu cũ vẫn giữ nguyên.                      |

**Các thao tác:**

* Nhấn **"Duyệt"** → CTV được kích hoạt ngay lập tức và nhận mã ref riêng.
* Nhấn **"Từ chối"** → nhập lý do → CTV không được tham gia.
* **Duyệt/từ chối hàng loạt:** tích chọn nhiều dòng → chọn hành động.

> **Nên duyệt ai?** Đọc phần lý do tham gia họ viết. Người có kênh thật (nhóm Facebook, blog, TikTok đang chạy) là người đáng duyệt. Người để trống lý do hoặc gõ vài ký tự vô nghĩa thường đăng ký cho vui, duyệt cũng không mang lại đơn nào.
>
> **Nên dùng "Tạm khóa" hay "Từ chối"?** Nếu CTV đã hoạt động rồi mà có dấu hiệu gian lận, hãy dùng **"Tạm khóa"** — thao tác này dừng họ lại nhưng **giữ nguyên dữ liệu cũ** để bạn điều tra. **"Từ chối"** dành cho người mới đăng ký mà bạn không muốn nhận.

### Bước 3: Duyệt hoa hồng

Vào **Admin** → **Affiliate** → **Hoa hồng**.

Hoa hồng được **tạo tự động** khi booking chuyển sang trạng thái **Đã thanh toán** / **Đã xác nhận** / **Hoàn thành**. Nhưng tạo ra chưa phải là trả — **admin cần duyệt thì tiền mới vào ví CTV**.

Đây là chốt chặn quan trọng: nó cho bạn cơ hội kiểm tra trước khi tiền đi ra.

| Trạng thái    | Ý nghĩa                                                           |
| ------------- | ----------------------------------------------------------------- |
| **Chờ duyệt** | Chưa cộng tiền vào ví CTV. Đang đợi bạn.                          |
| **Đã duyệt**  | Đã cộng tiền vào ví CTV.                                          |
| **Từ chối**   | Không cộng tiền (ví dụ: booking bị hủy, hoặc phát hiện gian lận). |

**Các thao tác:**

* **Duyệt** — Tiền hoa hồng cộng ngay vào ví CTV.
* **Từ chối** — Nhập lý do, tiền không được cộng.
* **Duyệt hàng loạt** — Tích chọn nhiều dòng → chọn **"Duyệt hàng loạt"**.
* **Xử lý ngay** — Chạy lại việc kiểm tra hoa hồng cho các booking chưa xử lý. Dùng khi có sự cố, ví dụ CTV báo booking đã thanh toán xong mà hoa hồng không tự hiện ra.

> **Cẩn thận — đừng duyệt hàng loạt một cách mù quáng.** Trước khi tích chọn cả trang và bấm duyệt, hãy lướt qua xem có dòng nào bất thường: một CTV bỗng dưng có hàng chục hoa hồng trong một ngày, hoặc các booking có tên khách trùng nhau. Đó là dấu hiệu tự đặt hàng để ăn hoa hồng.
>
> **Khi nào nên Từ chối?** Rõ nhất là khi **booking đã bị hủy sau khi thanh toán** — khách đã lấy tiền về, bạn không có doanh thu thì không thể trả hoa hồng. Luôn nhập lý do rõ ràng để CTV hiểu và không thắc mắc.

### Bước 4: Xử lý yêu cầu rút tiền

Vào **Admin** → **Affiliate** → **Yêu cầu rút tiền**.

Đây là bước tiền thật rời khỏi tài khoản của bạn, nên hãy làm cẩn thận.

**Quy trình xử lý:**

1. **Xem thông tin ngân hàng của CTV** — tên ngân hàng, số tài khoản, chủ tài khoản, chi nhánh.
2. **Chuyển khoản thực tế** theo đúng thông tin đó, bằng app ngân hàng của công ty.
3. **Quay lại hệ thống** → nhấn **"Xác nhận đã thanh toán"** → nhập **mã giao dịch ngân hàng** → nhấn **"Lưu"**.

**Nếu từ chối:** nhấn **"Từ chối"** → nhập lý do → **tiền tự động trả lại ví CTV**. Bạn không phải làm gì thêm, CTV có thể gửi yêu cầu mới.

| Trạng thái        | Ý nghĩa                                                 |
| ----------------- | ------------------------------------------------------- |
| **Đang chờ**      | CTV đã gửi yêu cầu, tiền đang bị đóng băng trong ví họ. |
| **Đã thanh toán** | Bạn đã chuyển khoản và xác nhận xong.                   |
| **Từ chối**       | Không thực hiện, tiền được trả lại ví CTV.              |

> **Quan trọng — đừng bỏ qua bước nhập mã giao dịch.** Đây là bằng chứng bạn đã chuyển tiền. Sau này nếu CTV khiếu nại "chưa nhận được tiền", mã này là thứ duy nhất giúp bạn tra ra lệnh chuyển trong sao kê ngân hàng. Bỏ trống nó là tự chuốc rắc rối cho mình sáu tháng sau.
>
> **Cẩn thận về thứ tự:** hãy **chuyển khoản trước, bấm xác nhận sau**. Nếu bấm xác nhận trước rồi quên chuyển, hệ thống ghi là đã trả, CTV không nhận được tiền và bạn sẽ mất rất nhiều thời gian đối soát để tìm ra lỗi.

### Lưu ý & xử lý sự cố

**CTV khiếu nại "khách đặt qua link của em mà không có hoa hồng".** Kiểm tra lần lượt:

* Khách đã **thanh toán xong** chưa? Booking chưa thanh toán thì chưa sinh hoa hồng.
* Có quá **Thời hạn tracking** (mặc định 30 ngày) kể từ lúc khách bấm link không?
* CTV có **tự đặt cho chính mình** không? Trường hợp này hệ thống không tính.
* Khách có bấm link trên máy này nhưng lại đặt trên máy/trình duyệt khác không? Khi đó hệ thống mất dấu và không có cách nào khôi phục.
* Thử nút **"Xử lý ngay"** ở mục Hoa hồng để hệ thống quét lại các booking chưa xử lý.

**Hoa hồng tính ra số lạ, không giống mức bạn nghĩ.** Nhớ lại thứ tự ưu tiên: **Danh mục cụ thể > Loại dịch vụ > Mặc định chung**. Rất có thể dịch vụ đó đang khớp một cấu hình theo danh mục mà bạn quên mất là mình đã tạo. Hãy vào **Cấu hình hoa hồng** và rà lại từ dòng cụ thể nhất.

**Nghi ngờ CTV gian lận (tự đặt, dùng nhiều tài khoản ảo).** Đừng xóa tài khoản họ. Hãy chuyển sang **"Tạm khóa"** để giữ lại toàn bộ dữ liệu làm bằng chứng, đồng thời **Từ chối** các hoa hồng đáng ngờ kèm lý do rõ ràng.

**CTV không rút được tiền dù ví còn số dư.** Hai nguyên nhân: (1) chưa đạt **Số tiền rút tối thiểu**; (2) một phần đang là **Tiền đang giữ** từ yêu cầu rút trước đó. Hãy bảo họ nhìn con số **Số dư khả dụng**, không phải Tổng ví.

**Link giới thiệu bấm vào báo lỗi hoặc mở nhầm trang.** Có thể tour/khách sạn đích đã bị gỡ khỏi website hoặc đổi đường dẫn. Bảo CTV tạo lại link mới từ địa chỉ hiện tại của trang.

**Duyệt CTV xong nhưng họ báo vẫn không tạo được link.** Bảo họ đăng xuất rồi đăng nhập lại, hoặc nhấn **Ctrl + F5**. Trạng thái mới đôi khi cần tải lại trang mới hiện ra.

### Xem thêm

* [1. Bảng điều khiển](./) — theo dõi doanh thu tổng để cân đối với chi phí hoa hồng.
* [1.2. Quản lý đại lý](quan-ly-dai-ly.md) — mô hình đối tác nạp tiền trước, phù hợp với đơn vị chuyên nghiệp hơn.
* [1.1. Mã giảm giá](ma-giam-gia.md) — kết hợp mã giảm giá với chiến dịch affiliate để tăng tỷ lệ chốt đơn.
