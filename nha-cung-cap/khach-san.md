# Nhập & quản lý khách sạn

Đây là nơi bạn tự đăng và quản lý các cơ sở lưu trú của mình — khách sạn, resort, homestay, villa — để bán trên website.

Trước khi bắt tay, hãy nhớ cấu trúc **hai tầng** này, vì hiểu nó là hiểu hết cách làm:

- **Khách sạn** là "cái nhà" — có tên, ảnh, địa chỉ, hạng sao, tiện nghi chung.
- **Phòng** nằm bên trong cái nhà đó — mỗi loại phòng có giá riêng, số lượng riêng, sức chứa riêng.

Khách hàng đặt **phòng**, chứ không đặt cả khách sạn. Vì vậy tạo xong khách sạn, bạn **bắt buộc** phải sang bước tạo phòng (bài [Nhập & quản lý phòng](phong.md)). Khách sạn không có phòng nào thì khách nhìn thấy nhưng không đặt được gì.

> **Đường dẫn:** Đăng nhập khu nhà cung cấp > menu **Hotel**. Nếu không thấy mục **Hotel** trên thanh menu, bạn chưa mua gói dịch vụ — xem lại [trang tổng quan](README.md).

## Màn hình danh sách khách sạn

Đây là màn hình đầu tiên khi bấm **Hotel**. Nó liệt kê toàn bộ khách sạn **do bạn tạo**.

Trên cùng là **ba thẻ thống kê** cho bạn nhìn nhanh tình hình:

- **Tổng số khách sạn**
- **Đang xuất bản** — số đang bán được trên website
- **Bản nháp chưa xong** — số bạn còn làm dở

Bên dưới là các công cụ lọc danh sách:

- **Ô tìm kiếm** — gõ tên hoặc địa điểm để lọc nhanh ngay tại chỗ (không cần bấm nút, danh sách tự lọc).
- **Tab trạng thái** — *Tất cả* / *Đang xuất bản* / *Bản nháp*, mỗi tab kèm con số đếm.
- **Sắp xếp** — *Mới cập nhật*, *Tên A → Z*, *Giá cao → thấp*, *Giá thấp → cao*.

> 📷 *[Cần chụp màn hình: danh sách khách sạn khu vendor — 3 thẻ thống kê phía trên, tab trạng thái và danh sách card khách sạn phía dưới]*

### Mỗi thẻ khách sạn có gì?

Mỗi khách sạn hiện ra dưới dạng một **thẻ** (card), trên đó có:

- **Badge trạng thái** ở góc — *Đang xuất bản*, *Chờ duyệt*, *Chưa hiển thị* hoặc *Bản nháp* (ý nghĩa xem mục "Trạng thái hiển thị" ở [trang tổng quan](README.md)).
- Thông tin nhanh: địa điểm, giá, số phòng, thời gian cập nhật gần nhất. Chỗ nào chưa nhập sẽ ghi "Chưa có địa điểm", "Chưa đặt giá", "Chưa có phòng".
- Với khách sạn **còn dở**, thẻ hiện thêm **thanh tiến độ** kiểu "Hoàn thành 4/8 bước" và gợi ý bước tiếp theo.
- **Các nút thao tác:**
  - Với bản nháp: **"Tiếp tục hoàn thiện"** (hoặc **"Xem lại & đăng"** nếu bạn đã nhập đủ các mục bắt buộc).
  - Với khách sạn đã đăng: **"Xem"**, **"Chỉnh sửa"**, **"Thêm phòng"**.
  - **Nút ba chấm (⋮)** mở thêm: *Danh sách phòng*, *Nhân bản*, *Ẩn khỏi website*, *Xoá*.

## Thêm khách sạn mới — Trình nhập theo từng bước

Bấm nút **"Thêm khách sạn"** ở đầu trang. Hệ thống **tạo ngay một bản nháp** và đưa bạn vào **trình nhập theo bước** (wizard) — một dạng điền thông tin chia nhỏ thành 8 bước, làm xong bước này bấm sang bước kia, thay vì phải điền một trang dài.

> **Đừng sợ mất công.** Vì bản nháp được tạo ngay từ đầu, bạn có thể **dừng bất cứ lúc nào** — thông tin đã điền vẫn được lưu (hệ thống tự lưu ngầm). Lần sau quay lại, bấm "Tiếp tục hoàn thiện" là làm tiếp từ chỗ đang dở.

