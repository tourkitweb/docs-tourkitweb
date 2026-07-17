# DANH SÁCH ẢNH CẦN CHỤP BỔ SUNG

> File này là **ghi chú công việc nội bộ**, không nằm trong `SUMMARY.md` nên GitBook không xuất bản ra ngoài.
> Xóa file này khi đã chụp xong toàn bộ.

**Tổng: 53 vị trí ảnh trên 10 trang** (các trang module mới, trước đây chưa có tài liệu nên chưa có ảnh).

## Cách nhận biết chỗ cần chèn ảnh

Mọi vị trí đều có cùng một định dạng, tìm bằng cách gõ `📷` là ra hết:

```markdown
> 📷 *[Cần chụp màn hình: mô tả màn hình cần chụp]*
```

Khi có ảnh, **thay nguyên dòng đó** bằng:

```markdown
![](../.gitbook/assets/<tên-file-ảnh>.png)
```

Lệnh liệt kê lại toàn bộ vị trí còn thiếu bất cứ lúc nào:

```bash
grep -rn "📷" --include="*.md" .
```

## Quy ước đặt tên ảnh

Ảnh cũ theo hệ `pgXXX-N.png` (số trang trong file PDF gốc). Ảnh mới **không nên** theo hệ này vì không có trang PDF tương ứng. Đề xuất đặt theo module cho dễ tra:

```
xe-01.png, xe-02.png, ...
du-thuyen-01.png, ...
```

Tất cả ảnh để chung trong thư mục `.gitbook/assets/`.

---

# CHECKLIST THEO TRANG

## Khối Sản phẩm

### `khoi-san-pham/xe.md` — 5 ảnh
- [ ] dòng 13 — menu Xe đang mở ở cột trái, thấy đủ 5 mục con
- [ ] dòng 31 — danh sách xe tại **Xe > Tất cả xe**, thấy ô tìm kiếm, cột chọn, danh sách
- [ ] dòng 62 — **Xe > Thêm xe mới**, thấy rõ các tab Nội dung, Địa điểm, Giá, Thuộc tính
- [ ] dòng 115 — **Xe > Thuộc tính**
- [ ] dòng 131 — **Xe > Cập nhật giá**, thấy lưới lịch theo tháng và giá trên từng ô ngày

### `khoi-san-pham/thuyen.md` — 5 ảnh
- [ ] dòng 23 — menu Thuyền đang mở, thấy đủ 5 mục con
- [ ] dòng 41 — danh sách tại **Thuyền > Tất cả thuyền**
- [ ] dòng 65 — **Thuyền > Thêm thuyền mới**, thấy các tab Nội dung, Địa điểm, Giá, Thuộc tính
- [ ] dòng 129 — **Thuyền > Thuộc tính**
- [ ] dòng 145 — **Thuyền > Cập nhật giá**, thấy lưới lịch theo tháng

### `khoi-san-pham/du-thuyen.md` — 5 ảnh
- [ ] dòng 18 — menu Du thuyền đang mở, đầy đủ mục con
- [ ] dòng 42 — **Thêm du thuyền mới**, các ô thông tin cơ bản
- [ ] dòng 69 — khu vực khai báo danh sách **phòng/cabin** trong trang sửa du thuyền
- [ ] dòng 94 — **Du thuyền > Cập nhật giá**, lịch theo ngày + ô nhập giá/số phòng
- [ ] dòng 104 — **Du thuyền > Khôi phục**, danh sách đã xóa

### `khoi-san-pham/khong-gian.md` — 4 ảnh
- [ ] dòng 16 — menu Không gian đang mở, đầy đủ mục con
- [ ] dòng 38 — **Thêm không gian mới**, các ô thông tin cơ bản
- [ ] dòng 82 — **Không gian > Cập nhật giá**, lịch theo ngày + ô nhập giá
- [ ] dòng 92 — **Không gian > Khôi phục**

### `khoi-san-pham/chuyen-bay.md` — 5 ảnh
- [ ] dòng 18 — menu Chuyến bay đang mở, đầy đủ mục con
- [ ] dòng 48 — **Chuyến bay > Hãng hàng không**
- [ ] dòng 56 — **Chuyến bay > Sân bay**
- [ ] dòng 62 — **Chuyến bay > Loại ghế**
- [ ] dòng 72 — **Thêm chuyến bay mới**, các ô hãng bay, sân bay đi/đến, giờ bay

### `khoi-san-pham/khoa-hoc.md` — 6 ảnh
- [ ] dòng 13 — menu Khóa học đang mở, thấy đủ 5 mục con
- [ ] dòng 33 — **Khóa học > Tất cả các khóa học**
- [ ] dòng 59 — **Khóa học > Add new course** (nhãn hiện tiếng Anh trên giao diện)
- [ ] dòng 99 — **Khóa học > Danh mục**
- [ ] dòng 123 — **Khóa học > Cấp độ**
- [ ] dòng 136 — **Khóa học > Thuộc tính**

