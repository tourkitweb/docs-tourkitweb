# 4.6. Menu

> **ĐỌC KỸ DÒNG NÀY TRƯỚC — đây là chỗ gây nhầm lẫn nhiều nhất:**
>
> Mục này quản lý **thanh menu hiển thị TRÊN WEBSITE cho KHÁCH XEM** — cái thanh ngang trên đầu trang chủ có các chữ như *Trang chủ, Tour, Khách sạn, Tin tức, Liên hệ*, và cả các cột liên kết ở cuối trang.
>
> **KHÔNG PHẢI** cột menu màu tối bên trái mà bạn đang dùng để quản trị. Cột đó là menu quản trị, do hệ thống tự sinh theo phân quyền, **bạn không sửa được và cũng không cần sửa**.
>
> Nhớ đơn giản: **sửa ở đây là sửa cái KHÁCH nhìn thấy, không phải cái BẠN nhìn thấy.**

Vậy dùng mục này khi nào? Khi bạn muốn:

- Thêm mục **"Tour Nhật Bản"** lên thanh menu vì bạn vừa mở tuyến mới.
- Bỏ mục **"Thuê xe"** xuống vì bạn không kinh doanh mảng đó nữa.
- Đổi thứ tự: đưa **"Khách sạn"** lên trước **"Tin tức"** vì khách quan tâm khách sạn hơn.
- Gom nhiều tour thành một menu con xổ xuống cho gọn.

> **Đường dẫn:** Menu bên trái > **Hệ thống** > **Menu**

![](../.gitbook/assets/pg129-0.png)

## Trong mục này có gì?

- **Danh sách menu** — nơi bạn tạo và sửa nội dung các menu.
- **Vị trí đặt menu** — nơi khai báo các "chỗ trống" trên giao diện mà menu có thể nằm vào.

## Hiểu 2 khái niệm trước khi bắt tay làm

Nhiều người vào đây rồi loay hoay vì không phân biệt được hai thứ này. Hãy dành 1 phút đọc:

**Menu** = **nội dung**, tức là *danh sách các mục gì, theo thứ tự nào*. Ví dụ menu tên "Menu chính" gồm: Trang chủ → Tour → Khách sạn → Liên hệ.

**Vị trí đặt menu** = **chỗ để**, tức là *cái menu đó nằm ở đâu trên giao diện*. Ví dụ: vị trí "Đầu trang", vị trí "Cuối trang".

Ví von cho dễ nhớ: **Menu là bức tranh, Vị trí là cái đinh trên tường.** Bạn vẽ tranh xong (tạo menu) mà không treo lên đinh nào (không gán vị trí) thì **không ai nhìn thấy bức tranh của bạn cả**.

> **Đây chính là lý do phổ biến nhất khiến người ta than "tôi tạo menu rồi mà web không hiện gì":** menu đã tạo xong nhưng chưa được gán vào vị trí nào.

**Một quy tắc quan trọng: mỗi vị trí chỉ giữ được MỘT menu.** Nếu vị trí "Đầu trang" đang treo Menu A, mà bạn gán Menu B vào đó, thì **Menu A tự động bị gỡ ra**. Menu A không bị xóa, nó vẫn còn trong danh sách, chỉ là không còn hiện trên web nữa.

## Danh sách menu

Màn hình này liệt kê các menu bạn đã tạo, với các cột:

- **Tiêu đề (Title)** — tên menu. Bấm vào tên là mở ra để sửa.
- **Use for** (Dùng cho) — cột **quan trọng nhất**: cho biết menu này **đang được treo ở vị trí nào**. Nếu cột này **trống**, nghĩa là menu đó chưa treo ở đâu cả — khách không nhìn thấy nó. Đây là chỗ đầu tiên nên nhìn khi menu không hiện trên web.
- **Hiển thị** — công tắc bật/tắt nhanh.
- **Ngày (Date)** — lần sửa gần nhất.

Có nút **"Add new"** (Thêm mới) để tạo menu mới, và hành động hàng loạt (chỉ có lệnh **Xóa**).

> **Mẹo:** Hầu hết website chỉ cần **2 menu**: một cho đầu trang, một cho cuối trang. Đừng tạo nhiều menu rồi rối. Nếu bạn chỉ muốn **thêm một mục** vào thanh menu hiện có, **đừng tạo menu mới** — hãy mở menu đang có sẵn ra và thêm mục vào đó.

## Sửa nội dung một menu

Bấm vào tên menu để mở ra. Màn hình chia làm 2 phần: **cột trái** là kho nguyên liệu, **phần giữa** là menu của bạn.

### Bước 1: Chọn thứ muốn thêm (cột trái)

