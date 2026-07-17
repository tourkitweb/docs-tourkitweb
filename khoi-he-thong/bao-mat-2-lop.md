# 4.12. Bảo mật 2 lớp

Mật khẩu thôi là chưa đủ. Mật khẩu có thể bị lộ: bạn dùng chung một mật khẩu cho nhiều nơi, nhân viên cũ vẫn nhớ, ai đó nhìn trộm lúc bạn gõ, hoặc bạn lỡ bấm vào một đường link lừa đảo.

**Bảo mật 2 lớp** thêm một lớp khóa thứ hai: sau khi nhập đúng mật khẩu, hệ thống hỏi thêm **một mã 6 số** chỉ có trên điện thoại của bạn. Kẻ gian dù biết mật khẩu nhưng không cầm điện thoại của bạn thì vẫn **không vào được**.

> **Đường dẫn:** Menu bên trái > **Bảo mật 2 lớp**

## Hiểu cho dễ: nó giống hệt cái bạn đã dùng ở ngân hàng

Bạn chuyển khoản qua app ngân hàng chưa? Nhập xong số tiền, app hỏi thêm **mã OTP**. Đó chính xác là bảo mật 2 lớp.

Chỉ có **một điểm khác** so với ngân hàng, và bạn cần nhớ điều này:

| | **Ngân hàng (OTP qua SMS)** | **Ở đây (ứng dụng xác thực)** |
|---|---|---|
| Mã đến từ đâu? | Tin nhắn SMS gửi về máy | **Ứng dụng tự sinh ra ngay trên điện thoại** |
| Cần sóng/mạng không? | **Có**, phải có sóng để nhận tin | **Không cần**. Máy bay, ra nước ngoài, hết tiền điện thoại — vẫn có mã |
| Mã sống bao lâu? | Vài phút | **30 giây**, hết 30 giây tự đổi mã mới |

Điểm cần nhớ: **mã KHÔNG được gửi tới bạn**. Bạn phải **tự mở ứng dụng ra để xem**. Rất nhiều người ngồi chờ tin nhắn SMS mãi không thấy — vì sẽ **không bao giờ có** tin nhắn nào cả.

> 📷 *[Cần chụp màn hình: trang "2FA của tôi" tại Bảo mật 2 lớp > 2FA của tôi, hiển thị mã QR và ô nhập mã 6 số]*

## Trong mục này có gì?

Nhấn vào **Bảo mật 2 lớp** ở menu bên trái, bạn sẽ thấy tối đa 3 mục con:

- **2FA của tôi** — nơi **bạn** thiết lập bảo mật 2 lớp cho chính tài khoản mình. Đây là mục hầu hết mọi người dùng.
- **Quản lý admin** — dành cho **quản trị viên cấp cao**, để cấp/gỡ bảo mật 2 lớp cho các tài khoản khác.
- **Cấu hình** — dành cho **quản trị viên cấp cao**, chỉnh các thông số kỹ thuật.

> **Bạn chỉ thấy 1 mục "2FA của tôi"?** Đó là bình thường và đúng — bạn là người dùng thường, chỉ quản lý được tài khoản của mình.
>
> **Không thấy menu "Bảo mật 2 lớp" đâu cả?** Tài khoản của bạn chưa được cấp quyền nào liên quan. Toàn bộ menu sẽ ẩn đi. Hãy liên hệ quản trị viên của đơn vị bạn.

## ĐIỀU QUAN TRỌNG NHẤT PHẢI BIẾT TRƯỚC

Hãy đọc kỹ phần này trước khi làm bất cứ điều gì.

### 1. Bạn KHÔNG tự bật được bảo mật 2 lớp cho mình

Hệ thống này thiết kế khác với Facebook hay Google. Bạn **không tự bật** được.

**Quản trị viên cấp cao phải "Cấp QR" cho bạn trước.** Họ tạo mã QR rồi gửi cho bạn, sau đó bạn mới quét được. Nếu bạn vào **"2FA của tôi"** mà không thấy mã QR nào, nghĩa là **chưa ai cấp cho bạn** — hãy liên hệ quản trị viên, đừng loay hoay tìm nút bật.

### 2. ⚠️ MẤT ĐIỆN THOẠI = MẤT QUYỀN TRUY CẬP

