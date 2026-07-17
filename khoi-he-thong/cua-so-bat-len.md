# 4.2. Cửa sổ bật lên

**Cửa sổ bật lên** (tiếng Anh là **"Popup"**) là cái khung quảng cáo tự nhảy ra giữa màn hình khi khách vào website của bạn. Chắc chắn bạn đã gặp nó ở nhiều trang web: một tấm ảnh khuyến mãi hiện lên, có dấu **X** ở góc để tắt đi.

Mục này để bạn **tự tạo những cửa sổ đó**, không cần nhờ ai sửa code.

Dùng khi nào? Ví dụ thực tế:

- Bạn đang chạy chương trình **"Giảm 20% tour Hạ Long trong tháng 7"** và muốn mọi khách vào web đều nhìn thấy.
- Bạn muốn quảng bá một tour mới ra mắt.
- Bạn muốn mời khách để lại số điện thoại để được tư vấn.

Ưu điểm lớn nhất: bạn **hẹn giờ trước** được. Ví dụ tạo sẵn popup Tết từ tháng 12, đặt lịch chạy từ 20/1 đến 10/2 — đến ngày nó tự hiện, hết ngày nó tự tắt, bạn không cần nhớ để vào tắt tay.

> **Đường dẫn:** Menu bên trái > **Hệ thống** > **Cửa sổ bật lên**

> **Lưu ý:** Mục này **không có menu con**. Bấm vào là vào thẳng danh sách các cửa sổ bật lên.

![](../.gitbook/assets/pg123-0.png)

## Màn hình danh sách có gì?

Vào mục này, bạn thấy một bảng liệt kê các cửa sổ bật lên đã tạo, với các cột:

- **Tên (Name)** — tên bạn đặt cho popup. Đây là **tên nội bộ để bạn nhận ra nó**, khách hàng không nhìn thấy tên này. Nên đặt tên rõ ràng như `Khuyen mai He 2026`, `Popup Tet Nguyen Dan` — tránh đặt `popup 1`, `test`.
- **Trạng thái (Status)** — một nhãn nhỏ cho biết popup này đang **chạy thật** hay chỉ **đang lưu nháp**. Đây là cột bạn cần nhìn kỹ nhất.
- **Ngày (Date)** — lần sửa gần nhất.

Phía trên có ô **tìm kiếm theo tên**, ô **hành động hàng loạt**, và nút **"Thêm mới"** để tạo popup mới.

## Tạo một cửa sổ bật lên mới

Nhấn nút thêm mới ở góc trên bên phải. Màn hình tạo popup chia thành nhiều phần, ta đi lần lượt.

### Bước 1: Nội dung — popup sẽ hiện cái gì?

Đây là phần bắt buộc phải điền:

- **Tên (Name)** — như đã nói ở trên, tên nội bộ cho bạn dễ quản lý, khách không thấy.
- **Ảnh banner (Banner Image)** — **đây chính là nội dung mà khách nhìn thấy**. Cửa sổ bật lên ở đây hoạt động rất đơn giản: nó là **một tấm ảnh có thể bấm được**, không phải một trang có chữ và nút bấm phức tạp. Vậy nên **mọi thông tin khuyến mãi của bạn phải nằm sẵn trong tấm ảnh** — bạn thiết kế ảnh đó trước rồi tải lên đây.
- **Đường dẫn khi bấm (Redirect URL)** — khách bấm vào tấm ảnh thì đi đâu? Ví dụ dán vào đây địa chỉ trang tour đang khuyến mãi. Bạn mở trang tour đó ở tab khác, copy nguyên dòng địa chỉ trên thanh trình duyệt rồi dán vào.
- **Mở link ở tab mới (Open link in new tab)** — tích ô này thì khi khách bấm, trang mới mở ra ở một tab riêng, **trang cũ vẫn còn nguyên**. Nên tích, vì khách xem xong tour mà không thích thì vẫn còn trang cũ để quay lại — không bị mất khách.

> **Cẩn thận với ảnh:** Ảnh chụp từ điện thoại hoặc ảnh thiết kế chưa nén thường rất nặng (5–10 MB). Ảnh nặng làm popup hiện chậm, hoặc khách đã tắt trang trước khi ảnh kịp hiện — coi như quảng cáo vô ích. Hãy dùng ảnh dưới 1 MB.
>
> **Mẹo:** Nhớ nghĩ tới khách xem bằng **điện thoại** — họ chiếm phần lớn lượng truy cập. Chữ trong ảnh phải to, đọc được trên màn hình nhỏ.

### Bước 2: Thời điểm bật lên — hiện lúc nào?

Phần này (**"Trigger"** — điều kiện kích hoạt) quyết định popup nhảy ra vào lúc nào. Bạn chọn **một trong 4 kiểu**:

