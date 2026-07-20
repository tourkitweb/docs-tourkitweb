# 4.4. Kết nối khách sạn

**Kết nối khách sạn** giúp website của bạn **tự động lấy dữ liệu phòng khách sạn từ một đối tác bên ngoài** về, thay vì bạn phải ngồi nhập tay từng khách sạn, từng loại phòng, từng mức giá.

Hình dung cho dễ: bình thường muốn bán 100 khách sạn, bạn phải tự tạo 100 khách sạn trong hệ thống, tự cập nhật giá mỗi ngày, tự kiểm tra còn phòng hay hết phòng. Với người làm một mình thì đó là công việc không tưởng.

Kết nối khách sạn giải quyết đúng chuyện đó: bạn ký hợp đồng với một đơn vị có sẵn kho phòng, họ đưa bạn một "chìa khóa kỹ thuật", bạn khai báo chìa khóa đó vào đây. Từ đó:

* Danh sách khách sạn **tự chảy về** website của bạn.
* **Giá và tình trạng còn phòng tự cập nhật**, không cần bạn động tay.
* Khách đặt phòng trên web của bạn, đơn hàng **tự chuyển sang** cho đối tác xử lý.

> **Đường dẫn:** Menu bên trái > mục **Kết nối khách sạn**

> **Lưu ý:** Tính năng này có thể chưa được bật trên website của bạn. Nếu không thấy mục này trong menu, hãy liên hệ đơn vị triển khai.

> 📷 _\[Cần chụp màn hình: trang chính của mục Kết nối khách sạn]_

## Ai cần đọc bài này?

Nói thẳng để bạn không mất thời gian:

**Bạn KHÔNG cần mục này nếu:** bạn tự nhập khách sạn của mình vào hệ thống, hoặc có đối tác tự đăng phòng lên (mô hình Vendor). Hãy đọc [4.3. Quản lý Vendor](quan-ly-vendor.md) thay vì bài này.

**Bạn CẦN mục này nếu:** bạn đã ký hợp đồng với một đơn vị cung cấp kho phòng và họ đã đưa bạn thông tin kết nối.

> **Đây là phần kỹ thuật nhất trong toàn bộ khối Hệ thống.** Việc thiết lập ban đầu **thường do đơn vị triển khai làm giúp bạn một lần duy nhất**. Sau đó bạn chỉ vào để theo dõi và điều chỉnh giá. Bài này viết để bạn **hiểu chuyện gì đang diễn ra**, chứ không phải để bạn tự cài từ đầu. Nếu chưa từng làm bao giờ, hãy nhờ đơn vị triển khai — sai ở đây có thể khiến giá phòng trên web hiển thị sai và bạn bán lỗ mà không biết.

## Trong mục này có gì?

Bên trong thường gồm các phần sau:

* **Cài đặt API** — nơi khai báo "chìa khóa" để nối với đối tác. Làm một lần lúc đầu.
* **Cấu hình giá** — quyết định giá bán ra trên web của bạn so với giá đối tác đưa về. **Đây là phần bạn cần quan tâm nhất.**
* **Nhật ký API** — sổ ghi lại mọi lần hệ thống nói chuyện với đối tác. Dùng khi cần tìm nguyên nhân lỗi.
* **Hướng dẫn** — tài liệu kỹ thuật đi kèm.

## Cài đặt API — "chìa khóa" để nối

**API** nghe rất kỹ thuật, nhưng hiểu đơn giản là: **cách để hai website tự nói chuyện với nhau mà không cần con người ngồi giữa.**

Ví von: bạn muốn nhân viên lấy hàng trong kho của đối tác, đối tác đưa bạn một **chìa khóa kho**. Thông tin trong phần Cài đặt API chính là cái chìa khóa đó — chỉ có điều nó ở dạng một chuỗi ký tự dài loằng ngoằng.

**Bạn không tự nghĩ ra chuỗi này được.** Nó do **đối tác cung cấp cho bạn** sau khi ký hợp đồng. Việc của bạn chỉ là dán nó vào đúng ô.

> 📷 _\[Cần chụp màn hình: trang Cài đặt API trong mục Kết nối khách sạn]_

**Sau khi dán xong, hãy dùng nút kiểm tra kết nối.** Đây là bước quan trọng: nó thử gọi sang đối tác một lần để xem chìa khóa có mở được cửa không.

* **Báo thành công** → chìa khóa đúng, đi tiếp.
* **Báo lỗi** → đừng làm gì thêm nữa, mọi bước sau đều vô ích. Xem phần xử lý sự cố ở cuối bài.

> **Cẩn thận — bảo mật:** Chuỗi ký tự này giống như **mật khẩu tài khoản ngân hàng của bạn với đối tác**. Ai cầm được nó có thể thao tác thay bạn. Tuyệt đối:
>
> * Không chụp màn hình gửi qua Zalo/Facebook.
> * Không dán vào file Excel dùng chung.
> * Không đưa cho người không có trách nhiệm.
>
> Nếu lỡ để lộ, hãy báo đối tác ngay để họ cấp chìa khóa mới.

## Cấu hình giá — phần quan trọng nhất với túi tiền của bạn

Đây là phần bạn **thực sự cần hiểu**, vì nó quyết định bạn lãi hay lỗ.

Vấn đề: đối tác đưa về **giá gốc** của phòng. Nhưng bạn không thể bán đúng giá gốc — bán vậy thì bạn không được đồng nào, còn phải chịu phí cổng thanh toán. Bạn cần cộng thêm phần của mình.

**Cấu hình giá** chính là nơi bạn đặt ra quy tắc đó: _"Giá đối tác đưa về bao nhiêu thì tôi bán ra bấy nhiêu."_

