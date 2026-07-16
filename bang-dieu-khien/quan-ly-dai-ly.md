# 1.2. Quản lý đại lý

1.2.1. Danh sách đại lý 1.2.2. Quản lý hạng đại lý

1.2.3. Lịch sử nạp tiền

## Danh sách đại lý

![](../.gitbook/assets/pg015-0.png)

## Theo dõi các chỉ số tổng quan

- Tổng đại lý: Hiển thị số lượng đại lý đã chính thức trong hệ thống (hiện tại là 0).

- Tổng doanh số: Tổng số tiền giao dịch từ các đại lý.

- Tổng số dư: Tổng số tiền hiện có trong ví/tài khoản của các đại lý.

- Chờ duyệt: Số lượng yêu cầu đăng ký mới đang đợi bạn xử lý (hiện tại có 3 yêu cầu).

## Xử lý yêu cầu đăng ký đại lý mới

Tại mục "Yêu cầu đăng ký đại lý" (phần có nền màu vàng nhạt), bạn có danh sách các bên đang muốn gia nhập hệ thống.

- Xem thông tin: Bạn có thể kiểm tra Tên, Email, Số điện thoại và thông tin ngân hàng (như MB Bank của các đại lý Vietnamtravel) để xác minh danh tính.

- Phê duyệt (Nút xanh): Nhấn vào đây để chấp nhận đại lý. Sau khi nhấn, đại lý sẽ được chuyển xuống danh sách chính thức và có thể bắt đầu hoạt động.

- Từ chối (Nút đỏ dấu X): Nhấn vào đây nếu thông tin đăng ký không hợp lệ hoặc bạn không muốn hợp tác.

## Quản lý danh sách đại lý chính thức

Phần bảng bên dưới cùng (hiện đang trống) là nơi quản lý các đại lý đã được phê duyệt. Tại đây bạn có thể:

- Tìm kiếm/Lọc: Sử dụng ô "Tìm kiếm tên, email, SĐT..." hoặc lọc theo "Hạng đại lý" để nhanh chóng tìm thấy đối tác cần quản lý.

- Theo dõi chi tiết: Xem ID, hạng đại lý (Vàng, Bạc, Đồng...), doanh số riêng và số dư hiện tại của từng bên.

## Các tác vụ bổ sung (Góc trên bên phải)

- Thêm đại lý (+): Nhấn nút màu xanh dương để chủ động thêm mới một đại lý vào hệ thống mà không cần họ phải gửi yêu cầu đăng ký.

![](../.gitbook/assets/pg016-0.png)

- Xuất dữ liệu: Nhấn nút có biểu tượng tải xuống để trích xuất danh sách

![](../.gitbook/assets/pg016-1.png)

đại lý ra file (thường là Excel) phục vụ việc báo cáo hoặc lưu trữ nội bộ.

*📺 Video hướng dẫn: TourkitWeb | Hướng dẫn quản lý đại lý*

## Quản lý hạng đại lý

## Tổng quan giao diện Quản lý Hạng Đại lý

![](../.gitbook/assets/pg018-0.png)

Tại màn hình chính của mục này, bạn có thể theo dõi:

- Tổng hạng đại lý: Số lượng các cấp bậc bạn đã tạo (ví dụ: Đồng, Bạc, Vàng, Kim Cương).

- Đang hoạt động / Không hoạt động: Trạng thái của các hạng này trên hệ thống.

- Tổng user đại lý: Số lượng đối tác đang thuộc các hạng này.

## Cách thêm và thiết lập Hạng Đại lý mới

Khi bạn nhấn nút "+ Thêm Hạng Đại lý", hệ thống sẽ yêu cầu nhập các thông tin sau:

A. Thông tin cơ bản

- Tên đại lý: Đặt tên cho cấp độ (Ví dụ: Đại lý Cấp 1, Đại lý VIP...).

- Doanh số tối thiểu & tối đa: Đây là điều kiện để đại lý đạt được hạng này. ◦ Ví dụ: Hạng Bạc yêu cầu doanh số từ 10.000.000đ đến 50.000.000đ. Nếu để trống "Doanh số tối đa", hệ thống hiểu đây là hạng cao nhất.