- **Ngay khi tải trang (Page load immediately)** — khách vừa vào là hiện ngay. Chắc chắn khách thấy, nhưng dễ gây khó chịu vì họ chưa kịp xem gì đã bị chặn.
- **Sau X giây (After X seconds)** — chờ một lúc rồi mới hiện. Chọn kiểu này thì bên dưới hiện thêm ô để bạn điền **số giây**.
- **Khi cuộn được X% trang (Scroll X% of page)** — khách cuộn xuống tới một mức nào đó mới hiện. Chọn kiểu này thì bên dưới hiện ô để bạn điền **phần trăm**. Ý nghĩa: người cuộn xuống là người thật sự đang quan tâm nội dung.
- **Khi khách định thoát (Exit intent)** — hệ thống nhận ra khách đang đưa chuột lên để đóng tab, và hiện popup ngay lúc đó như một lời níu kéo cuối cùng.

> **Mẹo chọn kiểu nào:** Nếu bạn phân vân, hãy chọn **"Sau X giây"** và điền khoảng **5 đến 10 giây**. Đây là lựa chọn cân bằng nhất: khách có thời gian nhìn qua website trước, không bị chặn ngay từ giây đầu, mà vẫn chưa kịp thoát.
>
> **Đừng đặt 1 giây.** Nó gây cảm giác bị làm phiền, khách bấm tắt theo phản xạ mà không thèm đọc — bạn mất công thiết kế ảnh mà không ai xem.

### Bước 3: Hiện ở trang nào?

Phần **"Show on"** cho bạn chọn popup xuất hiện ở những trang nào, gồm 2 danh sách:

- **Trang được hiện (Include URLs)** — chỉ hiện ở những địa chỉ bạn liệt kê ở đây.
- **Trang không hiện (Exclude URLs)** — loại trừ, không hiện ở những địa chỉ này.

Cả hai đều **thêm được nhiều dòng**, và hỗ trợ **dấu sao `*`** với nghĩa là "bất kỳ gì". Ví dụ `*/checkout/*` nghĩa là "mọi trang thanh toán".

> **Mẹo rất quan trọng:** Hãy **luôn loại trừ trang thanh toán** bằng cách thêm `*/checkout/*` vào ô "Trang không hiện". Lý do: khách đang điền thông tin đặt tour, chuẩn bị trả tiền, mà bị một cửa sổ nhảy ra che mất — nhiều người sẽ bỏ đi luôn. Bạn mất một đơn hàng thật để đổi lấy một lượt xem quảng cáo. Không đáng.

### Bước 4: Lịch chạy — chạy từ ngày nào tới ngày nào?

Phần **"Schedule"** (lịch):

- **Ngày bắt đầu (Start date)** và **Ngày kết thúc (End date)** — popup chỉ tự động hiện trong khoảng thời gian này. Hết ngày kết thúc, nó tự ngừng, bạn không cần nhớ vào tắt.
- **Lặp lại sau khi khách tắt (Repeat after dismiss)** — khách đã bấm X tắt popup rồi, thì bao lâu sau mới hiện lại cho họ? Bạn điền một con số ở ô **"Show every"** và chọn đơn vị: **ngày / tháng / năm**.

> **Cẩn thận:** Nếu không đặt phần lặp lại này cho hợp lý, khách tắt popup xong bấm sang trang khác lại thấy nó nhảy ra tiếp — cực kỳ khó chịu và họ sẽ rời web. Đặt **1 ngày** là mức hợp lý cho hầu hết trường hợp: khách đã tắt thì hôm nay không bị làm phiền nữa.

### Bước 5: Xuất bản — bước quan trọng nhất, đừng bỏ qua

Ở **cột bên phải** màn hình có phần chọn trạng thái, với 2 lựa chọn:

- **"Publish"** (Xuất bản) — popup **chạy thật**, khách vào web sẽ thấy.
- **"Draft"** (Bản nháp) — chỉ lưu lại cho bạn, **khách không nhìn thấy gì cả**.

Chọn xong nhấn nút **"Save Changes"** (Lưu thay đổi).

> **Đây là lỗi phổ biến nhất của mục này:** Làm xong hết, thiết kế ảnh đẹp, bấm Lưu, rồi ra ngoài web ngồi thắc mắc *"sao không thấy popup đâu?"*. Nguyên nhân 9/10 lần là **popup đang ở trạng thái "Draft" (Bản nháp)**. Lưu ≠ Xuất bản. Phải chọn **"Publish"** thì khách mới thấy.

Cạnh nút Lưu còn có nút **"Preview"** (Xem trước) để bạn kiểm tra popup trông thế nào trước khi cho chạy thật. **Hãy luôn bấm xem trước** — rẻ hơn nhiều so với việc để khách nhìn thấy một tấm ảnh sai chính tả.

## Xem popup của bạn hiệu quả không?