Cột trái là các hộp chứa những thứ bạn có thể đưa vào menu:

- **Trang (Page)** — các trang tĩnh: Giới thiệu, Liên hệ, Điều khoản…
- **Địa điểm (Location)** — các điểm đến: Hà Nội, Đà Nẵng, Phú Quốc…
- **Tin tức (News)** và **Danh mục tin tức** — bài viết và nhóm bài viết.
- **Các loại dịch vụ bạn đang bán** — tùy website của bạn bật những module nào, có thể có: Tour, Khách sạn, Xe, Du thuyền, Sự kiện, Vé máy bay, Không gian, Visa, Bất động sản, Khóa học…
- **Custom Url** (Đường dẫn tùy chỉnh) — dùng khi bạn muốn trỏ tới **bất kỳ địa chỉ nào**, kể cả trang ngoài website (ví dụ trang Facebook của công ty). Bạn nhập 2 thứ: **URL** (địa chỉ) và **Link Text** (chữ hiện trên menu).

### Bước 2: Thêm vào menu

Trong mỗi hộp có ô **tìm kiếm** — gõ tên thứ bạn cần (ví dụ gõ `Hạ Long` trong hộp Tour). Tích chọn rồi nhấn nút **"Add to Menu"** (Thêm vào menu). Nó sẽ nhảy sang phần giữa.

### Bước 3: Sắp xếp bằng cách kéo thả

Đây là phần thú vị nhất và cũng dễ làm nhất: bạn **dùng chuột kéo các mục lên xuống** để đổi thứ tự.

**Muốn tạo menu con xổ xuống?** Kéo một mục và **thả nó vào bên trong, thụt lề dưới một mục khác**. Nó sẽ thành mục con. Ví dụ kéo "Tour Nhật Bản" vào dưới "Tour" → khách rê chuột vào "Tour" sẽ thấy "Tour Nhật Bản" xổ ra.

> **Mẹo cho người mới:** Kéo thả cần một chút quen tay. Hãy giữ chuột vào **chỗ có biểu tượng để kéo** trên mục đó, giữ nguyên và di chuyển từ từ — đừng kéo giật. Nếu kéo hỏng, cứ kéo lại, **chưa bấm lưu thì chưa có gì thay đổi trên web cả**. Cứ thử thoải mái.

### Bước 4: Sửa chi tiết từng mục

Bấm vào một mục trong menu để mở ra các tùy chọn:

- **Label** (Nhãn) — **chữ hiện ra cho khách đọc**. Đây là thứ bạn hay cần sửa nhất. Ví dụ mục tour tên đầy đủ dài dòng, bạn sửa Label thành `Hạ Long` cho gọn. **Sửa Label không làm đổi tên tour gốc**, chỉ đổi chữ trên menu.
- **URL** (Địa chỉ) — chỉ sửa được với mục Custom Url. Với các mục khác, hệ thống tự biết đường dẫn.
- **Class** — dành cho kỹ thuật, để trống.
- **Target** (Mở ở đâu) — chọn **Normal** (mở trong cùng cửa sổ) hoặc **Open new tab** (mở tab mới). Với mục trỏ ra ngoài (Facebook, đối tác), nên chọn **Open new tab** để khách không rời khỏi web của bạn.
- **Icon Html** — thêm biểu tượng nhỏ, dành cho kỹ thuật.
- **Enable mega menu** (Bật mega menu) — "mega menu" là loại menu xổ xuống **to như một tấm bảng nhiều cột**, thay vì một danh sách dọc thông thường. Dùng khi bạn có rất nhiều mục con. Bật lên thì có thêm: **Columns** (số cột, từ 2 đến 12) và **Mega image url** (ảnh minh họa trong bảng đó).
- **Nút Delete** — gỡ mục này khỏi menu. **Chỉ gỡ khỏi menu thôi, tour/khách sạn gốc vẫn còn nguyên trong hệ thống** — đừng lo.

> **Mẹo về mega menu:** Đừng bật nếu chỉ có 3-4 mục con — một bảng to đùng xổ ra cho 3 dòng chữ nhìn rất trống trải. Chỉ dùng khi bạn có từ 8-10 mục con trở lên. Và về số cột: đừng chọn 12 cột, mỗi cột sẽ hẹp tới mức chữ bị cắt vụn. **3 hoặc 4 cột** là hợp lý cho hầu hết trường hợp.

### Bước 5: Gán vị trí và Lưu — bước quyết định

Trong màn hình sửa menu có phần liệt kê các **vị trí** dưới dạng ô tích. Tích vào vị trí bạn muốn menu này hiện ra (ví dụ: Đầu trang), rồi **nhấn Lưu**.

