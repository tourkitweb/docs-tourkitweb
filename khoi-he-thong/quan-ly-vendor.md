# 4.3. Quản lý Vendor

Trước hết, giải nghĩa từ khóa:

> **Vendor = nhà cung cấp.** Đó là **đối tác bán dịch vụ ngay trên website của bạn**, chứ không phải nhân viên của bạn.

Hình dung như một cái chợ: bạn là **chủ chợ**, còn Vendor là các **tiểu thương thuê sạp** trong chợ của bạn. Ví dụ một chủ khách sạn ở Đà Nẵng đăng ký tài khoản trên web của bạn, tự đăng phòng của họ lên, khách đặt phòng qua web của bạn. Khách sạn đó chính là một Vendor.

Mô hình này giải quyết vấn đề: bạn có website và có khách, nhưng không thể tự sở hữu hàng trăm khách sạn hay hàng nghìn tour. Vendor mang hàng đến bán, bạn thu phí hoặc hoa hồng.

Từ đó phát sinh 2 việc phải quản lý, và đó chính là nội dung của mục này:

1. **Vendor phải trả gì cho bạn** để được bán trên web (mua gói dịch vụ).
2. **Bạn phải trả lại gì cho Vendor** — vì khách trả tiền vào tài khoản của bạn, bạn giữ hộ, rồi trả lại phần của họ. Việc này gọi là **thanh toán (payout)**.

> **Đường dẫn:** Menu bên trái > **Hệ thống** > **Quản lý Vendor**

> **Lưu ý:** Tính năng này có thể chưa được bật trên website của bạn. Nếu không thấy mục này trong menu, hãy liên hệ đơn vị triển khai.

![](../.gitbook/assets/pg123-0.png)

## Nếu bạn không thấy mục "Quản lý Vendor"

Đây là chuyện **rất bình thường**, đừng nghĩ hệ thống bị lỗi. Có 3 khả năng:

**1. Website của bạn không chạy mô hình chợ.** Nếu bạn chỉ bán tour của chính công ty mình, bạn không cần Vendor. Tính năng này chỉ bật khi bạn thực sự có đối tác bán hàng trên web.

**2. Bạn thấy mục "Thanh toán" đứng riêng thay vì "Quản lý Vendor".** Đây là điểm rất hay gây bối rối, nên giải thích rõ:

* Nếu website **chưa bật** gói quản lý nâng cao, bạn sẽ thấy một mục tên **"Thanh toán"** đứng độc lập trong nhóm Hệ thống. Nó lo đúng một việc: trả tiền cho Vendor.
* Nếu website **đã bật** gói nâng cao, mục "Thanh toán" đó **biến mất khỏi vị trí cũ** và chui vào **bên trong "Quản lý Vendor"**, cùng với các mục về gói dịch vụ.

Nói cách khác: **hai mục này không bao giờ cùng xuất hiện.** Nếu hôm nay bạn thấy "Thanh toán" mà mai lại thấy "Quản lý Vendor", nghĩa là đơn vị triển khai vừa bật gói nâng cao cho bạn — không phải bạn làm mất mục nào cả.

**3. Vai trò của bạn chưa được cấp quyền.** Hãy liên hệ quản trị viên.

## Trong mục này có gì?

Khi mục **"Quản lý Vendor"** được bật, bên trong thường gồm các phần sau:

* **Gói dịch vụ** — các "gói cước" bạn bán cho Vendor. Ví dụ: gói cho đăng 5 khách sạn/tháng, gói cho đăng không giới hạn.
* **Yêu cầu mua gói** — hàng chờ các Vendor đăng ký mua gói, chờ bạn duyệt.
* **Thanh toán Vendor** — danh sách các yêu cầu đòi tiền từ Vendor. Đây là phần bạn dùng nhiều nhất, mô tả kỹ bên dưới.
* **Cài đặt** — các thiết lập chung cho mô hình Vendor.

> **Lưu ý:** Danh sách "các Vendor của bạn là ai" **không nằm ở đây**. Vendor bản chất vẫn là người dùng, nên bạn quản lý họ tại [**4.1. Người dùng**](nguoi-dung.md) **> Tất cả người dùng**, rồi lọc theo vai trò **Vendor**.

## Gói dịch vụ và Yêu cầu mua gói