Ở cuối mỗi bước luôn có ba nút:

- **"Quay lại"** — về bước trước.
- **"Lưu nháp"** — lưu lại rồi thoát, chưa cần điền đủ.
- **"Tiếp tục: [tên bước sau]"** — kiểm tra thông tin bước hiện tại rồi sang bước kế. Ở bước cuối, nút này đổi thành **"Hoàn tất & Đăng"**.

> 📷 *[Cần chụp màn hình: giao diện wizard thêm khách sạn — thanh các bước ở trên, nội dung bước đang nhập, và 3 nút Quay lại / Lưu nháp / Tiếp tục ở dưới]*

### 8 bước nhập khách sạn

Dưới đây là toàn bộ 8 bước theo đúng thứ tự. Dấu ⭐ đánh dấu những mục **bắt buộc** — thiếu chúng thì khách sạn không đăng bán được.

**Bước 1 — Tên & Mô tả**
- ⭐ **Tên khách sạn** và ⭐ **Nội dung mô tả** giới thiệu.
- **Video** giới thiệu (dán link YouTube, không bắt buộc).

**Bước 2 — Vị trí & Địa chỉ**
- ⭐ Chọn **Địa điểm** (tỉnh/thành phố) và ⭐ nhập **Địa chỉ** cụ thể.
- Ghim vị trí trên **bản đồ** và mô tả khu vực xung quanh (không bắt buộc).

> **Không tìm thấy tỉnh/thành cần chọn?** Nghĩa là địa điểm đó chưa được tạo trong hệ thống. Hãy liên hệ quản trị viên để họ thêm địa điểm, rồi bạn quay lại chọn.

**Bước 3 — Hình ảnh**
- ⭐ **Ảnh đại diện** — ảnh khách nhìn thấy đầu tiên, hãy chọn ảnh đẹp nhất.
- **Ảnh bìa (banner)** và **Thư viện ảnh** (nhiều ảnh phụ để khách xem chi tiết).

> **Về ảnh:** ảnh từ điện thoại đời mới thường nặng 5–10 MB, tải lên rất chậm. Hãy dùng ảnh khoảng 1–2 MB là đủ đẹp. Nếu bấm tải mà quay mãi không xong, gần như chắc chắn do ảnh quá nặng.

**Bước 4 — Tiện nghi**
- Tích chọn các tiện nghi **của cả khách sạn**: hồ bơi, bãi đỗ xe, phòng gym, wifi… Đây là các tiêu chí để khách lọc tìm trên website.

**Bước 5 — Chính sách & Nổi bật**
- **Hạng sao**, **số điện thoại**, **website** của khách sạn.
- **Điểm nổi bật** và **Chính sách** (nội quy, quy định chung).

**Bước 6 — Giờ nhận/trả phòng**
- **Giờ nhận phòng (check-in)** và **giờ trả phòng (check-out)**.
- Cho phép đặt theo ngày, số ngày báo trước tối thiểu, số đêm ở tối thiểu.

**Bước 7 — Giá & Phụ phí**
- ⭐ **Giá** cơ bản của khách sạn.
- **Giá khuyến mãi**, thời gian flash sale.
- Bật/tắt **phụ phí thêm người** và **phí dịch vụ**.

> **Đây chỉ là giá tham khảo ở cấp khách sạn.** Giá khách thực sự trả là giá của **từng loại phòng** bạn tạo ở bước sau. Đừng bỏ trống ô này (nó bắt buộc), nhưng hãy hiểu giá bán thật nằm ở phần Phòng.

**Bước 8 — Danh mục & Hoàn tất**
- Chọn **Danh mục** (loại hình: 5 sao, resort, homestay…) để khách dễ lọc.
- Chọn các khách sạn **tương tự** để gợi ý chéo, và điền thông tin **SEO** (tiêu đề, mô tả hiển thị trên Google).
- Bấm **"Hoàn tất & Đăng"** để đăng bán.

