# 4.11. Công cụ

**Công cụ** là hộp đồ nghề của người quản trị. Trong đây có 3 thứ không liên quan trực tiếp đến việc bán hàng, nhưng rất cần khi bạn muốn website nói được nhiều thứ tiếng, hoặc khi cần tìm hiểu **"ai đã làm gì, lúc nào"**.

Người dùng hằng ngày gần như không cần vào đây. Bạn chỉ mở mục này khi: muốn thêm/sửa ngôn ngữ cho website, muốn đổi một dòng chữ đang hiện tiếng Anh sang tiếng Việt, hoặc khi cần điều tra một sự cố.

> **Đường dẫn:** Menu bên trái > **Công cụ**

![](../.gitbook/assets/pg149-0.png)

## Trong mục này có gì?

Nhấn vào **Công cụ** ở menu bên trái, bạn sẽ thấy 3 mục con:

- **Ngôn ngữ** — khai báo website của bạn hỗ trợ những thứ tiếng nào (Tiếng Việt, English, 中文…).
- **Quản lý dịch thuật** — dịch từng dòng chữ trên website sang các thứ tiếng đó.
- **Nhật ký hệ thống** — sổ ghi chép lại các lỗi kỹ thuật đã xảy ra.

> **Không thấy mục "Công cụ" trong menu?** Mỗi mục con ở trên cần một quyền riêng. Nếu tài khoản của bạn **không có quyền nào trong cả 3 mục**, thì **toàn bộ menu "Công cụ" sẽ biến mất** khỏi thanh bên trái — không phải website bị lỗi. Hãy liên hệ quản trị viên để được cấp quyền.
>
> Tương tự, nếu bạn chỉ có quyền với 1 mục, bạn sẽ thấy menu "Công cụ" nhưng bên trong chỉ có đúng 1 mục con đó.

## Hiểu đúng: "Ngôn ngữ" và "Quản lý dịch thuật" khác nhau thế nào?

Hai mục này luôn đi cùng nhau và rất dễ lẫn. Hãy hình dung như việc **xuất bản một cuốn sách sang tiếng nước ngoài**:

- **Ngôn ngữ** = **quyết định sẽ dịch sang tiếng gì**. Bạn tuyên bố: "Cuốn sách này sẽ có bản tiếng Anh." Chỉ là khai báo, chưa dịch chữ nào.
- **Quản lý dịch thuật** = **ngồi dịch từng câu**. Đây mới là nơi làm việc thật.

Thứ tự bắt buộc: **khai báo ngôn ngữ trước, dịch sau.** Chưa khai báo tiếng Anh thì không có chỗ để dịch sang tiếng Anh.

## Ngôn ngữ

Đây là nơi bạn khai báo website hỗ trợ những thứ tiếng nào. Website chỉ bán cho khách Việt thì bạn gần như không cần đụng tới mục này.

> **Đường dẫn:** Menu bên trái > **Công cụ** > **Ngôn ngữ**

### Danh sách ngôn ngữ hiện có

Khi vào trang, bạn thấy bảng liệt kê các ngôn ngữ đã khai báo, với các cột:

- **Name** (Tên) — tên ngôn ngữ hiển thị cho khách chọn, ví dụ `Tiếng Việt`, `English`.
- **Locale** (Mã ngôn ngữ) — mã kỹ thuật ngắn của ngôn ngữ, ví dụ `vi`, `en`, `zh`. Máy dùng mã này để phân biệt.
- **Status** (Trạng thái) — đang bật (Publish) hay đang nháp (Draft).
- **Date** (Ngày) — ngày tạo.

Bạn có thể **tìm kiếm** theo tên hoặc mã khi danh sách dài.

### Thêm một ngôn ngữ mới

Điền form thêm ngôn ngữ với 3 thông tin:

- **Name** (Tên) — tên hiển thị. Ví dụ: `English`.
  > **Mẹo:** Nên viết tên bằng chính ngôn ngữ đó (`English` chứ không phải `Tiếng Anh`, `中文` chứ không phải `Tiếng Trung`). Khách Trung Quốc vào website không đọc được chữ "Tiếng Trung", nhưng nhìn `中文` là hiểu ngay.

- **Flag** (Cờ) — chọn lá cờ quốc gia hiển thị kèm tên, giúp khách nhận ra nhanh.

- **Locale** (Mã ngôn ngữ) — **quan trọng nhất, và không được trùng**. Mỗi ngôn ngữ một mã duy nhất.
  > **Cẩn thận:** Đây là mã kỹ thuật theo chuẩn quốc tế, **không phải bạn tự nghĩ ra**. Tiếng Anh là `en`, tiếng Việt là `vi`, tiếng Trung là `zh`, tiếng Hàn là `ko`, tiếng Nhật là `ja`. Nếu bạn tự đặt `tienganh` thì hệ thống vẫn cho lưu nhưng sẽ không hoạt động đúng. Không chắc mã nào, hãy hỏi đơn vị triển khai.

Sau khi thêm, bạn cần chuyển ngôn ngữ sang trạng thái **Publish** thì khách mới chọn được trên website.

### Làm hàng loạt

Tích vào ô vuông đầu mỗi dòng để chọn nhiều ngôn ngữ, rồi chọn hành động: **Publish** (bật), **chuyển sang Draft** (tạm ẩn), hoặc **Delete** (xóa). **Nhớ bấm nút áp dụng** — chọn xong mà quên bấm áp dụng là không có gì xảy ra, đây là lỗi cực kỳ phổ biến.

> **Nên tạm ẩn thay vì xóa.** Nếu bạn muốn dừng bán cho khách Trung Quốc một thời gian, hãy chuyển ngôn ngữ đó sang **Draft**. Toàn bộ công sức dịch thuật vẫn được giữ nguyên, khi cần bật lại là dùng ngay. Xóa hẳn thì rủi ro hơn nhiều.

## Quản lý dịch thuật

Đây là nơi bạn **dịch từng dòng chữ trên website** sang các ngôn ngữ đã khai báo.

> **Đường dẫn:** Menu bên trái > **Công cụ** > **Quản lý dịch thuật**

**Khi nào cần dùng?**
- Website có khách nước ngoài, bạn cần bản tiếng Anh.
- Hoặc: **có một vài dòng trên website đang hiện tiếng Anh mà bạn muốn đổi thành tiếng Việt**. Đây là lý do phổ biến nhất khiến người Việt vào mục này. Ví dụ chữ **"Custom Fields"** trong menu — bạn có thể dịch nó tại đây.

### Màn hình chính

Bạn thấy bảng liệt kê tất cả các ngôn ngữ với các cột:

- **Name** — tên ngôn ngữ.
- **Percent** — **phần trăm đã dịch xong**. Đây là con số bạn nên nhìn đầu tiên: 100% là đã dịch hết, 40% nghĩa là còn 60% số dòng đang hiện tiếng gốc.
- **Translated** — số dòng đã dịch.
- **Last build at** — **lần cuối bạn bấm "Build"**. Xem giải thích ở dưới, đây là cột quan trọng.
- **Actions** — các nút thao tác.

### Quy trình dịch — 3 bước, làm đúng thứ tự

Đây là phần quan trọng nhất của cả trang. Rất nhiều người dịch xong rồi thắc mắc *"sao website vẫn y như cũ?"* — vì họ bỏ qua bước 3.

#### Bước 1: Nạp danh sách chữ cần dịch

Ở đầu trang có nút **"Find Translations"** (Tìm các chuỗi cần dịch). Bấm nút này, hệ thống sẽ **quét website và gom về danh sách tất cả các dòng chữ** có thể dịch được.

