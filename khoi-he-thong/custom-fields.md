# 4.8. Custom Fields

Mỗi doanh nghiệp du lịch có những thông tin riêng mà hệ thống không thể đoán trước được. Ví dụ: bạn muốn mỗi tour đều có ô **"Mã tour nội bộ"**, hoặc mỗi khách sạn đều có ô **"Giờ nhận phòng sớm"**. Những ô này hệ thống không làm sẵn, vì mỗi công ty một kiểu.

**Custom Fields** (tạm dịch: _Trường thông tin tự tạo_) chính là nơi bạn **tự thêm những ô nhập thông tin riêng** đó vào. Sau khi tạo xong, khi bạn vào thêm/sửa một tour hay một khách sạn, những ô bạn vừa tạo sẽ xuất hiện ngay trong form, y như các ô có sẵn.

Nói ngắn gọn: **hệ thống thiếu ô nào, bạn tự thêm ô đó**.

> **Đường dẫn:** Menu bên trái > **Custom Fields**

> **Lưu ý về tên tiếng Anh:** Trên giao diện thật, mục này và các mục con của nó vẫn **hiển thị bằng tiếng Anh** (chưa được dịch). Bạn hãy tìm đúng chữ tiếng Anh trên màn hình nhé:
>
> * **"Custom Fields"** — Trường thông tin tự tạo (mục cha)
> * **"Field Groups"** — Danh sách nhóm trường
> * **"Add New Group"** — Thêm nhóm mới

## Trong mục này có gì?

Khi nhấn vào **Custom Fields** ở menu bên trái, bạn sẽ thấy 2 mục con:

* **"Field Groups"** (Danh sách nhóm trường) — nơi liệt kê tất cả các nhóm ô thông tin bạn đã tạo. Vào đây để xem lại, sửa hoặc xóa.
* **"Add New Group"** (Thêm nhóm mới) — nơi tạo một nhóm ô thông tin mới.

> **Không thấy mục "Custom Fields" trong menu?** Tài khoản của bạn chưa được cấp quyền xem mục này. Hãy liên hệ quản trị viên của đơn vị bạn để được cấp quyền.

## Hiểu đúng 2 khái niệm trước khi làm

Chỉ có 2 khái niệm thôi, bạn nắm được là làm được hết:

**1. Field (Trường) = MỘT Ô nhập thông tin.** Ví dụ: ô "Mã tour nội bộ", ô "Tên hướng dẫn viên", ô "Ghi chú nội bộ".

**2. Field Group (Nhóm trường) = MỘT NHÓM chứa nhiều ô, gắn vào một loại sản phẩm.** Bạn không tạo lẻ từng ô. Bạn tạo một **nhóm**, rồi bỏ các ô vào trong nhóm đó, rồi chỉ định nhóm này áp dụng cho loại sản phẩm nào (Tour? Khách sạn? Xe?).

Hình dung đơn giản: **Nhóm giống như một cái ngăn kéo, các ô là những tờ giấy bạn bỏ vào ngăn kéo đó.** Bạn dán nhãn cái ngăn kéo là "Thông tin nội bộ của Tour", rồi từ đó mọi tour đều có ngăn kéo này.

## Tạo một nhóm trường mới

Ví dụ thực tế xuyên suốt: bạn muốn mỗi **Tour** có thêm 2 ô là **"Mã tour nội bộ"** và **"Tên hướng dẫn viên"**.

### Bước 1: Mở màn hình tạo nhóm

Vào menu bên trái, nhấn **Custom Fields**, rồi chọn **"Add New Group"** (Thêm nhóm mới).

### Bước 2: Đặt tên cho nhóm

Ô **"Title"** (Tiêu đề) — đặt tên gợi nhớ cho nhóm này. Tên này **chỉ bạn và nhân viên nhìn thấy trong trang quản trị**, khách hàng ngoài website không thấy. Cứ đặt tiếng Việt có dấu thoải mái.

Ví dụ: `Thông tin nội bộ của Tour`

### Bước 3: Chọn nhóm này áp dụng cho loại sản phẩm nào

Đây là bước **quan trọng nhất, bắt buộc phải chọn**, nếu bỏ trống hệ thống sẽ không cho lưu.

Bạn chọn một hoặc nhiều loại dịch vụ mà nhóm ô này sẽ xuất hiện. Các lựa chọn có sẵn gồm: **Khách sạn (Hotel), Tour, Không gian (Space), Xe (Car), Sự kiện (Event), Du thuyền (Cruise)**.

Trong ví dụ của chúng ta, bạn chọn **Tour**.