> **Điều gì xảy ra khi bấm "Hoàn tất & Đăng"?**
> - Nếu website **không** bắt duyệt: khách sạn chuyển sang **"Đang xuất bản"** ngay.
> - Nếu website **có** bắt quản trị viên duyệt: khách sạn chuyển sang **"Chờ duyệt"** — bạn phải đợi quản trị viên phê duyệt thì khách mới thấy.

> **Bấm "Hoàn tất" mà bị đưa sang trang Gói dịch vụ?** Nghĩa là gói dịch vụ của bạn đã hết hạn hoặc hết lượt đăng. Chỉ những sản phẩm **đang xuất bản** mới tính vào hạn mức gói. Hãy gia hạn/nâng gói rồi đăng lại.

## Bước tiếp theo bắt buộc: Tạo phòng

Đăng xong khách sạn, việc **chưa hề kết thúc**. Khách đặt phòng chứ không đặt khách sạn, nên bạn phải tạo ít nhất một loại phòng. Từ thẻ khách sạn, bấm **"Thêm phòng"** (hoặc mở nút ⋮ > *Danh sách phòng*).

👉 Xem chi tiết ở bài [Nhập & quản lý phòng](phong.md).

## Sửa khách sạn đã đăng

Bấm **"Chỉnh sửa"** trên thẻ khách sạn. Hệ thống mở lại đúng trình nhập 8 bước ở trên, bạn nhảy tới bước cần sửa, chỉnh rồi bấm **"Lưu thay đổi"**.

> **Sửa khách sạn đang bán KHÔNG làm nó biến mất khỏi website.** Khi bạn sửa một khách sạn đã "Đang xuất bản", nó vẫn giữ nguyên trạng thái đó — không bị đẩy về "Chờ duyệt" hay bị ẩn đi. Bạn cứ yên tâm chỉnh sửa.

## Tạm ẩn & Xoá khách sạn

Mở nút **ba chấm (⋮)** trên thẻ khách sạn:

- **"Ẩn khỏi website"** — tạm gỡ khách sạn khỏi website mà không xoá. Nó chuyển về dạng nháp, hiện badge **"Chưa hiển thị"**. Muốn bán lại thì mở ra và đăng lại.
- **"Nhân bản"** — tạo một bản sao để đỡ phải nhập lại từ đầu khi bạn có nhiều khách sạn giống nhau.
- **"Xoá"**:
  - Xoá một **bản nháp** = xoá **vĩnh viễn**, không lấy lại được.
  - Xoá một khách sạn **đã đăng** = đưa vào **thùng rác**, vẫn khôi phục được.

> **Lỡ xoá khách sạn đã đăng?** Nó nằm trong mục **Khôi phục** (thùng rác) của khu nhà cung cấp, bạn lấy lại được. Nhưng **bản nháp thì xoá là mất luôn** — hãy cân nhắc trước khi xoá nháp.

## Lưu ý & xử lý sự cố

**Bấm "Thêm khách sạn" nhưng không vào được / không thấy nút:** kiểm tra thanh menu có mục **Hotel** không. Không có nghĩa là bạn chưa mua gói dịch vụ.

**Đăng xong mà ngoài website không thấy khách sạn:** kiểm tra lần lượt:
1. Trạng thái có phải **"Đang xuất bản"** không? Nếu "Chờ duyệt" thì đợi quản trị viên; nếu "Bản nháp" thì bạn chưa nhập đủ mục bắt buộc (các mục có dấu ⭐).
2. Đã tạo **ít nhất một loại phòng** chưa? Không có phòng, khách không đặt được.
3. Đã **mở bán ngày nào** cho phòng chưa (xem bài Phòng)?
4. Thử tải lại trang bằng **Ctrl + F5**.

**Nhập giá bị sai số:** gõ số thuần, không thêm dấu chấm phân cách hay chữ "đ". Ví dụ gõ `1200000` chứ đừng gõ `1.200.000đ`.

**Tải ảnh mãi không lên:** ảnh quá nặng, hãy giảm còn khoảng 1–2 MB rồi tải lại.

**Bị đá sang trang Gói dịch vụ khi đăng:** gói của bạn hết hạn hoặc hết lượt. Vào mục **Gói dịch vụ** để gia hạn/nâng gói.

## Xem thêm

- [Khu Nhà cung cấp (tổng quan)](README.md)
- [Nhập & quản lý phòng](phong.md)
- [Nhập & quản lý tour](tour.md)
