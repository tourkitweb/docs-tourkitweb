# 4.17. SEO

**SEO** là làm cho website dễ được Google tìm thấy và xếp hạng cao. Bộ công cụ SEO của hệ thống (gọi là **SEO Pro**) **miễn phí và có sẵn trên mọi website** — bạn không phải mua hay cài thêm gì. Nó gồm hai phần:

* **Khung SEO trong từng bài viết, tour, khách sạn, địa điểm** — nơi điền tiêu đề, mô tả hiện trên Google, có chấm điểm tự động. Cách dùng xem [Đăng bài chuẩn SEO](../khoi-noi-dung/tin-tuc.md#dang-bai-chuan-seo).
* **Mục SEO trên menu quản trị** — các công tắc dùng chung cho cả website: chặn Google khi đang lên bài, Sitemap, xác minh Google, chuyển hướng link cũ. Đây là nội dung của trang này.

Các tính năng trong SEO Pro **dùng hay không là do bạn chọn**: bật cái nào thì cái đó chạy, tắt thì hệ thống không làm gì với nó.

> **Đường dẫn:** Menu bên trái > **SEO** > **SEO Settings** (Cài đặt SEO) hoặc **Redirects** (Chuyển hướng)

> **Không thấy mục "SEO" trong menu?** Tài khoản của bạn chưa được cấp quyền quản lý SEO. Hãy nhờ quản trị viên cấp quyền, hoặc nhờ họ làm giúp.

> 📷 *[Cần chụp màn hình: trang SEO Settings — phần "Chặn Google khi đang lên bài" và phần "Sitemap" với ô "Bật Sitemap"]*

***

## Cài đặt SEO (SEO Settings)

Trang này gồm nhiều khung xếp từ trên xuống. Chỉnh xong khung nào cũng phải bấm nút xanh **"Lưu cài đặt"** ở cuối trang thì mới có hiệu lực.

### Chặn Google khi đang lên bài

**Dùng khi nào:** website mới, đang nhập nội dung — giá chưa chuẩn, ảnh còn ảnh mẫu, bài còn dở. Nếu Google ghé vào lúc này, nó sẽ đưa những trang dở dang đó lên kết quả tìm kiếm và **nhớ rất lâu**. Bật chế độ này là bảo Google: "chưa xong, đừng đưa trang nào lên".

**Cách bật:** ở ô **"Chế độ đang lên bài (chặn Google index toàn website)"**, chọn **"Bật — chặn Google index mọi trang"** → bấm **"Lưu cài đặt"**.

Khi chế độ đang bật:

* **Mọi trang** của website được gắn lệnh "đừng đưa lên Google" — kể cả bài bạn điền SEO đầy đủ, kể cả bài đang để ô **"Cho phép search engine index?"** là **"Có"**.
* Thanh trên cùng của **mọi màn hình quản trị** hiện nút đỏ **"Đang chặn Google"** — bấm vào là tới thẳng chỗ tắt.
* Khung SEO trong từng bài có dải vàng nhắc "Website đang bật Chặn Google…".
* Khách có link **vẫn vào xem website bình thường**. Chế độ này chỉ chặn Google, không khoá website.

**Khi sẵn sàng ra mắt:** chọn **"Tắt — cho Google index bình thường"** → **"Lưu cài đặt"**. Nút đỏ trên thanh quản trị biến mất là xong. Google sẽ bắt đầu ghé lại trong vài ngày tới vài tuần; muốn nhanh hơn, xem phần [Gửi sitemap cho Google](#gui-sitemap-cho-google) bên dưới.

> **Tuyệt đối đừng bật trên website đang chạy thật.** Các trang đã có trên Google sẽ **bị gỡ dần khỏi kết quả tìm kiếm**, khách tìm không ra bạn nữa. Lỡ bật nhầm vài ngày thì sau khi tắt có khi phải chờ nhiều tuần mới lấy lại thứ hạng cũ.

> **Lỗi hay gặp nhất là QUÊN TẮT.** Website đã ra mắt cả tháng mà Google không có trang nào — vì chế độ này vẫn bật. Hãy để ý nút đỏ **"Đang chặn Google"** trên thanh quản trị: còn thấy nó nghĩa là website vẫn đang chặn.

### Sitemap (sơ đồ website)

**Sitemap là gì:** một "danh bạ" liệt kê mọi bài viết, tour, khách sạn… trên website, đặt ở địa chỉ `tenmien.com/sitemap_index.xml`. Google đọc danh bạ này để biết website có những trang nào, nhờ vậy tìm ra trang mới nhanh hơn — nhất là website có hàng trăm, hàng nghìn sản phẩm.

Ô **"Bật Sitemap"** có 2 lựa chọn:

| Lựa chọn | Hệ thống làm gì |
| --- | --- |
| **Bật — dựng sitemap và tự cập nhật mỗi đêm** | Dựng sitemap **ngay sau khi bạn lưu** (website nhiều sản phẩm có thể mất vài phút). Sau đó **tự dựng lại mỗi đêm** (khoảng 3 giờ 30 sáng) — bài, tour, khách sạn mới đăng trong ngày sẽ có trong sitemap từ sáng hôm sau. |
| **Tắt — không dùng sitemap** | **Xoá** sitemap ngay khi lưu. Địa chỉ `/sitemap_index.xml` báo không tồn tại, hệ thống không tự dựng nữa. |

> **Nên bật hay tắt?** Hầu hết website bán tour, khách sạn **nên bật**. Chỉ tắt khi website không cần (ví dụ website giới thiệu vài trang) hoặc đơn vị triển khai dặn tắt.

Bên dưới ô này còn có:

* **Bảng "Include featured image in sitemap"** — với từng loại nội dung (News, Tour, Hotel, Event, Cruise), chọn **Enabled** để đưa kèm ảnh đại diện vào sitemap. Nhờ vậy ảnh tour, khách sạn có cơ hội hiện ở **Google Hình ảnh**. Nên chọn **Enabled** cho Tour và Hotel.
* **Bảng "Sitemap Files"** — danh sách các tệp sitemap đang có và **lần cập nhật gần nhất**. Bấm vào tên tệp để mở xem.
* **Nút "Cập nhật Sitemap"** — dựng lại sitemap **ngay bây giờ**, không chờ tới đêm. Dùng khi vừa đăng bài/sản phẩm quan trọng muốn Google biết sớm. Sitemap đang tắt thì nút này bị mờ.

### Gửi sitemap cho Google

Bật sitemap xong, nên báo cho Google biết địa chỉ của nó (chỉ làm **một lần**):

1. Vào **Google Search Console** (`search.google.com/search-console`), đăng nhập bằng tài khoản Google của công ty, thêm website của bạn.
2. Google yêu cầu **xác minh** bạn là chủ website: chọn cách **"Thẻ HTML"**, Google đưa một dòng dạng `<meta name="google-site-verification" content="AbC123…" />`. Copy **chỉ phần mã** trong ngoặc kép sau `content=` (ví dụ `AbC123…`).
3. Dán mã đó vào ô **"Google Search Console Verification"** ở khung **"Social & Verification"** của trang này → **"Lưu cài đặt"** → quay lại Search Console bấm **Xác minh**.
4. Trong Search Console, mở mục **Sơ đồ trang web (Sitemaps)**, nhập `sitemap_index.xml` → **Gửi**.

> **Chỉ dán phần mã, không dán cả dòng `<meta …>`.** Dán cả dòng thì Google không xác minh được.

### Mạng xã hội & dữ liệu cho Google

* Khung **"Social & Verification"**:
  * **Facebook App ID**, **Twitter / X Site Handle** — dành cho kỹ thuật, **để trống** nếu đơn vị triển khai không dặn.
  * **Twitter Card Type** — để mặc định **Summary Large Image** (khung xem trước ảnh lớn khi chia sẻ link).
  * **Google Search Console Verification** — xem mục ngay trên.
* Khung **"JSON-LD Structured Data"** (dữ liệu có cấu trúc — giúp Google hiểu trang này là tour, khách sạn hay bài viết):
  * **Enable JSON-LD** — để **"Có"**.
  * **Site Type (Schema.org)** — loại hình doanh nghiệp. Công ty du lịch để **Travel Agency**.

***

## Chuyển hướng (Redirects)

**Dùng khi nào:** bạn đổi đường dẫn một bài/sản phẩm đã đăng lâu, hoặc xoá một trang cũ. Người đã lưu link cũ, và cả Google, vẫn sẽ vào địa chỉ cũ — và gặp trang lỗi. **Hệ thống không tự chuyển** địa chỉ cũ sang địa chỉ mới, bạn phải tạo một **chuyển hướng**: ai vào địa chỉ cũ sẽ được đưa sang địa chỉ mới, thứ hạng Google cũng được chuyển theo.

> **Đường dẫn:** Menu bên trái > **SEO** > **Redirects**

**Cách thêm:**

1. Bấm **"Add Redirect"** ở góc trên bên phải.
2. **From URL** — địa chỉ cũ, chỉ phần sau tên miền, **bắt đầu bằng dấu `/`**. Ví dụ `/tin-tuc/khuyen-mai-he-2025`.
3. **To URL** — địa chỉ mới. Có thể là phần sau tên miền (`/tin-tuc/khuyen-mai-he-2026`) hoặc địa chỉ đầy đủ.
4. **Redirect Type** — chọn **"301 – Permanent"** (chuyển vĩnh viễn, thứ hạng Google chuyển theo). Chỉ chọn **"302 – Temporary"** khi chuyển tạm vài hôm rồi sẽ quay lại địa chỉ cũ.
5. **Status** — để **"Kích hoạt"**.
6. **Ghi chú** (không bắt buộc) — ghi lý do để sau này người khác hiểu.
7. Bấm **"Tạo"**.

Màn hình danh sách cho bạn **tìm theo địa chỉ** (ô **"Search URL..."**), xem cột **Hits** (số lần có người đi qua chuyển hướng này), sửa hoặc xoá.

> **Tránh chuyển hướng nối đuôi** (A → B, rồi lại B → C). Khi đổi đường dẫn lần nữa, hãy sửa chuyển hướng cũ để A trỏ thẳng tới C.

***

## Lưu ý & xử lý sự cố

**Bật Sitemap, lưu xong mà bảng "Sitemap Files" vẫn trống.** Hệ thống đang dựng sitemap ở phía sau — website nhiều sản phẩm có thể mất vài phút. Chờ một lúc rồi tải lại trang (**F5**).

**Mở `tenmien.com/sitemap_index.xml` báo không tồn tại.** Sitemap đang **tắt**, hoặc vừa bật mà chưa dựng xong. Kiểm tra ô **"Bật Sitemap"**, chờ vài phút rồi thử lại.

**Thanh trên cùng trang quản trị có nút đỏ "Đang chặn Google".** Chế độ "đang lên bài" đang bật — Google không đưa trang nào của bạn lên. Nếu website đã ra mắt, bấm vào nút đó và chọn **"Tắt"** ngay.

**Đã tắt chế độ chặn Google mà vẫn chưa thấy website trên Google.** Google cần thời gian ghé lại, thường vài ngày tới vài tuần. Gửi sitemap qua Google Search Console (mục [Gửi sitemap cho Google](#gui-sitemap-cho-google)) để Google biết sớm hơn.

**Đã tạo chuyển hướng mà vào link cũ vẫn ra trang lỗi.** Kiểm tra: **From URL** có bắt đầu bằng dấu `/` và gõ đúng từng ký tự không; **Status** có đang là **"Kích hoạt"** không. Trình duyệt cũng hay nhớ trang cũ — nhấn **Ctrl + F5** hoặc thử bằng cửa sổ ẩn danh.

**Xác minh Google Search Console báo thất bại.** Thường do dán cả dòng `<meta …>` thay vì chỉ phần mã, hoặc quên bấm **"Lưu cài đặt"** trước khi bấm Xác minh.

## Xem thêm

* [2.1. Tin tức — Đăng bài chuẩn SEO](../khoi-noi-dung/tin-tuc.md#dang-bai-chuan-seo) — khung SEO trong từng bài
* [3.1. Địa điểm](../khoi-san-pham/dia-diem.md) — các trang theo địa điểm dùng để lên top Google
* [4.9. Cài đặt](cai-dat.md)