Đây là cảnh báo nghiêm túc nhất của cả bài viết, xin bạn đọc chậm:

**Hệ thống này KHÔNG có mã dự phòng (recovery code).** Bạn có thể đã nghe nói về "mã dự phòng" ở các dịch vụ khác — **ở đây không có**. Không có danh sách mã để in ra cất tủ.

Nghĩa là: **mất điện thoại, đổi điện thoại mới, hay lỡ tay xóa ứng dụng xác thực → bạn không còn cách nào tự lấy lại mã.** Không có nút "gửi mã qua email", không có câu hỏi bí mật.

**Cách duy nhất để lấy lại:** liên hệ **quản trị viên cấp cao** để họ **cấp lại mã QR mới** cho bạn.

**Vậy nếu bạn CHÍNH LÀ quản trị viên cấp cao duy nhất và mất điện thoại thì sao?** Bạn phải nhờ **đơn vị triển khai kỹ thuật** can thiệp trực tiếp vào hệ thống. Việc này mất thời gian và không phải lúc nào cũng làm được ngay.

### 3. Ba việc phải làm để tự bảo vệ mình

Vì không có mã dự phòng, hãy tự lo trước:

1. **Chụp màn hình mã QR và cất giữ nơi an toàn** ngay khi được cấp. Có ảnh QR này, bạn cài lại lên điện thoại mới lúc nào cũng được.
   > **Nơi an toàn nghĩa là:** một thư mục riêng tư trên máy tính có mật khẩu, hoặc in ra cất trong két. **KHÔNG** gửi vào nhóm Zalo, **KHÔNG** để trong album ảnh chung, **KHÔNG** đăng lên đâu cả. Ai có ảnh QR đó là **có luôn quyền sinh mã như bạn**.

2. **Chép lại "khóa bí mật" (dãy chữ và số hiện cạnh mã QR)** và cất cùng chỗ. Nó có tác dụng y hệt mã QR, dùng khi bạn không quét được QR mà phải gõ tay.

3. **Đảm bảo có ÍT NHẤT HAI quản trị viên cấp cao** trong đơn vị. Nếu chỉ có một người và người đó mất điện thoại, cả công ty mắc kẹt. Có hai người thì họ cấp lại QR cho nhau được.

## Cài ứng dụng xác thực trên điện thoại

Trước khi làm gì, bạn cần có ứng dụng này trên điện thoại. Nó **hoàn toàn miễn phí**.

### Bước 1: Tải ứng dụng

Hệ thống hướng dẫn dùng **Google Authenticator**. Hãy dùng đúng ứng dụng này cho khớp với hướng dẫn.

- **Điện thoại Android:** mở **CH Play** (Google Play), gõ tìm `Google Authenticator`.
- **Điện thoại iPhone:** mở **App Store**, gõ tìm `Google Authenticator`.

Nhận diện: biểu tượng hình **dấu hoa thị / ngôi sao nhiều cánh màu xanh dương và xám**, nhà phát hành ghi rõ là **Google LLC**.

> **Cẩn thận:** Trên cửa hàng có **rất nhiều ứng dụng nhái** tên na ná, có cái còn tính phí hoặc đánh cắp dữ liệu. Hãy nhìn kỹ **tên nhà phát hành phải là Google LLC** và ứng dụng phải **miễn phí**. Thấy đòi trả tiền là tải nhầm.

### Bước 2: Mở ứng dụng lên

Mở ra, nếu nó hỏi đăng nhập tài khoản Google thì bạn có thể **bỏ qua** cũng được — ứng dụng vẫn chạy bình thường mà không cần đăng nhập.

Lần đầu mở, màn hình sẽ trống trơn. **Đúng rồi đấy**, chưa có gì cả. Bạn sẽ thêm ở bước sau.

> 📷 *[Cần chụp màn hình: giao diện ứng dụng Google Authenticator trên điện thoại, hiển thị mã 6 số kèm vòng tròn đếm ngược]*

## Thiết lập bảo mật 2 lớp cho tài khoản của bạn

### Bước 1: Xin mã QR từ quản trị viên

Như đã nói ở trên, bạn không tự tạo được. Hãy nhắn cho quản trị viên cấp cao của đơn vị: *"Anh/chị cấp QR bảo mật 2 lớp cho tài khoản của em nhé."*