> **Điều này nghĩa là gì?** Sau khi lưu, mỗi lần bạn vào **Tour > Thêm tour mới** hoặc mở sửa một tour cũ, form sẽ có thêm khu vực "Thông tin nội bộ của Tour" với 2 ô bạn sắp tạo. Còn khi bạn vào thêm Khách sạn thì sẽ **không** thấy — vì bạn chỉ chọn Tour.
>
> **Mẹo:** Bạn có thể chọn nhiều loại cùng lúc, ví dụ chọn cả Tour và Du thuyền, thì cả hai đều có nhóm ô này.

### Bước 4: Thêm từng ô vào nhóm

Nhấn nút thêm trường (**"Add Field"**) để tạo ô đầu tiên. Mỗi ô có các thông tin sau — nghe thì nhiều nhưng thực tế bạn **chỉ cần điền 2 cái đầu là chạy được**:

* **"Field Label"** (Nhãn của ô) — **BẮT BUỘC**. Đây là dòng chữ bạn sẽ nhìn thấy phía trên ô nhập khi làm việc. Gõ tiếng Việt có dấu bình thường. Ví dụ: `Mã tour nội bộ`
*   **"Field Name"** (Tên kỹ thuật của ô) — hệ thống **tự điền giúp bạn** ngay khi bạn gõ xong nhãn ở trên. Nó tự bỏ dấu tiếng Việt và nối các chữ bằng gạch dưới, ví dụ `Mã tour nội bộ` sẽ tự thành `ma_tour_noi_bo`.

    > **Cẩn thận:** Đây là tên mà máy dùng để lưu dữ liệu. **Bạn không nên sửa ô này**, và đặc biệt là **không sửa sau khi đã dùng nhóm này để nhập liệu thật** — vì đổi tên kỹ thuật thì dữ liệu cũ sẽ không tìm thấy được nữa, coi như mất. Cứ để hệ thống tự điền.
* **"Field Type"** (Kiểu ô) — chọn ô này là loại gì. Xem bảng ở mục tiếp theo bên dưới để chọn cho đúng.
*   **"Required?"** (Bắt buộc?) — chọn **Yes** nếu bắt buộc phải điền ô này thì mới lưu được sản phẩm. Chọn **No** nếu được phép bỏ trống.

    > **Mẹo:** Đừng vội để **Yes** cho mọi ô. Nếu bạn đã có sẵn 200 tour cũ chưa có thông tin này, thì mỗi lần nhân viên sửa một tour cũ sẽ bị chặn lại bắt điền. Hãy để **No** trước, khi nào dữ liệu đã đầy đủ hãy bật lên.
* **"Instructions"** (Hướng dẫn) — dòng chữ nhỏ hiện bên dưới ô, để nhắc nhân viên nhập cho đúng. Ví dụ: `Mã do phòng điều hành cấp, gồm 6 ký tự`
* **"Placeholder"** (Chữ mờ gợi ý) — chữ xám mờ hiện sẵn bên trong ô khi ô còn trống. Gõ vào là nó biến mất, nó **không phải là dữ liệu**. Ví dụ: `VD: HN0125`
* **"Default Value"** (Giá trị mặc định) — nội dung tự điền sẵn cho mọi sản phẩm mới. Để trống nếu không cần.
* **"Options"** (Các lựa chọn) — ô này **chỉ hiện ra khi** bạn chọn Field Type là **Select / Checkbox / Radio**. Xem cách điền ở mục riêng bên dưới.
* **"Wrapper Class"** (Độ rộng hiển thị) — dành cho người rành kỹ thuật, để chỉnh ô nằm rộng hay hẹp trên form. **Bạn cứ để trống**, hệ thống sẽ tự dàn đẹp. Nếu bạn muốn 2 ô nằm cạnh nhau trên cùng một hàng, người kỹ thuật sẽ điền `col-md-6` cho cả hai.

Điền xong ô thứ nhất, bạn nhấn thêm trường lần nữa để tạo ô **"Tên hướng dẫn viên"**, làm tương tự.

### Bước 5: Đặt trạng thái và lưu

*   **"Status"** (Trạng thái) — chọn **"Publish"** (Xuất bản) để nhóm này hoạt động thật. Nếu chọn **"Draft"** (Bản nháp) thì nhóm chỉ được lưu lại chứ **các ô sẽ không xuất hiện** khi bạn thêm/sửa tour.

    > **Lỗi phổ biến nhất ở mục này:** tạo xong xuôi, vào thêm tour lại chẳng thấy ô nào. Nguyên nhân gần như luôn là **nhóm đang ở trạng thái Draft**. Quay lại "Field Groups", mở nhóm ra và chuyển sang **Publish**.
* **"Order"** (Thứ tự) — nếu bạn có nhiều nhóm cùng gắn vào Tour, số này quyết định nhóm nào hiện lên trước. Số nhỏ hiện trước. Không quan tâm thì để nguyên.
* **"Position"** (Vị trí) — nhóm ô sẽ hiện ở khu vực nào của trang. Cứ để mặc định (`normal`) là ổn.

