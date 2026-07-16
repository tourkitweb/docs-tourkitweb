# 4.10. Tích hợp

4.9.1. Open AI 4.9.2. Tourkit CRM

4.9.3. PMS Gohost - Khách 4.9.4. Thanh toán tingee sạn

4.9.5. Thông báo qua các 4.9.6. Affiliate với đối tác kênh Telegram/ Discord

## Open AI

## Tourkit CRM

![](../.gitbook/assets/pg138-0.png)

## a, Đồng bộ đơn hàng/ request booking từ Website

## về hệ thống CRM

Mục này dùng để thiết lập kết nối kỹ thuật giữa website/hệ thống của bạn và hệ thống CRM.

- Bật đồng bộ CRM?: Tích chọn vào ô để Có, bật tính năng đồng bộ CRM kích hoạt toàn bộ tính năng kết nối. Nếu bỏ tích, mọi hoạt động đồng bộ sẽ tạm dừng.

- CRM API Endpoint: Nhập đường dẫn link API được cung cấp từ phía hệ thống CRM của bạn. ◦ Lưu ý: Không điền dấu gạch chéo ( ) ở cuối đường dẫn (Ví dụ đúng: / ). https://crm.example.com/api/phieu

- CRM API Key: Nhập mã khóa bảo mật (API Key) do bên CRM cung cấp để xác thực quyền truy cập dữ liệu.

- Lưu cấu hình: Nhấp nút [Lưu cài đặt] màu xanh lá ở góc trên cùng bên phải để hoàn tất thiết lập.

## b, Đồng bộ Tours từ CRM về hệ thống (Đồng bộ

## Tours từ CRM)

Mục này hỗ trợ bạn chủ động kéo các chương trình Tour mẫu đã có sẵn trên CRM về lưu trữ và hiển thị trên hệ thống website hiện tại.

- Ngày bắt đầu / Ngày kết thúc (dd/mm/yyyy): Chọn khoảng thời gian để giới hạn dữ liệu tour muốn kéo về. Hệ thống sẽ chỉ quét các tour được tạo hoặc cập nhật trong khoảng thời gian này.

- Force update (cập nhật lại tour đã tồn tại): * Tích chọn: Nếu muốn ghi đè, cập nhật thông tin mới nhất từ CRM cho các tour đã từng đồng bộ về hệ thống trước đó. ◦ Bỏ tích: Hệ thống sẽ bỏ qua và chỉ tải về các tour mới hoàn toàn.

- Dry run (xem trước, không lưu): Tích chọn nếu bạn chỉ muốn chạy thử nghiệm để kiểm tra xem dữ liệu có lỗi gì không mà không muốn lưu trực tiếp vào cơ sở dữ liệu.

- Thực hiện: Nhấp nút số màu vàng [Đồng bộ Tours từ CRM] để bắt đầu quá trình quét dữ liệu.

## c, Kiểm tra thử nghiệm đồng bộ (Test đồng bộ CRM)

Tính năng này giúp bạn kiểm tra xem luồng dữ liệu đẩy từ hệ thống lên CRM có hoạt động mượt mà và chính xác hay không đối với một đơn hàng cụ thể.

- Chọn Booking: Nhấp vào ô tìm kiếm và nhập mã booking, tên khách hàng, email hoặc số điện thoại để chọn một đơn hàng thực tế cần test.

- Xem Payload: Nhấp nút [Xem Payload] (màu xanh cyan) để kiểm tra cấu trúc dữ liệu thô (JSON) hệ thống sẽ gửi đi trước khi thực hiện đẩy sang CRM.

- Test Sync CRM: Nhấp nút [Test Sync CRM] (màu xanh dương) để tiến hành gửi thử dữ liệu của đơn hàng đó lên CRM và kiểm tra kết quả trả về của hệ thống kết nối.

## PMS Gohost - Khách sạn

![](../.gitbook/assets/pg140-0.png)

## a, Kết nối PMS Gohost

Trước khi đồng bộ dữ liệu, vui lòng nhập đầy đủ thông tin kết nối PMS Gohost trong phần cài đặt hệ thống.

Sau khi cấu hình thành công, hệ thống sẽ có thể lấy dữ liệu từ PMS Gohost để đồng bộ về website.

## b, Cấu hình Booking và Thanh toán

Phần này giúp định nghĩa cách xử lý dòng tiền và nguồn dữ liệu khi đổ về hệ thống PMS.

- Payment Collect: Chọn hình thức thu tiền khách hàng để làm cơ sở xử lý quy trình thanh toán trên PMS.

- Booking Source (Nguồn đặt phòng): Chọn tên nguồn ghi nhận đơn hàng khi đổ vào PMS (Ví dụ: từ website, booking.com, agoda...).

- **Lưu ý:** Tên nguồn được chọn phải khớp chính xác với danh sách Booking Source đã thiết lập sẵn bên hệ thống PMS của bạn.

- Phương thức thanh toán (Payment Method): Chọn phương thức thanh toán tương ứng được ghi nhận vào PMS khi cổng thanh toán (ví dụ: Tingee) xác nhận giao dịch thành công.

## c, Đồng bộ Hotels từ PMS về hệ thống

Tính năng này giúp bạn chủ động kéo toàn bộ danh sách phòng/khách sạn từ PMS Gohost về lưu trữ và hiển thị trực tiếp trên hệ thống hiện tại. Quá trình này thường diễn ra rất nhanh (chỉ mất vài giây).

