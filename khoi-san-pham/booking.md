# 3.8. Booking

## Quản lý Booking tập trung

Hệ thống tự động tổng hợp tất cả đơn đặt dịch vụ (Khách sạn, Vé máy bay, Tour...) giúp bạn điều phối và theo dõi dòng tiền hiệu quả.

## a, Chỉ số thống kê nhanh

Các thẻ màu phía trên hiển thị tức thời tình trạng vận hành:

- Tổng đơn: Tổng lượng đơn hàng đã phát sinh.

- Chờ xử lý: Các đơn hàng mới cần nhân viên tiếp nhận ngay.

- Hoàn thành & Đã hủy: Thống kê kết quả kinh doanh cuối cùng.

![](../.gitbook/assets/pg107-0.png)

## b, Thông tin chi tiết đơn hàng

Bảng Danh sách Booking cung cấp mọi dữ liệu cần thiết để xử lý:

- Mã đơn & Dịch vụ: Xác định loại hình khách đặt (ví dụ: Hotel, Flight API) và thời gian sử dụng dịch vụ.

- Khách hàng: Tên, Email và Số điện thoại để liên hệ xác nhận.

- Thanh toán: Hiển thị rõ Tổng tiền, số tiền Đã thanh toán và số tiền Còn lại cần thu.

- Trạng thái: Theo dõi tiến độ thanh toán (Chưa thanh toán, Offline Payment...) và tình trạng đơn (Đang xử lý, Đã hủy).

![](../.gitbook/assets/pg108-0.png)

## c, Công cụ quản lý và Xuất dữ liệu

- Bộ lọc chuyên sâu: Tìm kiếm nhanh đơn hàng theo Nhà cung cấp, Trạng thái, Loại dịch vụ, Khoảng ngày hoặc Tên/SĐT khách hàng.

- Hành động hàng loạt: Chọn nhiều đơn để cập nhật trạng thái đồng thời.

- Xuất dữ liệu (Export): Nhấn nút Export (màu xanh lá) để tải danh sách đơn hàng về máy tính phục vụ báo cáo.

![](../.gitbook/assets/pg108-1.png)
