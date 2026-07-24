# Nhập hàng loạt bằng Excel

Nếu bạn có **nhiều khách sạn hoặc nhiều tour** cần đăng cùng lúc, việc điền từng cái qua trình nhập 8 bước sẽ rất lâu. Tính năng **Import Excel** cho phép bạn khai báo hàng loạt trong một file bảng tính rồi tải lên một lần — hệ thống tự tạo tất cả.

Tính năng này có ở cả hai màn quản lý:

- **Khu nhà cung cấp > Hotel** — nhập hàng loạt khách sạn và phòng.
- **Khu nhà cung cấp > Tour** — nhập hàng loạt tour, bảng giá theo khách và lịch khởi hành.

> **Khi nào nên dùng?** Khi bạn có sẵn danh sách (thường là một file Excel của riêng bạn) và muốn đưa lên nhanh. Nếu chỉ thêm một hai sản phẩm, dùng nút **"Thêm khách sạn" / "Thêm tour"** như bình thường sẽ nhanh hơn.

## Quy trình chung: 3 bước

Dù là khách sạn hay tour, cách làm đều giống nhau:

1. **Tải file mẫu** về máy.
2. **Điền dữ liệu** vào file theo hướng dẫn có sẵn trong file.
3. **Tải file lên** (Import) — hệ thống tạo/cập nhật sản phẩm.

Ở đầu màn danh sách khách sạn (hoặc tour), cạnh nút "Thêm…", bạn sẽ thấy hai nút:

- **"Tải file mẫu"** — tải về file Excel mẫu.
- **"Import Excel"** — mở cửa sổ để chọn file đã điền và tải lên.

![](../.gitbook/assets/ncc-import-nut.png)

> **Luôn tải file mẫu MỚI mỗi lần làm.** File mẫu được tạo lại theo dữ liệu hệ thống tại thời điểm bạn tải — danh sách địa điểm, tiện ích, danh mục… luôn cập nhật. Đừng dùng lại file mẫu cũ từ nhiều tháng trước.

## Hiểu về file mẫu

Mở file mẫu ra, bạn sẽ thấy nhiều **sheet** (thẻ ở đáy bảng tính):

- **HƯỚNG DẪN** — đọc trang này trước tiên, có giải thích từng cột.
- **Các sheet dữ liệu** (KHÁCH SẠN, PHÒNG… hoặc TOUR, LỊCH KHỞI HÀNH…) — nơi bạn nhập.
- **DANH MỤC** — danh sách các giá trị hợp lệ (địa điểm, tiện ích, danh mục…) **lấy trực tiếp từ hệ thống**. Chỉ để tra cứu, **không sửa** sheet này.

Vài quy tắc quan trọng khi điền:

- **Cột có dấu (*)** ở tiêu đề là **bắt buộc**, được tô nền vàng nhạt. Các cột khác có thể bỏ trống.
- **Các dòng màu xám** ở đầu mỗi sheet là **dòng ví dụ** (mã bắt đầu bằng "VD"). Chúng chỉ để bạn xem cách điền — hệ thống **tự bỏ qua** khi import, bạn giữ hay xoá đều được. Nhập dữ liệu thật vào các dòng trắng bên dưới.
- **Ô có mũi tên thả xuống** (địa điểm, danh mục, tiện ích, trạng thái…) — bấm vào và **chọn từ danh sách**, đừng gõ tay. Gõ sai tên sẽ bị bỏ qua.

> **Tên phải khớp đúng.** Địa điểm, danh mục, tiện ích bạn điền phải trùng với tên trong sheet DANH MỤC. Nếu điền một cái tên hệ thống không có (ví dụ địa điểm chưa được tạo), sản phẩm **vẫn được tạo** nhưng phần đó bị **bỏ trống** và hệ thống báo cảnh báo cho bạn biết.

## Nhập khách sạn

File mẫu khách sạn có hai sheet dữ liệu:

- **KHÁCH SẠN** — mỗi dòng là một khách sạn. Cần đặt một **"Mã khách sạn"** bất kỳ (ví dụ KS001, KS002…) để nối sang phòng.
- **PHÒNG** — mỗi dòng là một loại phòng. Cột **"Mã khách sạn"** ở đây phải **trùng** mã đã đặt ở sheet KHÁCH SẠN, để hệ thống biết phòng thuộc khách sạn nào.