### `khoi-san-pham/tai-san.md` — 6 ảnh
- [ ] dòng 13 — menu Tài sản đang mở, thấy đủ 5 mục con
- [ ] dòng 40 — **Tài sản > Tất cả các tài sản**
- [ ] dòng 66 — **Thêm tài sản mới**, thấy các tab Nội dung, Địa điểm, Giá, Thuộc tính
- [ ] dòng 123 — **Tài sản > Thuộc tính**
- [ ] dòng 139 — **Tài sản > Danh mục**
- [ ] dòng 159 — **Tài sản > Liên hệ tài sản**, bảng danh sách yêu cầu liên hệ

### `khoi-san-pham/don-hang.md` — 2 ảnh
- [ ] dòng 24 — danh sách **Đơn hàng**
- [ ] dòng 64 — trang chi tiết / chỉnh sửa một đơn hàng

## Khối Hệ thống

### `khoi-he-thong/slide-item.md` — 5 ảnh
- [ ] dòng 17 — **dải logo đối tác chạy ngang trên trang chủ website** (ảnh ngoài web, không phải admin — để khách hình dung "slide item" là cái gì)
- [ ] dòng 27 — menu Slide item đang mở, thấy đủ 3 mục con
- [ ] dòng 45 — **Slide item > Danh mục**
- [ ] dòng 68 — **Slide item > Tất cả item**, bảng cột Ảnh, Tiêu đề, Danh mục, Thứ tự, Trạng thái
- [ ] dòng 83 — **Thêm slide item**, các ô Tiêu đề, Nhãn, Danh mục, Hình ảnh, URL liên kết, Mô tả, Thứ tự, Trạng thái

### `khoi-he-thong/ket-noi-khach-san.md` — 4 ảnh
- [ ] dòng 17 — trang chính mục **Kết nối khách sạn**
- [ ] dòng 46 — **Cài đặt API**
- [ ] dòng 71 — **Cấu hình giá**
- [ ] dòng 94 — **Nhật ký API**

> ⚠️ Đây là app Pro `HotelConnect`. Nếu chưa bật trên máy local thì **không chụp được** — cần bật app trước hoặc lấy ảnh từ site thật.

### `khoi-he-thong/doi-ngu.md` — 3 ảnh
- [ ] dòng 13 — mục Đội ngũ trong menu trái, nhóm Hệ thống
- [ ] dòng 27 — danh sách thành viên, cột Ảnh, Tên, Chức danh, Thứ tự, Trạng thái
- [ ] dòng 37 — **Thêm thành viên**, các ô Họ và tên, Chức danh, Ảnh đại diện, Thứ tự sắp xếp, Trạng thái

### `khoi-he-thong/bao-mat-2-lop.md` — 3 ảnh
- [ ] dòng 23 — **Bảo mật 2 lớp > 2FA của tôi**, hiện mã QR và ô nhập mã 6 số
- [ ] dòng 91 — giao diện **Google Authenticator trên điện thoại**, mã 6 số + vòng tròn đếm ngược *(ảnh chụp điện thoại, không phải màn hình máy tính)*
- [ ] dòng 111 — trang 2FA của tôi hiện mã QR cùng **khóa bí mật** dạng chữ và số

> ⚠️ **Che/làm mờ mã QR và khóa bí mật thật trước khi đăng.** Ai quét được mã đó sẽ tạo được mã đăng nhập vào tài khoản.

---

# LƯU Ý KHI CHỤP

1. **Che dữ liệu nhạy cảm** — email/SĐT khách thật, mã QR 2FA, khóa bí mật, API key, số tài khoản ngân hàng.
2. **Dùng dữ liệu mẫu trông hợp lý** — tên tour thật, giá thật. Ảnh có "test test 123" làm khách mất tin tưởng.
3. **Chụp đủ ngữ cảnh** — nên thấy cả menu trái để khách biết mình đang ở đâu.
4. **Thống nhất độ rộng trình duyệt** (gợi ý 1440px) để ảnh đều nhau.
5. **Ngôn ngữ giao diện để tiếng Việt**, trừ các nhãn vốn hiện tiếng Anh (Custom Fields, Field Groups, Add New Group, Add new course) — với các nhãn đó chụp đúng như giao diện thật, vì tài liệu đã ghi rõ chúng hiện tiếng Anh.

# PHƯƠNG ÁN TỰ ĐỘNG CHỤP

Máy đã có sẵn **Playwright 1.61.1**, site local chạy tại `http://localhost`, trang đăng nhập `/login`, admin ở `/admin`.
Có thể viết script tự đăng nhập rồi chụp lần lượt từng trang. **Cần: tài khoản admin local.**

Điều kiện: các module Xe / Thuyền / Du thuyền / Không gian / Chuyến bay / Khóa học / Tài sản phải **đang được bật** thì mới vào chụp được — nếu module tắt, menu không hiện.