Họ sẽ vào **Bảo mật 2 lớp > Quản lý admin**, tìm tên bạn và bấm **"Cấp QR"**, rồi gửi mã QR cho bạn.

### Bước 2: Mở trang "2FA của tôi"

Vào **Menu bên trái > Bảo mật 2 lớp > 2FA của tôi**.

Bạn sẽ thấy **một hình vuông đen trắng loang lổ** — đó chính là mã QR. Bên cạnh thường có một **dãy chữ và số** (khóa bí mật).

> **Trang trống, không có QR?** Quản trị viên chưa cấp cho bạn. Quay lại Bước 1.
>
> **Ngay lúc này, hãy chụp màn hình trang này lại** và cất nơi an toàn, như đã dặn ở phần cảnh báo phía trên. Đừng bỏ qua, đây là "phao cứu sinh" duy nhất của bạn.

> 📷 *[Cần chụp màn hình: trang 2FA của tôi hiển thị mã QR cùng khóa bí mật dạng chữ và số]*

### Bước 3: Quét mã QR bằng điện thoại

1. **Cầm điện thoại**, mở ứng dụng **Google Authenticator**.
2. Nhấn dấu **cộng (+)**, thường ở góc dưới bên phải.
3. Chọn **"Quét mã QR"** (Scan a QR code).
4. Nếu máy hỏi xin quyền dùng camera, chọn **"Cho phép"**.
5. **Đưa camera điện thoại hướng vào màn hình máy tính**, ngắm sao cho mã QR nằm gọn trong khung.

Chỉ sau 1-2 giây, ứng dụng sẽ **tự nhận** và thêm một dòng mới, hiển thị **6 chữ số** kèm một vòng tròn đang đếm ngược.

> **Không quét được? Có 2 cách xử lý:**
>
> **Cách 1 — chỉnh lại camera:** tăng độ sáng màn hình máy tính lên tối đa, lau ống kính camera, đưa điện thoại cách màn hình khoảng **20-30cm**, giữ tay cho vững đừng rung.
>
> **Cách 2 — nhập tay (chắc ăn hơn):** trong ứng dụng, thay vì chọn "Quét mã QR", chọn **"Nhập khóa thiết lập"** (Enter a setup key). Sau đó gõ **dãy chữ và số** hiện bên cạnh mã QR trên màn hình. Gõ chậm, đừng nhầm số `0` với chữ `O`, số `1` với chữ `l`.

### Bước 4: Nhập mã 6 số để xác nhận

Nhìn vào ứng dụng trên điện thoại, bạn thấy **6 chữ số** — ví dụ `284 913`.

Gõ 6 số đó vào **ô nhập mã** trên màn hình máy tính, rồi bấm nút xác nhận.

**Lưu ý khi gõ:**
- **Không gõ dấu cách.** Ứng dụng hiển thị `284 913` cho dễ đọc, nhưng bạn gõ liền: `284913`.
- **Nhìn vòng tròn đếm ngược.** Nếu nó sắp hết (chỉ còn vài giây), **hãy chờ mã mới rồi hãy gõ**. Gõ đúng lúc mã đổi thì hệ thống sẽ báo sai.
- Gõ xong bấm xác nhận **ngay**, đừng đi pha trà rồi quay lại.

Nếu thành công, hệ thống sẽ báo tài khoản của bạn đã được xác nhận. **Xong!** Từ giờ mỗi lần thực hiện thao tác quan trọng, bạn chỉ cần mở ứng dụng lấy mã.

### Bước 5: Kiểm tra lại — đừng bỏ qua

Trước khi bạn coi như xong, hãy chắc chắn nó thật sự chạy. Đây là lúc tốt nhất để phát hiện sai sót — chứ không phải lúc bạn đang cần gấp giữa đêm.

Nếu chưa xác nhận thành công, bạn sẽ **không thực hiện được các thao tác quan trọng** như **thanh toán lại đơn hàng (retry payment)** hay **hoàn tiền cho khách (refund)** — hệ thống sẽ chặn lại và hỏi mã.

## Dùng hằng ngày như thế nào?

Sau khi cài xong, mọi thứ rất đơn giản:

1. Khi hệ thống hỏi mã, một ô nhập 6 số sẽ hiện ra.
2. **Mở ứng dụng Google Authenticator** trên điện thoại.
3. Đọc 6 số đang hiện, gõ vào ô, bấm xác nhận.

