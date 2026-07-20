# 3.6. Vé máy bay BGT

Mục **Vé máy bay BGT** cho phép website của bạn bán vé máy bay thật — khách tự tìm chuyến, chọn giờ bay và đặt vé ngay trên trang của bạn.

Điểm khác biệt quan trọng: giá vé và danh sách chuyến bay **không do bạn tự nhập tay**. Chúng được lấy tự động, theo thời gian thực, từ một nhà cung cấp dữ liệu vé máy bay bên ngoài tên là **AirData**. Việc của bạn ở đây chỉ là hai chuyện:

1. **Khai báo thông tin kết nối** để website nói chuyện được với AirData.
2. **Quyết định bạn cộng thêm bao nhiêu tiền** vào giá gốc để lấy lời.

> **Đường dẫn:** Menu bên trái > **Vé máy bay BGT**

Mục này gồm 4 phần:

* **Cài đặt API** — khai báo thông tin kết nối tới nhà cung cấp dữ liệu vé.
* **Cấu hình giá** — quy định mức cộng thêm / giảm giá cho từng hãng bay.
* **API Logs** — nhật ký: bản ghi lại mọi lần website hỏi dữ liệu vé, dùng khi cần tra lỗi.
* **Hướng dẫn** — tài liệu thao tác chi tiết ngay trong hệ thống.

> **Lưu ý:** "API" nghe rất kỹ thuật, nhưng bạn cứ hiểu đơn giản: đó là **đường dây nối** giữa website của bạn và kho dữ liệu vé máy bay của đối tác. Bạn không cần biết nó hoạt động ra sao — chỉ cần điền đúng thông tin mà đối tác cấp cho bạn.

> **Cẩn thận:** Toàn bộ thông tin trong phần **Cài đặt API** phải do **đơn vị cung cấp dịch vụ AirData gửi cho bạn**. Đừng tự đoán, đừng tự gõ đại. Điền sai thì website sẽ không tìm được chuyến bay nào.

## Cài đặt API

### a. Cấu hình API AirData

Đây là phần thiết lập kết nối cốt lõi. Không có phần này, mọi thứ còn lại đều vô nghĩa.

* **API Base URL** — địa chỉ kho dữ liệu của AirData. Hãy copy đúng nguyên văn từ email/tài liệu mà đối tác gửi.
* **API Token (Bearer)** — mã xác thực, giống như "chìa khóa" chứng minh website của bạn có quyền lấy dữ liệu. Khi bạn điền đúng, hệ thống sẽ hiện dòng chữ **"Đã có token"** màu xanh.

> **Cẩn thận:** Token là chuỗi ký tự rất dài. Khi copy dán, cực kỳ dễ bị **thiếu vài ký tự ở đầu/cuối** hoặc **dính dấu cách thừa**. Hãy bôi đen toàn bộ chuỗi rồi copy, và kiểm tra kỹ trước khi lưu.

![](../.gitbook/assets/pg098-0.png)

### b. Thông tin Agent (VN1A)

Phần này chỉ cần thiết cho các nghiệp vụ xử lý vé, đổi hành trình trên hệ thống **VN1A**.

* **Agency Code** — mã đại lý của bạn.
* **Pax Code (Customer Code)** — mã định danh khách hàng tương ứng.

> **Nếu bạn chỉ bán vé Vietjet (VJ):** bạn có thể **để trống cả hai ô này**, không ảnh hưởng gì.

![](../.gitbook/assets/pg098-1.png)

### c. Cấu hình đặt vé

Đây là các quy tắc cho quy trình khách đặt vé trên website:

**Thời gian hết hạn draft (phút)**

"Draft" ở đây nghĩa là **đơn đặt vé dang dở** — khách bấm đặt nhưng chưa thanh toán xong rồi bỏ đi. Ô này quy định sau bao nhiêu phút thì hệ thống tự hủy những đơn dang dở đó để trả chỗ lại. Mặc định là **30 phút**.

> **Mẹo:** Đừng để con số này quá lớn. Nếu đặt 300 phút, một khách bỏ ngang sẽ giữ chỗ suốt 5 tiếng và khách thật sự muốn mua sẽ không đặt được.

**Điều khoản & điều kiện**

* Tích chọn **"Bật điều khoản & điều kiện"** nếu bạn muốn khách **bắt buộc phải đồng ý** với quy định của bạn trước khi đặt vé.
* Sau khi bật, nhập nội dung chi tiết vào ô **"Nội dung điều khoản & điều kiện"**.

![](../.gitbook/assets/pg099-0.png)

### d. Kiểm tra và Lưu cài đặt

Điền xong chưa phải là xong. Bạn cần làm đủ 3 việc sau:

1. **Kiểm tra kết nối** — nhấn nút **"Kiểm tra kết nối API"** ở cuối trang. Hệ thống sẽ thử gọi sang AirData và báo lại cho bạn biết đã liên kết được hay chưa. **Hãy luôn làm bước này trước khi lưu.**
2. **Lưu cài đặt** — nhấn nút **"Lưu thay đổi"** ở khung bên phải.
3. **Xem lại trạng thái** — ô **"Trạng thái"** cho biết tính năng đang hoạt động hay không. Khi mọi thứ đã sẵn sàng, ô này hiện **"Đã kích hoạt"** màu xanh.

> **Nếu bấm "Kiểm tra kết nối API" mà báo lỗi:** đừng vội lưu. 9/10 trường hợp là do Base URL hoặc Token bị sai một ký tự, hoặc dính dấu cách thừa khi copy. Hãy xóa hết và dán lại cẩn thận. Nếu vẫn lỗi, hãy liên hệ đơn vị cung cấp AirData để xác nhận thông tin còn hiệu lực không.

![](../.gitbook/assets/pg099-1.png)

## Cấu hình giá

Đây là phần **quan trọng nhất với túi tiền của bạn**.

Giá lấy về từ AirData là **giá gốc**. Nếu bạn bán đúng giá gốc, bạn không lời đồng nào. Màn hình này là nơi bạn quy định: cộng thêm bao nhiêu vào giá gốc để ra **giá niêm yết** hiển thị cho khách.

{% embed url="https://youtu.be/xaPmo2PskeE?si=JjckJbshjYeyl-cQ" %}

### a. Thiết lập Tăng giá & Giảm giá

Tại mỗi hãng bay, bạn có hai cột để điều chỉnh:

**Cột "Tăng giá" (màu xanh)** — dùng để tạo ra **giá niêm yết**, tức là giá khách nhìn thấy. Đây là chỗ bạn cài phần lời hoặc phí dịch vụ của mình. Có 2 kiểu:

* **Loại %** — cộng thêm theo phần trăm giá gốc. Ví dụ đặt `10` thì vé gốc 1.000.000đ sẽ thành 1.100.000đ.
* **Loại VNĐ** — cộng thẳng một số tiền cố định. Ví dụ đặt `40000` thì vé nào cũng cộng thêm đúng 40.000đ.

**Cột "Giảm giá" (màu vàng)** — dùng để chạy khuyến mãi, giảm so với **giá niêm yết** vừa tính ở trên. Cũng có 2 kiểu:

* **Loại %** — giảm X% trên giá niêm yết.
* **Loại VNĐ** — trừ thẳng X đồng khỏi giá niêm yết.

> **Cẩn thận:** Hãy nhớ thứ tự — hệ thống **tăng giá trước, giảm giá sau**. Nếu bạn cộng thêm 10% rồi lại giảm 20%, kết quả là bạn đang **bán lỗ so với giá gốc**. Hãy tính kỹ trước khi lưu, hoặc thử với một chuyến bay cụ thể để xem con số cuối cùng ra bao nhiêu.

![](../.gitbook/assets/pg101-0.png)

### b. Các cấp độ cấu hình

Hệ thống cho phép bạn cài giá theo 2 cấp, để bạn không phải gõ đi gõ lại:

* **Mặc định (Tất cả hãng)** — dòng đầu tiên, **màu vàng nhạt**. Đây là mức áp dụng chung cho mọi hãng bay mà bạn chưa cài riêng. Cài một lần ở đây là xong cho tất cả.
* **Cấu hình theo từng hãng** — các dòng phía dưới (Galileo, Cebu Pacific, AirAsia…). Chỉ điền vào đây khi hãng đó có chính sách chiết khấu khác biệt, cần mức lời riêng.

> **Quy tắc để nhớ:** Ô nào **để trống** ở dòng của một hãng, hệ thống sẽ **tự lấy theo dòng mặc định**. Nên bạn chỉ cần điền ở những hãng thật sự khác biệt.

![](../.gitbook/assets/pg101-1.png)

### c. Các nút chức năng quan trọng

* **"Cập nhật danh sách hãng bay"** (nút xanh, **góc trên bên phải**) — nhấn khi bạn muốn lấy về danh sách hãng hàng không mới nhất từ đối tác. Nếu thấy thiếu một hãng nào đó trong bảng, hãy thử nút này trước tiên.
* **Nút "X"** (màu đỏ, **cuối mỗi dòng**) — xóa cấu hình riêng của hãng đó, đưa hãng đó quay về dùng mức mặc định. Nút này **không xóa hãng bay**, chỉ xóa mức giá riêng bạn đã cài.
* **"Lưu thay đổi"** (nút xanh lớn, **cột bên phải**) — **cực kỳ quan trọng**. Chỉnh xong bất kỳ con số nào, bạn **bắt buộc** phải nhấn nút này. Nếu đóng trang mà chưa lưu, mọi thứ bạn vừa gõ sẽ mất sạch và giá trên website vẫn y như cũ.

