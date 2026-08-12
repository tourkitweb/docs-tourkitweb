# 4.10. Tích hợp

**Tích hợp** là nơi bạn nối website của mình với **các dịch vụ của công ty khác**. Website không sống một mình: bạn có thể muốn đơn hàng tự chảy về phần mềm CRM, muốn nhận thông báo qua Telegram mỗi khi có khách đặt tour, muốn phần mềm quản lý khách sạn tự đẩy giá phòng sang website.

Mỗi kết nối như vậy gọi là một **tích hợp**. Tất cả nằm gọn trong mục này.

> **Đường dẫn:** Menu bên trái > **Tích hợp**

> **Không thấy mục "Tích hợp" trong menu?** Mục này cần quyền quản trị. Nếu tài khoản của bạn chưa được cấp quyền, mục này sẽ ẩn hoàn toàn. Hãy liên hệ quản trị viên của đơn vị bạn.

## "Tích hợp" khác gì "Cài đặt"?

Đây là chỗ nhầm lẫn phổ biến nhất, vì hai mục nằm sát nhau trong menu và trông giống hệt nhau. Cách phân biệt:

|                      | **Cài đặt**                                 | **Tích hợp**                                             |
| -------------------- | ------------------------------------------- | -------------------------------------------------------- |
| Nói về               | **Bên trong** website của bạn               | **Kết nối ra ngoài** với công ty khác                    |
| Ví dụ                | Tên công ty, logo, tiền tệ, cổng thanh toán | CRM, Telegram, PMS khách sạn, Accesstrade                |
| Bạn cần chuẩn bị gì? | Chỉ cần thông tin của chính bạn             | **Mã khóa (API Key) do bên kia cấp**                     |
| Bỏ qua thì sao?      | Website hiển thị thiếu/sai thông tin        | Website vẫn chạy bình thường, chỉ là không có kết nối đó |

**Mẹo tự phân biệt trong 3 giây:** _"Việc này có cần một công ty KHÁC cấp mã cho tôi không?"_

* **Không** → nằm ở [Cài đặt](cai-dat.md).
* **Có** → nằm ở **Tích hợp** (trang này).

> **Điều cần biết trước:** Mọi tích hợp đều là **tùy chọn**. Bạn không bắt buộc phải bật cái nào. Website vẫn bán hàng bình thường mà không cần một tích hợp nào cả. Chỉ bật khi bạn thật sự đang dùng dịch vụ đó.

## Trong mục này có gì?

Khi nhấn vào **Tích hợp**, danh sách các kết nối sẽ xổ ra ở cột bên trái. Mỗi kết nối có một bài hướng dẫn riêng:

| Kết nối | Dùng để làm gì |
| --- | --- |
| [Tourkit CRM](tich-hop/tourkit-crm.md) | Đẩy đơn hàng sang CRM, và kéo tour từ CRM về website |
| [PMS Gohost — Khách sạn](tich-hop/pms-gohost.md) | Nối phần mềm quản lý khách sạn để đồng bộ phòng và giá |
| [Thanh toán Tingee](tich-hop/thanh-toan-tingee.md) | Tự động ghi nhận khi tiền về tài khoản |
| [Thông báo Telegram / Discord](tich-hop/thong-bao-telegram-discord.md) | Nhận tin nhắn báo có khách đặt tour |
| [Affiliate với đối tác](tich-hop/affiliate-accesstrade.md) | Ghi nhận đơn hàng do đối tác giới thiệu (Accesstrade) |

> **Lưu ý:** Danh sách trên website của bạn có thể **ít hơn** bảng này. Mỗi tích hợp chỉ hiện ra khi tính năng tương ứng đã được bật cho website của bạn. Nếu bạn cần một kết nối mà không thấy trong menu, hãy liên hệ đơn vị triển khai.

## Cách làm việc chung với mọi tích hợp

Dù là kết nối nào, quy trình cũng chỉ có 4 bước giống nhau:

1. **Xin mã từ bên đối tác.** Đây là việc bên ngoài website — bạn liên hệ nhà cung cấp dịch vụ để họ cấp cho bạn API Key / Access Key / Token.
2. **Bật công tắc** — tích vào ô **"Enable"** hoặc ô "Bật…" ở đầu trang.
3. **Dán mã vào các ô tương ứng.**
4. **Nhấn nút \[Lưu cài đặt]** màu xanh lá ở **góc trên cùng bên phải**.

> **Cẩn thận với các mã khóa (API Key):** Chúng giống như **chìa khóa nhà**. Ai có mã đó có thể truy cập dữ liệu của bạn. Vì vậy:
>
> * **Không** đăng mã lên nhóm chat công khai, Facebook, hay diễn đàn.
> * **Không** chụp màn hình có chứa mã rồi gửi lung tung.
> * Nếu lỡ lộ, hãy liên hệ nhà cung cấp để họ **cấp mã mới** và hủy mã cũ.

> **Lỗi số 1 khi dán mã:** dính **dấu cách thừa** ở đầu hoặc cuối khi copy từ email/Zalo. Mắt thường không thấy, nhưng hệ thống báo sai mã. Mẹo: dán xong, bấm vào cuối ô, nhấn phím **End** rồi **Backspace** vài lần cho chắc.

## Lưu ý & xử lý sự cố chung

**Bật xong nhưng "không thấy gì xảy ra".** Với hầu hết tích hợp, đây là thứ tự kiểm tra:

1. Ô **Enable / Bật…** còn tích không?
2. Đã bấm **\[Lưu cài đặt]** chưa, có thấy thông báo thành công không?
3. Các mã có dính **khoảng trắng thừa** không?
4. Với Telegram/Discord: đã tích **thời điểm nhận thông báo** chưa?
5. Với Tingee/Accesstrade: đã khai báo **phía bên kia** chưa? (kết nối 2 chiều)

**Báo lỗi xác thực / sai key.** Gần như luôn là do mã dán sai, thiếu ký tự, hoặc mã đã bị bên kia hủy. Hãy xin lại mã mới từ nhà cung cấp.

**Trước khi gọi hỗ trợ, hãy chuẩn bị:** tên tích hợp đang gặp vấn đề, **ảnh chụp màn hình dòng báo lỗi** (đầy đủ, đừng cắt), và mô tả bạn đã làm gì trước khi lỗi xảy ra. Có 3 thứ này, việc xử lý sẽ nhanh hơn rất nhiều.

> **Nguyên tắc an toàn nhất khi làm tích hợp:** làm **từng cái một**. Bật một tích hợp → kiểm tra chạy tốt → mới sang cái tiếp theo. Bật cả 5 cái cùng lúc rồi có lỗi, bạn sẽ không biết cái nào gây ra.

## Xem thêm

* [4.9. Cài đặt](cai-dat.md) — cấu hình bên trong website (tiền tệ, cổng thanh toán)
* [4.13. Báo cáo](bao-cao.md) — xem đơn hàng và doanh thu
* [4.11. Công cụ](cong-cu.md) — nhật ký hệ thống, nơi xem lại lỗi đã xảy ra
