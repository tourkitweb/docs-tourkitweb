# 3.16. Đơn hàng

Đây là nơi bạn xem và xử lý **tất cả các đơn khách đã đặt** trên website: đơn đặt tour, đặt phòng khách sạn, thuê xe... Mỗi lần có khách đặt dịch vụ, một đơn hàng mới sẽ tự động xuất hiện tại đây.

Đây là màn hình bạn sẽ mở ra **mỗi ngày** để biết hôm nay có bao nhiêu khách mới và ai đang chờ mình xử lý.

> **Đường dẫn:** Menu bên trái > **Đơn hàng**
>
> Địa chỉ trực tiếp: `/admin/module/order`

> **Lưu ý:** Nếu bạn không thấy mục này trong menu, tài khoản của bạn chưa được cấp quyền xem đơn hàng (`order_view`) — hãy liên hệ quản trị viên.

## Phân biệt "Đơn hàng" và "Quản lý đơn hàng"

Hệ thống có 2 mục nghe rất giống nhau, người mới cực kỳ dễ nhầm:

| Mục | Nội dung |
|---|---|
| **Đơn hàng** (bài này) | Đơn hàng tổng thể — phần tiền bạc, thanh toán, trạng thái xử lý |
| **[Quản lý đơn hàng](booking.md)** | Chi tiết từng lượt đặt dịch vụ — khách nào, đi ngày nào, dịch vụ gì |

Hiểu nôm na: **Đơn hàng** giống tờ hóa đơn của cả giỏ hàng, còn **Quản lý đơn hàng** là từng món trong giỏ đó.

> 📷 *[Cần chụp màn hình: trang danh sách Đơn hàng tại Menu bên trái > Đơn hàng]*

## Bảy trạng thái của một đơn hàng

Đây là phần quan trọng nhất cần nắm. Mỗi đơn luôn ở **một trong 7 trạng thái**, cho bạn biết đơn đó đang ở đâu trong quy trình:

| Trạng thái | Nhãn trên màn hình | Nghĩa là gì |
|---|---|---|
| Bản nháp | **Draft** | Đơn chưa hoàn tất, khách bỏ dở giữa chừng. Chưa cần xử lý. |
| Tạm giữ | **On-hold** | Đơn đang bị giữ lại chờ điều gì đó — thường là chờ khách chuyển khoản. |
| Đang xử lý | **Processing** | Bạn đã nhận đơn và đang làm — đặt phòng, xác nhận chỗ với đối tác. |
| Hoàn thành | **Completed** | Xong xuôi, khách đã đi và đã trả tiền đầy đủ. Đây là đích đến. |
| Đã hủy | **Cancelled** | Đơn bị hủy — khách đổi ý hoặc bạn không đáp ứng được. |
| Thất bại | **Failed** | Đơn lỗi, thường do thanh toán không thành công. |
| Đã hoàn tiền | **Refunded** | Đơn đã hủy và bạn đã trả lại tiền cho khách. |

> **Chỉ đơn ở trạng thái "Completed" mới được tính vào doanh thu** trong các báo cáo. Nếu cuối tháng bạn thấy báo cáo doanh thu thấp hơn thực tế, nguyên nhân thường là còn nhiều đơn đã đi rồi nhưng **quên chuyển sang Completed**.

## Quy trình xử lý một đơn bình thường

Một đơn hàng thuận lợi sẽ đi qua các bước:

1. **Khách đặt trên website** → đơn tự động xuất hiện với trạng thái chờ xử lý.
2. **Bạn kiểm tra đơn** → xem khách đặt gì, đã trả tiền chưa.
3. **Khách thanh toán** → bạn chuyển đơn sang **Processing**.
4. **Bạn xác nhận dịch vụ** → đặt chỗ với đối tác, gửi xác nhận cho khách.
5. **Khách đã sử dụng dịch vụ xong** → bạn chuyển đơn sang **Completed**.

## Xem và sửa một đơn hàng

**Bước 1:** Tại danh sách, tìm đơn cần xử lý rồi nhấn nút **"Chỉnh sửa"** ở dòng đơn đó.

**Bước 2:** Màn hình chi tiết đơn sẽ hiện ra. Tại đây bạn xem được thông tin khách hàng, các dịch vụ đã đặt, số tiền, và tình trạng thanh toán.

**Bước 3:** Muốn đổi trạng thái, chọn trạng thái mới trong danh sách xổ xuống.

**Bước 4:** Nhấn **"Lưu thay đổi"** để ghi lại.

> **Mỗi lần đổi trạng thái, hệ thống tự ghi lại một dòng nhật ký** trong đơn: đổi từ trạng thái nào sang trạng thái nào. Nhờ vậy bạn luôn truy được ai đã làm gì với đơn, rất hữu ích khi có tranh cãi với khách.

> 📷 *[Cần chụp màn hình: trang chi tiết/chỉnh sửa một đơn hàng]*

## Xử lý nhiều đơn cùng lúc

Nếu cần xử lý hàng loạt thay vì sửa từng đơn:

1. Tích chọn vào **ô vuông đầu dòng** của các đơn cần xử lý.
2. Chọn hành động mong muốn ở menu **"Hành động hàng loạt"** phía trên.
3. Nhấn nút **"Áp dụng"** để thực hiện.

> **Cẩn thận:** Hành động hàng loạt áp dụng ngay cho **tất cả** đơn bạn đã tích, và **không có nút hoàn tác**. Hãy đếm lại số đơn đã chọn trước khi bấm Áp dụng.

## Lưu ý & xử lý sự cố

**Khách báo đã đặt nhưng bạn không thấy đơn:** hãy kiểm tra bộ lọc trạng thái — rất có thể đơn đang ở **Draft** (khách bỏ dở) hoặc **Failed** (thanh toán lỗi) nên bị ẩn khỏi danh sách mặc định.

**Khách báo đã chuyển khoản nhưng đơn vẫn "chưa thanh toán":** với hình thức chuyển khoản thủ công, hệ thống **không tự biết** tiền đã về. Bạn phải kiểm tra sao kê ngân hàng rồi tự cập nhật trạng thái thanh toán cho đơn.

**Đổi trạng thái nhưng bấm Lưu không được:** kiểm tra xem tài khoản của bạn có quyền sửa đơn không. Quyền xem (`order_view`) và quyền sửa là hai thứ khác nhau.

**Lỡ chuyển nhầm trạng thái:** bạn chỉ cần chọn lại trạng thái đúng và lưu lần nữa. Nhật ký sẽ ghi cả hai lần đổi — đây là điều bình thường, không sao cả.

> **Cẩn thận với "Đã hoàn tiền":** trạng thái này chỉ **ghi nhận** rằng bạn đã hoàn tiền, chứ hệ thống **không tự động chuyển tiền** về cho khách. Bạn vẫn phải tự thực hiện việc hoàn tiền qua ngân hàng hoặc cổng thanh toán.

## Xem thêm

- [3.8. Booking](booking.md) — chi tiết từng lượt đặt dịch vụ
- [4.13. Báo cáo](../khoi-he-thong/bao-cao.md) — thống kê doanh thu và tình hình đặt chỗ