Bạn chỉ cần làm bước này **lần đầu tiên**, hoặc sau khi website được nâng cấp có thêm tính năng mới (kéo theo chữ mới chưa có trong danh sách).

#### Bước 2: Dịch từng dòng

Trong hàng của ngôn ngữ bạn muốn dịch, bấm nút **"Translate"**. Một màn hình mới mở ra, hiển thị **30 dòng mỗi trang**, mỗi dòng gồm:

- **Bên trái:** dòng chữ gốc.
- **Bên phải:** ô trống để bạn gõ bản dịch.

Bạn gõ bản dịch vào ô bên phải cho từng dòng.

**Công cụ giúp bạn tìm nhanh:**
- **Bộ lọc:** chọn **"not_translated"** để chỉ hiện các dòng **chưa dịch** — cực kỳ hữu ích, bạn không phải cuộn qua những dòng đã xong. Chọn **"translated"** để xem lại các dòng đã dịch.
- **Ô tìm kiếm:** gõ chữ cần tìm. Bạn có thể chọn tìm theo **chữ gốc** hoặc theo **bản dịch**.

> **Mẹo cho việc "sửa một dòng đang hiện tiếng Anh":** Bạn thấy chữ **"Add New Group"** trên giao diện và muốn nó thành tiếng Việt? Vào đây, dùng ô tìm kiếm gõ đúng `Add New Group`, tìm thấy dòng đó, gõ `Thêm nhóm mới` vào ô bên phải. Xong bước 2.

> **Cẩn thận với các dấu đặc biệt trong câu gốc.** Một số dòng có ký tự lạ như `:count`, `:name`, hoặc `%s`. **Đây là chỗ hệ thống sẽ điền số/tên vào**, ví dụ `Báo cáo :count` sẽ hiện ra thành `Báo cáo 5`. Khi dịch, bạn phải **giữ nguyên các ký tự đó** trong bản dịch, chỉ dịch phần chữ xung quanh. Xóa mất chúng thì con số sẽ không hiện ra nữa.

#### Bước 3: Bấm "Build" — BẮT BUỘC

Dịch xong, quay lại trang danh sách, tìm đúng hàng của ngôn ngữ đó và bấm nút **"Build"**.

> **Đây là bước bị bỏ quên nhiều nhất.** Nếu bạn chỉ dịch mà không Build, **bản dịch chỉ nằm trong kho, chưa được đưa ra website**. Bạn sẽ dịch cả buổi rồi ra ngoài xem và thấy không có gì thay đổi.
>
> **Hình dung:** Bước 2 là bạn viết bản thảo. Bước 3 (**Build**) là mang bản thảo đi in ra và dán lên website. Không in thì chẳng ai đọc được.

Sau khi Build xong, cột **"Last build at"** sẽ cập nhật thời gian mới. **Hãy nhìn cột này để tự kiểm tra**: nếu thời gian ở đó cũ hơn lúc bạn vừa dịch, nghĩa là bạn chưa Build.

Cuối cùng, ra ngoài website nhấn **Ctrl + F5** để tải lại trang cho sạch, rồi kiểm tra.

### Các nút khác

Trong menu **"More"** (Thêm) còn có:

- **"Load translate JSON"** — nhập bản dịch từ một tệp có sẵn. Dùng khi bạn nhận được tệp dịch từ đơn vị triển khai hoặc từ website khác, thay vì gõ tay lại từ đầu.

> **Các nút kỹ thuật khác trong trang này không dành cho người dùng thường.** Nếu bạn không chắc một nút làm gì, **đừng bấm thử** — hãy hỏi đơn vị triển khai. Riêng nút **"Translate"** và **"Build"** thì bấm thoải mái, hai nút này an toàn.

## Nhật ký hệ thống

Đây là **sổ ghi chép tự động** của website. Mỗi khi có trục trặc kỹ thuật, hệ thống ghi lại vào đây: lỗi gì, xảy ra lúc nào, ở đâu.