Cuối cùng nhấn nút **"Lưu"**.

### Bước 6: Kiểm tra lại thành quả

Đừng tin là xong, hãy tự kiểm tra: vào **Menu bên trái > Tour > Thêm tour mới**. Cuộn xuống, bạn phải thấy khu vực **"Thông tin nội bộ của Tour"** với 2 ô vừa tạo. Thấy rồi là thành công.

Từ giờ, mỗi tour bạn nhập vào 2 ô đó, dữ liệu sẽ được lưu riêng cho từng tour.

## Chọn "Field Type" (kiểu ô) nào cho đúng?

Đây là chỗ dễ phân vân nhất. Nguyên tắc: **thông tin bạn định lưu trông như thế nào, thì chọn kiểu như thế đó.**

| Bạn muốn nhập gì?                                     | Chọn kiểu              |
| ----------------------------------------------------- | ---------------------- |
| Một dòng chữ ngắn (mã tour, tên người)                | **Text Input**         |
| Một đoạn văn nhiều dòng, không cần trang trí          | **Textarea**           |
| Một đoạn văn dài có in đậm, gạch đầu dòng, chèn ảnh   | **WYSIWYG Editor**     |
| Một con số (số chỗ, số ngày)                          | **Number**             |
| Địa chỉ email                                         | **Email**              |
| Một đường link website                                | **URL**                |
| Chọn 1 trong nhiều đáp án có sẵn (danh sách xổ xuống) | **Select Dropdown**    |
| Tích được nhiều đáp án cùng lúc                       | **Checkbox**           |
| Chỉ được chọn đúng 1 đáp án (các nút tròn)            | **Radio Button**       |
| Một tấm ảnh                                           | **Image Upload**       |
| Nhiều tấm ảnh (bộ sưu tập)                            | **Gallery**            |
| Một tệp đính kèm (PDF, Word…)                         | **File Upload**        |
| Một ngày (chọn trên lịch)                             | **Date Picker**        |
| Một giờ                                               | **Time Picker**        |
| Cả ngày lẫn giờ                                       | **Date & Time Picker** |
| Một màu sắc                                           | **Color Picker**       |
| Một nhóm ô lặp đi lặp lại nhiều lần                   | **Repeater**           |

> **Về kiểu "Repeater" (Lặp lại):** đây là kiểu nâng cao. Dùng khi một thông tin có thể có nhiều dòng mà bạn không biết trước là bao nhiêu dòng. Ví dụ: bạn muốn liệt kê danh sách hướng dẫn viên của tour, mỗi người gồm _Tên_ và _Số điện thoại_, nhưng tour này có 1 người, tour kia có 3 người. Bạn tạo một ô kiểu Repeater, rồi bên trong nó tạo **Sub Fields** (các ô con) là "Tên" và "Số điện thoại". Khi nhập tour, bạn sẽ có nút thêm dòng để bấm bao nhiêu lần tùy ý.
>
> Nếu bạn thấy rối, cứ bỏ qua Repeater — 16 kiểu còn lại đủ dùng cho hầu hết nhu cầu.

## Cách điền ô "Options" (cho Select, Checkbox, Radio)

Khi bạn chọn kiểu **Select Dropdown**, **Checkbox** hoặc **Radio Button**, một ô lớn tên **"Options"** sẽ hiện ra. Đây là nơi bạn liệt kê các đáp án cho khách/nhân viên chọn.

Quy tắc: **mỗi đáp án viết trên MỘT DÒNG riêng**, theo mẫu:

```
giá_trị : Nhãn hiển thị
```

Trong đó:

* **Phần bên trái dấu hai chấm** là giá trị máy lưu — nên viết **không dấu, không khoảng trắng**.
* **Phần bên phải dấu hai chấm** là dòng chữ người dùng nhìn thấy — viết tiếng Việt có dấu thoải mái.

Ví dụ, ô "Mức độ vận động của tour":

```
nhe : Nhẹ nhàng, phù hợp người lớn tuổi
trung_binh : Vận động vừa phải
nang : Cần thể lực tốt
```

**Những lỗi hay gặp khi điền Options:**

* **Viết tất cả trên một dòng** → hệ thống hiểu thành một đáp án duy nhất. Phải nhấn Enter xuống dòng cho mỗi đáp án.
* **Quên dấu hai chấm** → đáp án hiển thị không như ý.
* **Copy từ Word/Excel dán vào** → hay dính khoảng trắng thừa hoặc ký tự lạ. Tốt nhất là **gõ tay lại**.
* **Sửa phần bên trái (giá trị) sau khi đã dùng** → các sản phẩm cũ đã chọn giá trị đó sẽ bị mất lựa chọn. Muốn đổi chữ hiển thị thì chỉ sửa **phần bên phải**, giữ nguyên phần bên trái.