Các cột chính của khách sạn: tên, loại hình, hạng sao, địa chỉ, địa điểm, số điện thoại, giá cơ bản, và **6 cột "Tiện ích khách sạn 1…6"** — mỗi cột chọn một tiện ích. Các cột chính của phòng: tên loại phòng, giá/đêm, số lượng phòng, sức chứa, và **6 cột "Tiện nghi phòng 1…6"**.

> **Nhớ thứ tự:** điền sheet KHÁCH SẠN trước, rồi mới tới PHÒNG. Một khách sạn không có phòng nào thì khách xem được nhưng **không đặt được** — hãy nhập ít nhất một loại phòng cho mỗi khách sạn.

## Nhập tour

File mẫu tour có ba sheet dữ liệu:

- **TOUR** — mỗi dòng là một tour. Đặt một **"Mã tour"** bất kỳ (ví dụ T001) để nối sang hai sheet kia. Có **"Giá cơ bản"** (dùng khi tour chỉ một mức giá), 3 cột **"Phong cách"** và 6 cột **"Tiện ích"**.
- **BẢNG GIÁ THEO KHÁCH** (không bắt buộc) — nơi khai báo **giá theo nhiều loại khách**. Mỗi dòng là một loại khách + giá; **tên loại khách do bạn tự đặt** (Người lớn, Trẻ em, Người cao tuổi, Khách VIP, Đoàn…). Nhiều dòng cùng một "Mã tour" = nhiều mức giá cho tour đó.
- **LỊCH KHỞI HÀNH** (không bắt buộc) — mỗi dòng là một ngày đi: ngày bắt đầu, ngày kết thúc, số chỗ, Bật/Tắt.

> **Giá cơ bản và bảng giá theo khách khác nhau thế nào?**
> - Nếu tour **chỉ một giá** cho mọi khách: chỉ cần điền **"Giá cơ bản"** ở sheet TOUR, bỏ trống sheet bảng giá.
> - Nếu tour có **nhiều mức giá** (người lớn/trẻ em/VIP…): điền ở sheet **BẢNG GIÁ THEO KHÁCH**. Khi đó tour tự bật chế độ giá theo loại khách, và **loại đầu tiên** trong bảng được lấy làm giá khởi điểm (thay cho ô Giá cơ bản).

> **Ngày khởi hành phải là ngày sắp tới.** Ngày đã qua (trước hôm nay) điền trong file sẽ bị **bỏ qua** — chỉ nhập ngày trong tương lai. Định dạng ngày là **YYYY-MM-DD** (ví dụ 2026-09-15).

> **Tour nhập bằng Excel mặc định là "chỉ bán theo ngày cụ thể".** Nghĩa là khách chỉ đặt được vào các ngày bạn khai trong sheet LỊCH KHỞI HÀNH. Muốn tour bán mọi ngày, vào sửa tour ở bước **Giá** và đổi thành *"Luôn có sẵn"*.

### Thay thế toàn bộ lịch khởi hành

Trong cửa sổ Import tour có một ô tích **"Thay thế toàn bộ lịch khởi hành"**. Ô này dành cho việc **làm mới lịch theo kỳ** (ví dụ mỗi tháng):

- **Để TẮT (mặc định):** import chỉ **thêm và cập nhật**. Ngày cũ trong hệ thống không bị đụng tới.
- **BẬT:** sau khi import, các ngày khởi hành **tương lai** không có trong file sẽ bị **xoá** để lịch trên web khớp đúng file bạn vừa tải lên.

> **Bật ô này KHÔNG làm mất đơn khách.** Hai loại ngày luôn được giữ lại kể cả khi không có trong file: ngày **đã qua** (để còn báo cáo) và ngày **đã có đơn khách đặt**. Với ngày đã có khách, hệ thống báo cảnh báo và không xoá.

**Cách dùng theo tháng:** mỗi kỳ, trong file bạn chỉ để **những ngày sắp mở bán**, tích "Thay thế toàn bộ lịch khởi hành" rồi import. Hệ thống tự dọn các ngày cũ không còn bán và giữ nguyên ngày đã có khách.

![](../.gitbook/assets/ncc-import-cua-so.png)

## Import lại để cập nhật

Bạn có thể sửa lại file rồi **import lại nhiều lần**. Hệ thống **khớp theo tên**:

- **Khách sạn / tour** khớp theo **tên** — trùng tên thì **cập nhật**, tên mới thì **tạo mới**. Không tạo trùng.
- **Phòng** khớp theo tên trong cùng khách sạn; **ngày khởi hành** khớp theo ngày.