Điểm mạnh: bạn đặt quy tắc **một lần**, nó áp dụng cho **toàn bộ** khách sạn tự động, kể cả những khách sạn mới chảy về sau này. Đối tác đổi giá thì giá bán của bạn cũng tự đổi theo đúng tỷ lệ — bạn không phải sửa tay ngày nào.

> 📷 _\[Cần chụp màn hình: trang Cấu hình giá trong mục Kết nối khách sạn]_

> **Cẩn thận nghiêm túc:** Đây là chỗ nguy hiểm nhất của cả mục. Đặt sai một con số, **toàn bộ hàng trăm khách sạn của bạn bán sai giá cùng lúc** — và tệ hơn là **hệ thống không báo lỗi gì cả**, vì với máy tính thì con số nào cũng hợp lệ. Bạn chỉ phát hiện ra khi đã bán lỗ vài chục đơn.
>
> **Cách làm an toàn:**
>
> 1. Đặt quy tắc xong, **lưu lại**.
> 2. **Mở website ra như một khách hàng thật**, tìm đúng khách sạn đó, xem giá hiện lên là bao nhiêu.
> 3. **Lấy máy tính bấm tay** xem có đúng như bạn dự tính không.
> 4. Đúng rồi mới yên tâm. Sai thì vào sửa ngay.
>
> Bước này mất 5 phút và tiết kiệm cho bạn rất nhiều tiền.

> **Mẹo:** Đừng quên cộng cả **phí cổng thanh toán** và các chi phí ngầm vào phần chênh lệch của bạn. Nhiều người chỉ tính hoa hồng mong muốn rồi phát hiện thực thu ít hơn dự tính.

## Nhật ký API — sổ ghi để tìm lỗi

**Nhật ký** ghi lại mọi lần website của bạn nói chuyện với đối tác: lúc mấy giờ, hỏi cái gì, đối tác trả lời gì, thành công hay lỗi.

Bạn **không cần vào đây khi mọi thứ chạy êm**. Nó chỉ hữu ích khi có sự cố: khách báo đặt phòng không được, hoặc giá hiển thị sai.

Nội dung trong này khá kỹ thuật, đầy chữ tiếng Anh và mã số. **Bạn không cần hiểu nó.** Việc của bạn chỉ là: khi báo lỗi cho đơn vị triển khai, hãy **chụp màn hình phần nhật ký tại thời điểm xảy ra lỗi** gửi kèm. Với người kỹ thuật, ảnh đó nói lên nhiều hơn cả trang mô tả — nó giúp họ tìm ra nguyên nhân nhanh gấp nhiều lần.

## Khách sạn tự chảy về nằm ở đâu?

Sau khi kết nối chạy, các khách sạn từ đối tác sẽ xuất hiện trong module **Khách sạn** bình thường, nằm chung với các khách sạn bạn tự nhập.

> **Cẩn thận:** Với những khách sạn được kéo về từ đối tác, hãy **hạn chế sửa tay** thông tin và giá. Lý do: mỗi lần hệ thống đồng bộ lại với đối tác, dữ liệu mới có thể **ghi đè lên phần bạn vừa sửa**, và công sức của bạn biến mất. Muốn thay đổi giá bán, hãy chỉnh ở **Cấu hình giá** — đó là cách đúng và bền vững.

## Lưu ý & xử lý sự cố

**Kiểm tra kết nối báo lỗi.** Kiểm tra theo thứ tự, đây là các nguyên nhân từ thường gặp nhất:

1. **Dán chuỗi bị dính dấu cách thừa** ở đầu hoặc cuối — lỗi số 1 và rất khó nhìn ra bằng mắt vì dấu cách vô hình. Hãy xóa sạch ô đó và dán lại thật cẩn thận.
2. **Dán thiếu ký tự** — chuỗi rất dài, khi bôi đen copy dễ bị hụt. Hãy copy lại toàn bộ.
3. **Chìa khóa đã hết hạn hoặc bị đối tác thu hồi** — liên hệ đối tác xin chuỗi mới.
4. **Nhầm giữa môi trường thử nghiệm và môi trường thật** — đối tác thường cấp 2 bộ khác nhau. Hỏi lại xem bạn đang dùng bộ nào.

**Kết nối báo thành công nhưng không thấy khách sạn nào về.** Việc kéo dữ liệu về **cần thời gian**, đặc biệt lần đầu với hàng trăm khách sạn — có thể mất từ vài phút tới lâu hơn. Hãy đợi rồi tải lại trang bằng **Ctrl + F5**. Nếu chờ lâu vẫn không thấy gì, liên hệ đơn vị triển khai.

**Giá trên web sai so với dự tính.** Vào **Cấu hình giá** kiểm tra lại quy tắc. Đây gần như luôn là nguyên nhân. Sau khi sửa, nhớ mở web ra kiểm tra lại bằng mắt và bấm máy tính đối chiếu.

**Khách báo đặt phòng thất bại.** Vào **Nhật ký API** xem lần gọi gần nhất có báo lỗi không, chụp màn hình gửi đơn vị triển khai. Đừng tự sửa cài đặt API khi chưa hiểu rõ — bạn có thể làm hỏng cả kết nối đang chạy tốt cho những khách khác.

**Khách sạn hiện trên web nhưng thiếu ảnh.** Ảnh thường được kéo về sau, chậm hơn thông tin chữ. Hãy đợi thêm rồi kiểm tra lại.

## Xem thêm

* [4. Khối HỆ THỐNG](./)
* [4.3. Quản lý Vendor](quan-ly-vendor.md)