- Ghi chú: Mô tả thêm về đặc quyền của hạng để đội ngũ quản trị dễ nắm bắt.

![](../.gitbook/assets/pg019-0.png)

B. Thiết lập Chiết khấu (Phần quan trọng nhất)

Hệ thống cho phép bạn tùy chỉnh mức hoa hồng/giảm giá cho đại lý theo từng loại dịch vụ:

- Các loại dịch vụ: Tour, Khách sạn, Vé máy bay, Sự kiện, Du thuyền.

- Cơ chế thiết lập: ◦ Mặc định (tất cả): Nhập con số chiết khấu chung cho toàn bộ hạng mục đó. ◦ Đơn vị: Bạn có thể chọn giữa Phần trăm (%) dựa trên giá gốc hoặc Số tiền cố định (VND) trên mỗi dịch vụ. ◦ Chiết khấu theo danh mục: Cho phép bạn chọn riêng từng tour hoặc khách sạn cụ thể để có mức chiết khấu khác với mức mặc định.

![](../.gitbook/assets/pg019-1.png)

## Các thao tác quản trị khác

- Nhập/Xuất: Dùng để đưa dữ liệu hạng đại lý từ file Excel vào hệ thống hoặc tải về để kiểm tra.

- Thao tác (Cột cuối cùng): Sau khi tạo xong, bạn có thể sửa (biểu tượng

![](../.gitbook/assets/pg020-0.png)

bút chì) hoặc xóa các hạng không còn sử dụng.

*📺 Video hướng dẫn: TourkitWeb | Hướng dẫn quản lý đại lý*

## Lịch sử nạp tiền

![](../.gitbook/assets/pg021-0.png)

## Theo dõi các chỉ số tài chính (Các thẻ phía trên)

- Tổng giao dịch: Tổng số lệnh nạp tiền đã phát sinh (bao gồm cả thành công, chờ duyệt và bị từ chối).

- Tổng tiền nạp: Tổng số tiền thực tế đã được cộng vào hệ thống (chỉ tính các lệnh đã xác nhận).

- Đang chờ duyệt: Số lượng giao dịch mà đại lý đã thông báo nạp nhưng bạn chưa kiểm tra tài khoản ngân hàng để xác nhận.

- Đã xác nhận: Số lượng giao dịch nạp tiền thành công.

## Bộ lọc và Tìm kiếm (Thanh công cụ)

Để quản lý danh sách hiệu quả khi số lượng giao dịch lớn, bạn có thể sử dụng:

- Bộ lọc trạng thái: Click nhanh vào các nút Tất cả, Đang chờ, Đã xác nhận, hoặc Đã từ chối để lọc danh sách.

- Ô tìm kiếm: Nhập tên đại lý hoặc email để kiểm tra lịch sử nạp tiền của một đối tác cụ thể.

## Quản lý chi tiết bảng giao dịch

Khi có dữ liệu, bảng này sẽ hiển thị các thông tin quan trọng:

- Số tiền nạp & Số dư: Xem số tiền họ nạp mỗi lần và số dư còn lại sau khi nạp.

- Mã CK (Mã chuyển khoản): Đây là thông tin quan trọng nhất để đối soát với lịch sử biến động số dư trên App ngân hàng của công ty.

- Ghi chú: Các nội dung đi kèm giao dịch (thường là cú pháp nạp tiền).

- Trạng thái: Cho biết lệnh đó là Thành công hay Thất bại.

- Hành động: Tại đây sẽ có các nút để bạn Phê duyệt (xác nhận đã nhận tiền) hoặc Hủy bỏ (nếu đại lý báo nạp ảo hoặc sai thông tin).

## Các tác vụ quan trọng khác

- Nút "Xuất" (Góc trên phải): Xuất toàn bộ lịch sử nạp tiền ra file Excel. Đây là tính năng cần thiết để làm báo cáo tài chính định kỳ hoặc đối soát với

![](../.gitbook/assets/pg022-0.png)

kế toán.

*📺 Video hướng dẫn: TourkitWeb | Hướng dẫn quản lý đại lý*