## Xem, sửa, xóa các nhóm đã tạo

Vào **Custom Fields > "Field Groups"**, bạn sẽ thấy danh sách tất cả các nhóm đã tạo, mỗi trang 20 nhóm.

Tại đây bạn có thể:

* **Tìm kiếm** nhóm theo tên, khi danh sách đã dài.
* **Lọc theo trạng thái** để xem riêng các nhóm đang bật (Publish) hay đang là nháp (Draft).
* **Nhấn vào tên nhóm** để mở ra sửa: thêm ô mới, đổi nhãn, xóa bớt ô.
* **Làm hàng loạt:** tích vào ô vuông đầu mỗi dòng để chọn nhiều nhóm, rồi chọn hành động (xóa / chuyển Publish / chuyển Draft) và **nhớ nhấn nút áp dụng** — rất nhiều người chọn xong rồi quên bấm áp dụng và tưởng hệ thống lỗi.

> **Cẩn thận khi xóa:** Xóa một nhóm đồng nghĩa các ô trong nhóm biến mất khỏi form, và **dữ liệu bạn đã nhập vào các ô đó cũng không còn dùng được**. Nếu chỉ muốn tạm ẩn đi, hãy chuyển sang **Draft** thay vì xóa — cách này an toàn hơn nhiều và bật lại lúc nào cũng được.

## Sao lưu và chuyển nhóm sang website khác (Export / Import)

Ở trang **"Field Groups"** có 2 chức năng hữu ích:

* **Export** (Xuất ra) — tải toàn bộ các nhóm, hoặc chỉ một nhóm, về máy tính dưới dạng một tệp. Dùng để **sao lưu phòng khi lỡ tay xóa mất**, hoặc để mang cấu hình sang một website khác.
* **Import** (Nhập vào) — tải tệp đó lên để khôi phục lại các nhóm. Tệp không được nặng quá 10MB.

> **Lưu ý quan trọng khi Import:** Các nhóm được nhập vào sẽ **luôn ở trạng thái "Draft"** (bản nháp). Đây là chủ ý của hệ thống để bạn kiểm tra lại trước. Sau khi nhập xong, bạn phải mở từng nhóm và chuyển sang **"Publish"** thì các ô mới thật sự xuất hiện.

## Lưu ý & xử lý sự cố

**Tạo nhóm xong nhưng vào thêm Tour không thấy ô nào.** Ba nguyên nhân theo thứ tự phổ biến:

1. Nhóm đang ở trạng thái **Draft** → mở nhóm, chuyển sang **Publish**.
2. Bạn quên chọn loại dịch vụ ở bước 3, hoặc chọn nhầm loại khác (chọn Hotel nhưng lại đi kiểm tra ở Tour).
3. Trình duyệt còn giữ trang cũ → nhấn **Ctrl + F5** để tải lại trang cho sạch.

**Hệ thống không cho lưu, báo lỗi đỏ.** Kiểm tra 2 chỗ bắt buộc: **"Title"** (tên nhóm) đã điền chưa, và **loại dịch vụ** đã chọn ít nhất một cái chưa.

**Ô "Field Name" bị trùng.** Hai ô trong cùng một nhóm không được trùng tên kỹ thuật. Nếu bạn đặt hai nhãn giống hệt nhau, hệ thống sẽ sinh ra tên trùng. Hãy đổi nhãn cho khác nhau.

**Đã nhập dữ liệu cho 50 tour, giờ sửa Field Name thì sao?** Dữ liệu cũ của 50 tour đó sẽ **không hiển thị nữa** vì hệ thống tìm theo tên kỹ thuật. Nguyên tắc vàng: **đặt tên một lần, dùng mãi mãi**. Muốn đổi chữ hiển thị thì chỉ sửa **"Field Label"** thôi — cái này sửa thoải mái, không ảnh hưởng dữ liệu.

**Nên tạo bao nhiêu ô là vừa?** Chỉ tạo những ô bạn **thật sự sẽ dùng**. Nhiều đơn vị hào hứng tạo 20 ô rồi bỏ trống 18 ô, khiến nhân viên nhập liệu rối và nản. Hãy bắt đầu từ 2-3 ô thiết yếu, thiếu thì thêm sau — thêm lúc nào cũng được.

## Xem thêm

* [4.9. Cài đặt](cai-dat.md) — cấu hình chung của toàn hệ thống
* [4.11. Công cụ](cong-cu.md) — nơi dịch các nhãn tiếng Anh sang tiếng Việt
