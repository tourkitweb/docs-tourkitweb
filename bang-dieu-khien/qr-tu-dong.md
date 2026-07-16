# 1.5. QR tự động

## a, Chỉ số theo dõi giao dịch

Các thẻ màu phía trên cung cấp cái nhìn tổng quan về tình trạng đồng bộ dữ liệu:

- Tổng Webhook: Tổng số lượt dữ liệu thanh toán đã gửi về hệ thống.

- Đã xử lý: Các giao dịch được ghi nhận và khớp lệnh thành công.

- Không khớp: Giao dịch nhận được nhưng thông tin (như nội dung chuyển khoản) không khớp với đơn hàng hiện có.

- Thất bại: Các yêu cầu gặp lỗi trong quá trình truyền tải dữ liệu.

![](../.gitbook/assets/pg034-0.png)

## b, Bộ lọc và Tìm kiếm

Để kiểm tra một giao dịch cụ thể, bạn có thể sử dụng các công cụ lọc phía dưới:

- Trạng thái (đã nhận, đã xử lý, không khớp, thất bại) & Loại khớp (đã cọc, đặt chỗ): Lọc theo các kết quả thành công, thất bại hoặc không khớp.

![](../.gitbook/assets/pg035-0.png)

- Khoảng thời gian: Chọn ngày bắt đầu và kết thúc để xem lịch sử giao dịch trong một thời điểm nhất định.

- Tìm kiếm: Nhập mã giao dịch hoặc thông tin liên quan để định vị nhanh.

![](../.gitbook/assets/pg035-1.png)

## c, Chi tiết Webhook Logs

Bảng danh sách cung cấp đầy đủ thông tin kỹ thuật của từng lần thanh toán:

- Transaction Code: Mã giao dịch duy nhất từ phía ngân hàng.

- Số tiền & Nội dung: Số tiền khách đã chuyển và nội dung chuyển khoản thực tế.

- Ngân hàng: Tên ngân hàng thực hiện giao dịch.

- Trạng thái & Khớp với: Hiển thị kết quả xử lý và mã đơn hàng tương ứng trên website mà giao dịch này đã được áp dụng.

- Thời gian: Ngày giờ chính xác hệ thống nhận được dữ liệu.

![](../.gitbook/assets/pg036-0.png)