> **File Excel nên là "bản gốc" của bạn.** Khi import lại, dữ liệu trong file sẽ **ghi đè** những gì bạn đã chỉnh tay ở màn quản lý (giá, tiện ích, bảng giá khách…). Vì vậy nếu quản lý bằng import, hãy sửa trong file rồi import lại, đừng sửa lẻ ở web rồi lại import file cũ (sẽ mất phần sửa lẻ đó).

> **Đổi tên hoặc đổi ngày sẽ sinh bản trùng.** Nếu bạn đổi *tên tour* trong file, import sẽ tạo một tour **mới** (vì không khớp tên cũ). Tương tự, đổi ngày khởi hành trong cùng một dòng sẽ tạo ngày mới mà ngày cũ vẫn còn. Muốn đổi thì thêm mới và xử lý cái cũ riêng.

## Đọc kết quả sau khi import

Import xong, màn danh sách hiện một **bảng kết quả** với các con số: bao nhiêu **tạo mới**, bao nhiêu **cập nhật**, bao nhiêu **dòng bị bỏ qua**, và (với tour) bao nhiêu **lịch đã xoá**, bao nhiêu **ngày quá khứ bỏ qua**.

Bên dưới là chi tiết:

- **Dòng bị bỏ qua** — kèm số dòng và lý do (ví dụ thiếu tên, không tìm thấy mã khách sạn/tour).
- **Cảnh báo** — những dòng vẫn tạo được nhưng có phần bị bỏ (ví dụ ngày đã có khách nên không xoá).
- **Tên không khớp** — các địa điểm / danh mục / tiện ích bạn điền mà hệ thống không có (đã bỏ qua).

> **Kiểm tra bảng kết quả sau mỗi lần import.** Con số "tạo mới / cập nhật" giúp bạn biết import có đúng như mong đợi không. Nếu thấy "dòng bị bỏ qua" nhiều, mở chi tiết đọc lý do rồi sửa file và import lại.

![](../.gitbook/assets/ncc-import-ket-qua.png)

## Những gì Import KHÔNG làm

Để tránh hiểu nhầm, có vài thứ import không xử lý — bạn làm thủ công sau:

- **Ảnh** — import không tải ảnh. Sau khi import, vào **"Chỉnh sửa"** từng sản phẩm để thêm ảnh đại diện, thư viện ảnh. (Khách sạn/tour không có ảnh vẫn hiển thị nhưng kém hấp dẫn.)
- **Địa điểm / danh mục mới** — import không tạo địa điểm hay danh mục mới. Tên bạn điền phải **đã có sẵn** trong hệ thống (xem sheet DANH MỤC). Cần thêm địa điểm mới thì liên hệ quản trị viên.
- **Giá theo loại khách của khách sạn** — phần này của tour làm được qua file; còn khách sạn nhập giá ở cấp phòng.

## Lưu ý & xử lý sự cố

**Tải file mẫu mà không tải được / báo lỗi:** thử lại; nếu vẫn lỗi, kiểm tra thanh menu còn mục Hotel/Tour không (không có nghĩa là bạn chưa mua gói dịch vụ).

**Import báo "Không đọc được file":** bạn đang tải nhầm file không phải Excel, hoặc file hỏng. Hãy tải lại **file mẫu mới**, điền lại và thử lại. Chỉ nhận đuôi **.xlsx** hoặc **.xls**, tối đa 10MB.

**Import xong nhưng thiếu sản phẩm:** mở bảng kết quả xem mục "dòng bị bỏ qua" — thường do thiếu cột bắt buộc (dấu *) hoặc mã khách sạn/tour ở sheet con không trùng mã ở sheet chính.

**Địa điểm / tiện ích không được gán:** tên điền không khớp sheet DANH MỤC. Mở sheet DANH MỤC, **copy đúng** tên dán vào, hoặc dùng ô thả xuống để chọn.

**Nhập giá bị sai số:** gõ số thuần, không thêm dấu chấm phân cách hay chữ "đ". Ví dụ `1500000` chứ không phải `1.500.000đ`.

**Sửa ở web xong import lại thì mất phần sửa:** đúng như cảnh báo ở trên — file ghi đè phần sửa tay. Hãy chọn một cách quản lý: hoặc luôn qua file, hoặc luôn qua web.

## Xem thêm

- [Nhập & quản lý khách sạn](khach-san.md)
- [Nhập & quản lý phòng](phong.md)
- [Nhập & quản lý tour](tour.md)