Chỉ vậy thôi. Mất khoảng 10 giây.

> **Bạn không cần internet trên điện thoại để lấy mã.** Ứng dụng tự tính mã dựa trên đồng hồ, không cần mạng. Ra nước ngoài, đi máy bay, hết data — vẫn dùng bình thường.

> **Mã đổi liên tục là bình thường.** Cứ 30 giây mã tự đổi thành số khác. Bạn không làm gì sai cả. Cứ dùng mã đang hiện tại thời điểm gõ.

## Dành cho quản trị viên cấp cao

Phần này chỉ dành cho người có quyền quản trị. Nếu bạn chỉ thấy mục **"2FA của tôi"**, bạn có thể bỏ qua phần này.

### Quản lý admin

> **Đường dẫn:** Menu bên trái > **Bảo mật 2 lớp** > **Quản lý admin**

Trang này liệt kê **tất cả những người có quyền vào trang quản trị**, kèm tình trạng bảo mật 2 lớp của từng người. Bạn nhìn một cái là biết ai đã cài, ai chưa.

Với mỗi người, bạn có các thao tác:

- **"Cấp QR" / "Cấp lại QR"** — tạo mã QR mới cho người đó. Đây là việc bạn làm khi có nhân viên mới, hoặc khi ai đó mất điện thoại.
  > **Cẩn thận:** Bấm **"Cấp lại QR"** sẽ **hủy ngay lập tức** mã QR cũ của người đó. Nếu họ đang dùng bình thường mà bạn lỡ tay bấm, **họ sẽ không đăng nhập được nữa** cho đến khi quét lại mã mới. Hãy chắc chắn bạn đang bấm đúng dòng của đúng người.

- **"Xem QR"** — mở lại mã QR đã cấp để gửi cho người dùng.
  > **Cẩn thận khi gửi QR cho nhân viên:** mã QR này giống như **chìa khóa tài khoản của họ**. Hãy gửi qua kênh **riêng tư** (nhắn riêng, hoặc tốt nhất là gọi họ đến tận nơi cho quét trực tiếp trên màn hình của bạn). **Tuyệt đối không đăng vào nhóm chat chung** — cả nhóm sẽ quét được và ai cũng sinh được mã của người đó.

- **"Xóa thiết bị"** — gỡ bỏ bảo mật 2 lớp của người đó.
  > **⚠️ Đặc biệt lưu ý:** thao tác này **không cần nhập mã xác thực** để thực hiện. Nghĩa là ai có quyền quản trị đều gỡ được lớp bảo vệ của người khác chỉ bằng một cú bấm. Vì vậy, hãy **rất cẩn trọng khi trao quyền quản trị** — chỉ trao cho người bạn thật sự tin tưởng.

- **"Mở khóa"** — dùng khi một người bị **khóa vì nhập sai mã quá nhiều lần**. Bấm nút này để họ thử lại được ngay, không cần chờ hết thời gian phạt.

> **Mỗi người chỉ dùng được MỘT thiết bị.** Bạn không thể cấp cho một người dùng cả điện thoại lẫn máy tính bảng. Cấp mã mới là mã cũ tự hủy.

### Cấu hình

> **Đường dẫn:** Menu bên trái > **Bảo mật 2 lớp** > **Cấu hình**

Trang này chỉnh 4 thông số kỹ thuật. **Giá trị mặc định đã hợp lý cho hầu hết trường hợp — bạn nên để yên, chỉ sửa khi thật sự cần.**

- **Issuer** (Tên đơn vị phát hành) — tên hiển thị trong ứng dụng xác thực trên điện thoại. Đặt tên công ty bạn để nhân viên dễ nhận ra, nhất là khi họ dùng ứng dụng cho nhiều nơi khác nhau.
  > **Lưu ý:** đổi tên này **chỉ ảnh hưởng đến các mã QR cấp mới về sau**. Những người đã quét mã trước đó vẫn thấy tên cũ trên điện thoại của họ — đây là bình thường, không cần sửa gì.