**Gói dịch vụ** là thứ bạn bán cho Vendor để họ được quyền đăng dịch vụ lên web của bạn — giống như bạn cho thuê sạp trong chợ, sạp to trả nhiều tiền hơn sạp nhỏ.

Bạn tạo trước các gói (tên gói, giá, được đăng bao nhiêu dịch vụ, thời hạn bao lâu). Vendor vào xem và đăng ký mua.

**Yêu cầu mua gói** là **hàng chờ**: Vendor đã bấm mua, đang chờ bạn xác nhận. Bạn vào đây xem và duyệt.

> **Nên xử lý sớm:** Vendor đang chờ bạn duyệt để bắt đầu đăng hàng và mang doanh thu về. Để hàng chờ tồn đọng là bạn đang tự làm chậm việc kinh doanh của mình.

## Thanh toán cho Vendor — phần bạn dùng nhiều nhất

### Hiểu dòng tiền trước đã

Đây là chỗ nhiều người mới nhầm, nên nói thật chậm:

1. Khách đặt phòng của Vendor trên website của bạn.
2. **Khách trả tiền vào tài khoản của BẠN**, không phải của Vendor.
3. Bạn giữ số tiền đó, giữ lại phần hoa hồng của mình.
4. Vendor muốn lấy phần của họ, họ **gửi một yêu cầu thanh toán** trong hệ thống.
5. Bạn xem yêu cầu, chuyển khoản thật ngoài đời, rồi **vào hệ thống đánh dấu là đã trả**.

> **Điểm cực kỳ quan trọng:** Hệ thống **không tự chuyển tiền** cho Vendor. Nó chỉ là **sổ ghi chép**. Việc chuyển khoản thật bạn vẫn phải làm qua ngân hàng như bình thường. Đổi trạng thái trong hệ thống chỉ là ghi lại rằng bạn đã trả. Đừng đánh dấu "đã trả" khi chưa thật sự chuyển khoản — sổ sách sẽ sai và bạn sẽ không biết mình còn nợ ai.

### Con số bên cạnh chữ "Thanh toán" nghĩa là gì?

Nếu thấy một **con số** hiện cạnh mục thanh toán, đó là **số yêu cầu thanh toán đang chờ bạn xử lý** — tức là số Vendor đang chờ tiền của bạn. Không phải tổng số tiền, không phải tổng số yêu cầu từ trước tới nay.

Số đó khác 0 nghĩa là **có người đang chờ bạn**. Số đó về 0 nghĩa là bạn đã xử lý hết.

### Bảng danh sách yêu cầu thanh toán có gì?

Mỗi dòng là một yêu cầu đòi tiền, với các cột:

* **ID** — mã số của yêu cầu, dùng để đối chiếu khi trao đổi với Vendor.
* **Vendor** — ai đang đòi tiền.
* **Ghi chú** — có 2 loại: ghi chú Vendor gửi cho bạn, và ghi chú bạn gửi lại cho Vendor.
* **Số tiền (Amount)** — số tiền họ yêu cầu.
* **Phương thức thanh toán (Payout Method)** — họ muốn nhận tiền bằng cách nào (chuyển khoản ngân hàng, ví điện tử…).
* **Ngày tạo** — lúc họ gửi yêu cầu.
* **Trạng thái (Status)** — yêu cầu này đang ở bước nào. Đọc kỹ phần dưới.

### 4 trạng thái của một yêu cầu thanh toán

Hãy hiểu 4 trạng thái này như 4 chặng của một quy trình:

* **Initial** (Mới gửi) — Vendor vừa gửi yêu cầu, **bạn chưa xem gì cả**. Đây chính là những cái được đếm vào con số cạnh menu. Đây là việc của bạn.
* **Confirmed** (Đã xác nhận) — bạn đã kiểm tra và đồng ý là số tiền này đúng, **nhưng chưa chuyển khoản**. Giống như "đã duyệt chi, đang chờ kế toán chuyển".
* **Paid** (Đã trả) — **tiền đã ra khỏi tài khoản của bạn**, việc xong. Chỉ đổi sang trạng thái này **sau khi đã chuyển khoản thật**.
* **Rejected** (Từ chối) — bạn không đồng ý trả yêu cầu này. Ví dụ số tiền sai, hoặc đơn hàng đó khách đã hủy.

### Cách xử lý một yêu cầu thanh toán