- Force update (cập nhật lại hotel/room đã tồn tại): * Tích chọn: Nếu muốn cập nhật lại toàn bộ thông tin mới nhất cho các khách sạn/phòng đã từng được đồng bộ trước đó.

- Bỏ tích: Hệ thống chỉ tải về những khách sạn hoặc phòng mới được thêm trên PMS.

- Dry run (xem trước, không lưu): Tích chọn nếu bạn muốn hệ thống chạy thử nghiệm để kiểm tra tính ổn định của dữ liệu mà không lưu đè vào cơ sở dữ liệu thật.

- Thực hiện: Nhấp nút [Đồng bộ Hotels từ PMS] màu vàng để bắt đầu quá trình kéo dữ liệu.

Hệ thống sẽ tự động:

- Lấy danh sách phòng từ PMS Gohost.

- Tạo mới các phòng chưa tồn tại trên website.

- Cập nhật thông tin các phòng đã được đồng bộ trước đó.

- Hệ thống có thể lấy: Giá phòng. Số lượng phòng còn trống. Trạng thái mở bán. từ PMS Gohost.

Sau khi hoàn tất, danh sách phòng sẽ xuất hiện trong phần quản lý phòng của website.

Vui lòng kiểm tra và cập nhật thêm các thông tin cần thiết như:

- Hình ảnh phòng.

- Nội dung mô tả.

- Tiện nghi.

- Thứ tự hiển thị.

- Trạng thái hiển thị.

**Lưu ý:** Một số nội dung marketing và hình ảnh thường cần được bổ sung thủ công trên website để tối ưu trải nghiệm khách hàng.

## Thanh toán Tingee

![](../.gitbook/assets/pg143-0.png)

## 1. Kích hoạt kết nối

- Bật Tingee Webhook?: Tích chọn ô để Có, bật nhận webhook từ Tingee hệ thống bắt đầu tự động nhận dữ liệu thông báo biến động số dư.

## 2. Các bước liên kết cấu hình

Thực hiện liên kết 2 chiều giữa hệ thống của bạn và Tingee theo các bước sau:

![](../.gitbook/assets/pg143-1.png)

## Thông báo qua các kênh Telegram / Discord

## a. Chọn thời điểm nhận thông báo

![](../.gitbook/assets/pg144-0.png)

Bạn có thể chọn một hoặc cả hai thời điểm sau:

🛒 Khi khách thêm vào giỏ hàng: Thông báo được gửi ngay khi khách tạo booking hoặc thêm dịch vụ vào giỏ hàng.

Phù hợp khi bạn muốn:

- Theo dõi khách hàng đang quan tâm đến sản phẩm.

- Chủ động liên hệ tư vấn sớm.

- Theo dõi lượng booking phát sinh trong ngày.

**Lưu ý:** Ở giai đoạn này khách chưa thanh toán, đơn hàng có thể bị hủy hoặc không hoàn tất.

✅ Khi khách thanh toán thành công: Thông báo được gửi khi booking đã hoàn tất thanh toán thành công.

Phù hợp khi bạn muốn:

- Xác nhận đơn hàng đã được thanh toán.

- Theo dõi doanh thu thực tế.

- Chỉ nhận các đơn hàng hoàn tất.

Nếu không chọn thời điểm nào, hệ thống sẽ không gửi thông báo dù Telegram hoặc Discord đã được bật.

## b. Thông báo qua kênh Telegram

![](../.gitbook/assets/pg145-0.png)

![](../.gitbook/assets/pg145-1.png)

*📺 Video hướng dẫn: Telegram: Hướng dẫn lấy ID Telegram cá nhân, nhóm*

Maxpro

## c. Thông báo qua kênh Discord

![](../.gitbook/assets/pg146-0.png)

![](../.gitbook/assets/pg146-1.png)

*📺 Video hướng dẫn: How to get Webhook URL of your Discord Server?*

JamessCz

## Affiliate với đối tác

![](../.gitbook/assets/pg147-0.png)

## Hướng dẫn kết nối Accesstrade

Để website có thể ghi nhận và đồng bộ đơn hàng với Accesstrade, vui lòng cung cấp các thông tin sau từ tài khoản Accesstrade của doanh nghiệp.

## Bước 1: Đăng nhập Accesstrade

Đăng nhập vào tài khoản Advertiser trên hệ thống Accesstrade.

## Bước 2: Lấy Access Key

1. Truy cập phần quản lý API hoặc Tracking theo hướng dẫn của Accesstrade. 2. Tìm thông tin Access Key. 3. Sao chép Access Key và dán vào ô:

Access Key

trong phần cài đặt website.

## Bước 3: Lấy Tracking Script

1. Trong tài liệu hoặc phần cài đặt Tracking của Accesstrade, tìm đoạn mã theo dõi (Tracking Script). 2. Sao chép toàn bộ đoạn mã được Accesstrade cung cấp. 3. Dán vào ô:

Tracking Script

trong phần cài đặt website.

## Bước 4: Lưu cấu hình

Sau khi nhập đầy đủ thông tin:

- Access Key

- Tracking Script

Nhấn Lưu cấu hình để hoàn tất kết nối.

## Lưu ý

- Mỗi tài khoản hoặc chiến dịch có thể sử dụng Access Key khác nhau.

- Vui lòng sao chép chính xác thông tin được Accesstrade cung cấp.

- Nếu không tìm thấy Access Key hoặc Tracking Script, vui lòng liên hệ nhân viên hỗ trợ của Accesstrade để được hướng dẫn.