- **Window** (Độ co giãn thời gian) — cho phép chấp nhận mã lệch bao nhiêu so với đồng hồ máy chủ. Chọn 1 (±30 giây), 2 (±60 giây), hoặc 3 (±90 giây).
  > **Khi nào cần tăng?** Nếu nhân viên **liên tục than mã đúng mà báo sai**, nguyên nhân thường là đồng hồ điện thoại của họ bị lệch. Tăng thông số này lên 2 hoặc 3 sẽ dễ thở hơn. Nhưng **cách đúng đắn hơn** là bảo họ chỉnh điện thoại về **tự động cập nhật giờ theo mạng**.

- **Max attempts** (Số lần sai tối đa) — nhập sai bao nhiêu lần thì bị khóa. Chọn từ 1 đến 20.
  > Để quá thấp (như 1-2) sẽ khiến nhân viên gõ nhầm một cái là bị khóa, rất phiền. Để quá cao thì kẻ gian có nhiều cơ hội dò. Khoảng 5 là hợp lý.

- **Lockout seconds** (Thời gian khóa) — bị khóa bao lâu thì tự mở, tính bằng giây. Từ 60 giây đến 86400 giây (24 giờ).

> **Lưu ý:** Hệ thống **không có nút "bắt buộc tất cả admin dùng 2FA"**. Việc yêu cầu mã được áp dụng theo **từng thao tác quan trọng** (như hoàn tiền, thanh toán lại) và theo phân quyền, chứ không phải bật một công tắc chung.

## Lưu ý & xử lý sự cố

**Nhập mã đúng mà cứ báo sai — lỗi phổ biến nhất.**
Gần như luôn là do **đồng hồ điện thoại bị lệch giờ**. Ứng dụng tính mã dựa vào thời gian, lệch vài chục giây là ra mã khác hoàn toàn. Cách sửa:
- **Android:** vào **Cài đặt > Hệ thống > Ngày và giờ** → bật **"Ngày và giờ tự động"**.
- **iPhone:** vào **Cài đặt > Cài đặt chung > Ngày & Giờ** → bật **"Đặt tự động"**.
Sau đó thử lại. Nếu vẫn không được, hãy báo quản trị viên tăng thông số **Window** lên.

**Gõ mã xong thì báo hết hạn.** Bạn gõ quá chậm, mã đã đổi giữa chừng. Hãy nhìn vòng tròn đếm ngược — **nếu sắp hết, chờ mã mới rồi hãy gõ**, đừng cố dùng mã sắp chết.

**Bị khóa vì nhập sai nhiều lần.** Hai lựa chọn: **chờ hết thời gian khóa** rồi thử lại, hoặc nhờ **quản trị viên bấm "Mở khóa"** cho bạn ngay.

**Đổi điện thoại mới.**
- **Nếu bạn đã chụp ảnh mã QR như đã dặn:** chỉ cần mở ảnh ra, cài Google Authenticator trên máy mới rồi quét lại. Xong trong 1 phút.
- **Nếu không có:** phải nhờ quản trị viên **cấp lại QR mới**. Không có cách nào khác.

> **Mẹo trước khi đổi/bán điện thoại cũ:** hãy **thiết lập xong trên máy mới trước**, kiểm tra chạy được rồi mới xóa dữ liệu máy cũ. Đừng xóa sạch máy cũ rồi mới nhớ ra chuyện này.

**Mất điện thoại, không có ảnh QR.** Liên hệ **ngay** quản trị viên cấp cao để cấp lại QR. Nếu bạn là quản trị viên cấp cao duy nhất, hãy liên hệ **đơn vị triển khai kỹ thuật**. Đây chính là tình huống mà phần cảnh báo đầu bài muốn bạn tránh.

**Vào "2FA của tôi" nhưng trang trống trơn.** Chưa ai cấp QR cho bạn. Hãy liên hệ quản trị viên — không phải lỗi hệ thống.

**Không thấy menu "Bảo mật 2 lớp".** Tài khoản của bạn chưa có quyền liên quan nào. Liên hệ quản trị viên.

## Xem thêm

- [Hướng dẫn đăng nhập tài khoản](../huong-dan-dang-nhap-tai-khoan.md) — nếu bạn bị hỏi mã 6 số khi đăng nhập
- [4.11. Công cụ](cong-cu.md) — nhật ký hệ thống, nơi ghi lại các hoạt động
- [4.9. Cài đặt](cai-dat.md) — cấu hình chung của hệ thống