> **Đường dẫn:** Menu bên trái > **Công cụ** > **Nhật ký hệ thống**

**Bạn có cần hiểu nội dung trong đây không? KHÔNG.** Nội dung ở đây là các dòng chữ kỹ thuật dày đặc, viết cho lập trình viên đọc. Bạn nhìn vào sẽ thấy rối mắt — **điều đó hoàn toàn bình thường**, không phải do bạn kém.

**Vậy mục này để làm gì với bạn?** Để bạn **giúp bộ phận kỹ thuật sửa lỗi nhanh hơn**. Khi website gặp sự cố:

1. Bạn vào đây.
2. Tìm dòng có **thời gian gần nhất với lúc lỗi xảy ra**.
3. **Chụp màn hình** dòng đó (chụp đầy đủ, đừng cắt bớt).
4. Gửi cho đơn vị hỗ trợ, kèm mô tả bạn đã làm gì trước khi lỗi xảy ra.

Với 3 thông tin đó, người kỹ thuật thường tìm ra nguyên nhân trong vài phút, thay vì phải hỏi đi hỏi lại bạn cả buổi.

> **Cẩn thận:** Trong nhật ký có thể chứa thông tin nhạy cảm. **Đừng đăng nội dung nhật ký lên các hội nhóm công khai trên Facebook để hỏi.** Chỉ gửi riêng cho đơn vị hỗ trợ chính thức của bạn.

> **Thấy nhiều dòng lỗi có đáng lo không?** Không nhất thiết. Website nào cũng ghi lại vô số cảnh báo vặt mà không ảnh hưởng gì đến việc bán hàng. **Chỉ quan tâm khi bạn thật sự đang gặp sự cố nhìn thấy được** — như khách không đặt được tour, trang trắng, không gửi được email. Đừng vào đây "dạo chơi" rồi tự làm mình lo lắng.

## Lưu ý & xử lý sự cố

**Dịch xong nhưng website vẫn hiện chữ cũ.** Theo thứ tự:
1. **Bạn đã bấm "Build" chưa?** — 90% trường hợp là do quên bước này. Kiểm tra cột "Last build at".
2. Đã nhấn **Ctrl + F5** ngoài website chưa? Trình duyệt hay giữ bản cũ.
3. Chờ khoảng 1 phút rồi thử lại.

**Bấm "Build" thì báo lỗi.** Đây là lỗi kỹ thuật về quyền ghi tệp trên máy chủ, **bạn không tự sửa được**. Hãy chụp màn hình dòng báo lỗi và liên hệ đơn vị triển khai.

**Thêm ngôn ngữ mới nhưng khách không thấy trên website.** Kiểm tra: ngôn ngữ đó đang ở trạng thái **Publish** hay **Draft**? Draft thì khách không thấy.

**Tìm mãi không thấy dòng chữ cần dịch.** Ba khả năng:
1. Bạn chưa bấm **"Find Translations"** để nạp danh sách.
2. Bạn gõ tìm kiếm không khớp chính xác — hãy thử gõ **ít chữ hơn**, ví dụ chỉ gõ `Custom` thay vì cả cụm `Custom Fields`.
3. Dòng chữ đó không nằm trong hệ thống dịch (ví dụ nó là nội dung bạn tự nhập cho tour, không phải nhãn giao diện) — trường hợp này bạn sửa trực tiếp ở nơi nhập tour, không phải ở đây.

**Không thấy menu "Công cụ" đâu cả.** Bạn không có quyền với cả 3 mục con. Liên hệ quản trị viên.

## Xem thêm

- [4.8. Custom Fields](custom-fields.md) — mục đang hiển thị tiếng Anh, bạn có thể dịch nó tại "Quản lý dịch thuật"
- [4.9. Cài đặt](cai-dat.md) — cấu hình chung của website
- [4.12. Bảo mật 2 lớp](bao-mat-2-lop.md) — bảo vệ tài khoản quản trị