Việc duyệt được làm theo kiểu **hành động hàng loạt** — tức là chọn nhiều yêu cầu rồi xử lý cùng lúc:

**Bước 1: Kiểm tra trước khi làm gì cả.** Đối chiếu số tiền Vendor yêu cầu với đơn hàng thực tế. Bước này không có nút bấm, nhưng là bước quan trọng nhất — nhầm ở đây là mất tiền thật.

**Bước 2: Tích chọn** các yêu cầu bạn muốn xử lý ở cột bên trái.

**Bước 3: Mở hộp thoại xử lý.** Một cửa sổ hiện ra để bạn điền:

* **Trạng thái (Status)** — chọn một trong 4 trạng thái ở trên.
* **Ngày thanh toán (Pay date)** — ngày bạn chuyển khoản thật. Điền đúng ngày để sau này đối chiếu sổ ngân hàng.
* **Ghi chú gửi Vendor (Note to vendor)** — lời nhắn cho Vendor. **Đặc biệt quan trọng khi bạn từ chối**: hãy viết rõ lý do, ví dụ _"Đơn #123 khách đã hủy nên không tính hoa hồng"_. Vendor sẽ nhận được lời nhắn này.

**Bước 4: Nhấn nút áp dụng** để lưu lại. **Không nhấn nút này thì không có gì xảy ra.**

> **Hệ thống sẽ tự gửi email cho Vendor** khi bạn đổi trạng thái hoặc từ chối yêu cầu. Nghĩa là: những gì bạn gõ trong ô ghi chú, Vendor sẽ đọc được. Hãy viết lịch sự, rõ ràng, đúng chính tả — đây là email đại diện cho công ty bạn.

> **Cẩn thận:** Đừng chọn tất cả rồi đánh dấu **"Paid"** cho nhanh. Mỗi dòng là tiền thật. Đánh dấu đã trả mà chưa chuyển khoản thì bạn sẽ quên mất khoản nợ đó, và Vendor sẽ gọi điện đòi. Ngược lại, hãy chuyển khoản xong rồi mới vào đánh dấu.

## Lưu ý & xử lý sự cố

**Tôi tìm mãi không thấy danh sách các Vendor của mình ở đâu.** Vì nó không nằm trong mục này. Vào [**4.1. Người dùng**](nguoi-dung.md) **> Tất cả người dùng**, rồi lọc theo vai trò **Vendor**.

**Hôm trước tôi thấy mục "Thanh toán" riêng, giờ không thấy nữa.** Không phải bạn làm mất. Website vừa được bật gói quản lý nâng cao, nên mục "Thanh toán" đã chuyển vào bên trong **"Quản lý Vendor"**. Xem lại phần đầu bài.

**Vendor báo họ đã gửi yêu cầu mà tôi không thấy.** Kiểm tra bộ lọc trạng thái — có thể bạn đang xem trạng thái khác. Hãy xem ở trạng thái **"Initial"** (Mới gửi). Nếu vẫn không có, nhấn **Ctrl + F5** để tải lại trang.

**Tôi lỡ đánh dấu "Paid" nhưng thực tế chưa chuyển tiền.** Chọn lại yêu cầu đó và đổi trạng thái về **"Confirmed"**. Nhưng lưu ý: **Vendor có thể đã nhận email báo đã trả tiền rồi**. Hãy chủ động nhắn cho họ giải thích, đừng để họ tưởng bạn nợ mà không trả.

**Tôi từ chối nhầm một yêu cầu.** Chọn lại và đổi trạng thái về **"Confirmed"** hoặc **"Initial"**. Vendor đã nhận email từ chối, nên hãy nhắn giải thích cho họ.

**Con số cạnh mục thanh toán không giảm dù tôi đã xử lý.** Tải lại trang bằng **Ctrl + F5**. Con số chỉ cập nhật khi trang được nạp mới.

> **Mẹo quản lý:** Hãy đặt lịch cố định — ví dụ **thứ Sáu hằng tuần** — để vào xử lý toàn bộ yêu cầu thanh toán một lượt. Vendor biết trước lịch thì họ không sốt ruột gọi điện, còn bạn thì không bị việc này cắt ngang mỗi ngày.

## Xem thêm

* [4. Khối HỆ THỐNG](./)
* [4.1. Người dùng](nguoi-dung.md)
* [4.4. Kết nối khách sạn](ket-noi-khach-san.md)