> **Nhắc lại lần cuối:** Không tích vị trí nào = menu không hiện trên web, dù bạn đã sắp xếp đẹp đến mấy.
>
> **Và nhớ:** tích vào một vị trí đang có menu khác thì menu cũ **tự động bị gỡ khỏi vị trí đó**. Nếu bạn tích bừa, thanh menu đầu trang của bạn có thể **đổi hoàn toàn ngay lập tức** cho mọi khách đang xem web. Hãy chắc chắn trước khi tích.

## Vị trí đặt menu

Đây là nơi khai báo **các "chỗ trống" trên giao diện** mà menu có thể nằm vào — ví dụ "Đầu trang", "Cuối trang cột 1", "Cuối trang cột 2".

> **Bạn gần như không cần động vào mục này.** Các vị trí đã được đơn vị triển khai thiết lập sẵn cho khớp với giao diện bạn đang dùng. Việc của bạn chỉ là **tích chọn vị trí** khi sửa menu.
>
> **Cẩn thận:** Đừng tự tạo vị trí mới. Vị trí phải khớp với cách giao diện được thiết kế — tạo một vị trí mà giao diện không biết đến thì nó **không hiện ra ở đâu cả**, và bạn sẽ ngồi tìm mãi không hiểu menu của mình biến đi đâu. Nếu bạn cần một chỗ đặt menu mới, hãy liên hệ đơn vị triển khai.

## Lưu ý & xử lý sự cố

**Tôi sửa menu ở đây nhưng cột menu bên trái (menu quản trị) không đổi.**
Đúng như vậy, và đây không phải lỗi. Hai cái đó **hoàn toàn khác nhau**. Mục này chỉ sửa menu trên website cho khách. Menu quản trị bên trái do hệ thống tự sinh theo phân quyền của bạn — muốn đổi những gì hiện ở đó, phải chỉnh **vai trò và quyền** tại [4.1. Người dùng](nguoi-dung.md).

**Tôi tạo menu xong nhưng ngoài web không thấy gì.**
Kiểm tra theo thứ tự này:

1. **Menu chưa được gán vị trí** — nguyên nhân số 1. Mở menu ra, tích chọn một vị trí, lưu lại. Hoặc nhìn cột **"Use for"** ở màn hình danh sách: trống nghĩa là chưa treo ở đâu.
2. **Công tắc "Hiển thị" đang tắt** — bật lên ở màn hình danh sách.
3. **Chưa nhấn Lưu** — kéo thả xong phải lưu.
4. **Trình duyệt giữ bản cũ** — nhấn **Ctrl + F5** trên trang web.

**Thanh menu đầu trang của tôi tự nhiên đổi hết!**
Ai đó (có thể là chính bạn) vừa gán một menu khác vào vị trí "Đầu trang", khiến menu cũ bị gỡ ra. Menu cũ **không mất**, vẫn nằm trong danh sách. Chỉ cần mở menu cũ ra, tích lại vị trí "Đầu trang" và lưu là mọi thứ trở lại như xưa.

**Kéo thả mãi không được, mục không chịu nhảy đúng chỗ.**
Hãy giữ chuột đúng vào biểu tượng kéo trên mục, di chuyển **chậm rãi**, và thả khi thấy chỗ trống hiện ra đúng vị trí mong muốn. Nếu vẫn khó, thử phóng to cửa sổ trình duyệt. Kéo thả trên **màn hình cảm ứng hoặc điện thoại rất khó** — hãy dùng máy tính có chuột cho việc này.

**Tôi xóa nhầm một mục khỏi menu.**
Bình tĩnh: bạn chỉ gỡ nó khỏi menu, **tour/khách sạn/bài viết gốc vẫn còn nguyên** trong hệ thống. Nếu **chưa bấm Lưu**, chỉ cần tải lại trang là mọi thứ trở về như cũ. Nếu đã lưu, hãy tìm lại nó ở cột trái và thêm vào menu lần nữa.

**Menu trên điện thoại nhìn khác trên máy tính.**
Đây là chuyện bình thường và cố ý. Màn hình điện thoại hẹp nên menu thường thu lại thành **biểu tượng ba gạch ngang (☰)**, bấm vào mới xổ ra. Không phải lỗi.

**Menu quá nhiều mục, tràn ra xấu.**
Hãy gom bớt thành **menu con** (kéo thụt vào dưới một mục cha). Thanh menu đầu trang lý tưởng chỉ nên có **5 đến 7 mục chính**. Nhiều hơn thì khách rối và không biết bấm vào đâu.

## Xem thêm

- [4. Khối HỆ THỐNG](README.md)
- [4.7. Giao diện](giao-dien.md)