Khi bạn **mở lại một popup đã tạo** để sửa, sẽ có thêm một phần thống kê (**Analytics**) cho biết:

- **Lượt xem (Views)** — bao nhiêu người đã nhìn thấy popup.
- **Lượt bấm (Clicks)** — bao nhiêu người bấm vào ảnh.
- **CTR** — tỷ lệ phần trăm giữa số người bấm và số người xem. Ví dụ 100 người thấy mà 3 người bấm thì CTR là 3%.
- **Lượt tắt (Closes)** — bao nhiêu người bấm X tắt đi.

**Cách đọc mấy con số này cho có ích:** Nếu **Lượt xem rất cao mà Lượt bấm gần bằng 0**, nghĩa là popup có hiện nhưng ảnh của bạn không đủ hấp dẫn, hoặc thông điệp không rõ. Hãy đổi ảnh khác, chứ đừng tăng tần suất hiện — làm vậy chỉ khiến khách khó chịu hơn.

> **Lưu ý:** Phần thống kê này **chỉ hiện khi bạn mở popup cũ ra sửa**. Lúc đang tạo mới thì chưa có số liệu gì, vì popup chưa chạy ngày nào.

## Các hành động hàng loạt

Ở màn hình danh sách, bạn tích chọn nhiều popup rồi chọn thao tác ở ô **Hành động hàng loạt**, sau đó nhấn **"Áp dụng"** (rất hay bị quên bước này):

- **Publish** (Xuất bản) — cho chạy.
- **Move to Draft** (Chuyển về nháp) — **cách tắt popup nhanh nhất** mà không mất công đã làm. Ví dụ khuyến mãi kết thúc sớm, bạn chuyển về nháp là nó biến mất khỏi web ngay, nhưng vẫn còn nguyên để năm sau dùng lại.
- **Move to Pending** (Chuyển sang chờ duyệt).
- **Clone** (Nhân bản) — tạo một bản sao. **Cực kỳ tiện:** năm ngoái bạn có popup Tết rất ổn, năm nay chỉ cần nhân bản nó ra, đổi ảnh và đổi lịch chạy, không phải làm lại từ đầu.
- **Delete** (Xóa) — xóa đi.

> **Mẹo:** Muốn ngừng một popup, hãy **chuyển về "Draft"** thay vì **"Delete"**. Chuyển nháp thì sau này lấy lại được, xóa thì mất công làm lại từ đầu.

Trang **Recovery** (thùng rác) chứa các popup đã xóa, cho phép **khôi phục lại** hoặc **xóa vĩnh viễn**.

## Lưu ý & xử lý sự cố

**Popup không hiện trên website.** Kiểm tra lần lượt theo thứ tự này, đây là 5 nguyên nhân theo mức độ thường gặp:

1. **Trạng thái vẫn là "Draft"** — nguyên nhân số 1. Mở popup ra, đổi sang **"Publish"** rồi lưu lại.
2. **Chưa tới ngày bắt đầu, hoặc đã qua ngày kết thúc** — kiểm tra lại phần Lịch chạy.
3. **Bạn đã tắt popup đó rồi** — hệ thống nhớ là bạn đã tắt nên không hiện lại cho bạn nữa. Hãy mở website bằng **cửa sổ ẩn danh** (trong Chrome: nhấn **Ctrl + Shift + N**) để xem như một khách hoàn toàn mới.
4. **Trang bạn đang đứng bị loại trừ** — xem lại danh sách "Trang không hiện".
5. **Trình duyệt giữ bản cũ** — nhấn **Ctrl + F5** để tải lại sạch.

**Popup hiện nhưng chỉ thấy khung trống / ô ảnh vỡ.**
Ảnh banner chưa được tải lên, hoặc tải lên bị lỗi. Mở popup ra, tải lại ảnh và lưu.

**Khách bấm vào popup nhưng không đi đâu cả.**
Ô **"Redirect URL"** đang trống hoặc dán sai địa chỉ. Hãy mở trang đích ở một tab khác, copy nguyên dòng địa chỉ trên thanh trình duyệt (phải bắt đầu bằng `https://`) rồi dán lại. Nhớ kiểm tra không bị dính dấu cách thừa ở đầu/cuối khi dán.

**Khách phàn nàn popup hiện đi hiện lại.**
Phần **"Repeat after dismiss"** đang đặt quá ngắn hoặc chưa đặt. Hãy đặt **1 ngày** trở lên.

**Popup che mất nội dung trên điện thoại.**
Ảnh bạn thiết kế theo tỷ lệ ngang của máy tính nên trên điện thoại bị chiếm hết màn hình. Hãy dùng ảnh có tỷ lệ vuông hoặc dọc hơn.

## Xem thêm

- [4. Khối HỆ THỐNG](README.md)
- [4.7. Giao diện](giao-dien.md)
