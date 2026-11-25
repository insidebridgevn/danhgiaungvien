# Đánh giá ứng viên — IBVN

Trang để các phòng ban xem hồ sơ ứng tuyển và đánh giá ứng viên (GitHub Pages).

- Giao diện: `index.html` (một file, không cần build).
- Dữ liệu: Google Sheet tuyển dụng, đọc/ghi qua Apps Script (file Code.gs của project Leader).
- Đăng nhập: chọn phòng ban + mã của phòng. Lần đầu mỗi phòng tự tạo mã; quên mã thì
  "Quản lý trang" reset trong mục **Quản lý tài khoản**.

## Cấu hình

Trong `index.html`, phần `CONFIG` đầu thẻ `<script>`:

```js
var API_URL = '';   // link /exec của Apps Script trang Leader
```

Để trống thì trang chạy chế độ xem trước với dữ liệu mẫu.