![](../.gitbook/assets/pg102-0.png)

## API Logs

**Logs** nghĩa là **nhật ký** — hệ thống ghi lại mọi lần website của bạn hỏi dữ liệu từ AirData: hỏi lúc nào, hỏi cái gì, đối tác trả lời ra sao.

Bạn không cần vào đây hàng ngày. Nhưng khi có sự cố — khách báo không tìm được chuyến bay, giá hiện sai — thì đây là nơi tìm nguyên nhân. Khi báo lỗi cho đơn vị kỹ thuật, việc bạn gửi kèm thông tin từ màn hình này sẽ giúp họ xử lý nhanh hơn rất nhiều.

### Bộ lọc tìm kiếm (phía trên)

Phần này giúp bạn tra cứu nhanh một giao dịch hoặc một lỗi cụ thể:

* **Mã đặt chỗ / PNR** — nhập mã đơn hàng hoặc mã PNR của hãng để tìm đúng nhật ký của một đơn. Đây là cách tìm nhanh nhất khi bạn đang xử lý khiếu nại của một khách cụ thể.
* **Endpoint** — lọc theo loại yêu cầu đã gửi đi. Ví dụ `/cheapest-fare` là các lượt tìm vé rẻ nhất.
* **Context** — lọc theo loại tác vụ: `SearchFlights` (tìm chuyến bay), `GetFlightDetail` (xem chi tiết chuyến bay), `GetCheapestFare` (tìm vé rẻ nhất).
* **Trạng thái** — lọc theo mã phản hồi. Bạn chỉ cần nhớ đơn giản: mã **200 là thành công**; mã bắt đầu bằng **4** hoặc **5** là **có lỗi**. Muốn xem có trục trặc gì không, hãy lọc theo các mã 4xx và 5xx.
* **Từ ngày** — chọn mốc thời gian bắt đầu, để không phải lục lại quá nhiều bản ghi cũ.
* **Nút kính lúp** — nhấn để chạy bộ lọc.
* **Nút dấu X** — xóa hết điều kiện lọc, đưa các ô về mặc định.

![](../.gitbook/assets/pg103-0.png)

## Hướng dẫn

Hệ thống có sẵn một trang hướng dẫn thao tác chi tiết dành riêng cho tính năng Vé máy bay BGT.

Để mở, bạn vào menu bên trái, nhấn vào **Vé máy bay BGT**, rồi chọn mục **Hướng dẫn** trong danh sách xổ xuống.

![](../.gitbook/assets/pg104-0.png)

![](../.gitbook/assets/pg104-1.png)

## Lưu ý & xử lý sự cố

**Website không tìm thấy chuyến bay nào:**

* Vào **Cài đặt API**, kiểm tra ô **"Trạng thái"** có đang là **"Đã kích hoạt"** màu xanh không.
* Nhấn **"Kiểm tra kết nối API"** để xem đường dây còn thông không.
* Nếu vẫn không được, mở **API Logs** và lọc theo mã lỗi 4xx/5xx để xem đối tác báo lỗi gì.

**Giá trên website vẫn là giá cũ sau khi sửa:** khả năng cao bạn quên nhấn **"Lưu thay đổi"** ở cột bên phải. Nếu chắc chắn đã lưu rồi, hãy tải lại trang bằng **Ctrl + F5** (giữ Ctrl rồi bấm F5) để trình duyệt lấy bản mới nhất.

**Thiếu một hãng bay trong bảng cấu hình giá:** nhấn nút **"Cập nhật danh sách hãng bay"** ở góc trên bên phải để đồng bộ lại.

**Khách đặt vé nhưng đơn tự biến mất:** đó là đơn dang dở đã quá **thời gian hết hạn draft** nên hệ thống tự hủy để trả chỗ. Nếu khách hay phàn nàn về việc này, bạn có thể tăng số phút trong phần **Cấu hình đặt vé** — nhưng đừng tăng quá nhiều.

**Không thấy mục này trong menu:** tính năng có thể chưa được bật trên website của bạn, hoặc tài khoản của bạn chưa được cấp quyền. Hãy liên hệ đơn vị triển khai hoặc quản trị viên.

## Xem thêm

* [3.8. Booking](booking.md) — nơi xem và xử lý các đơn vé máy bay khách đã đặt.
* [3.11. Chuyến bay](chuyen-bay.md) — module quản lý chuyến bay do bạn **tự khai báo tay**, khác với vé lấy tự động qua API ở trang này.
* [4.10. Tích hợp](../khoi-he-thong/tich-hop.md) — các kết nối khác với dịch vụ bên ngoài.
