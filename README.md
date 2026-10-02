# VGSI PILE — Dashboard Doanh thu & Dòng tiền

Trang HTML tĩnh hiển thị dashboard **Doanh thu & Dòng tiền** nhúng trực tiếp từ Excel Online (SharePoint/M365 của VGSI PILE).

## Nội dung

- `index.html` — trang dashboard, nhúng file Excel qua `iframe` (Excel Online embed).
- Tự động refresh iframe mỗi **5 phút** để lấy dữ liệu đã lưu mới nhất.
- Có link **"Mở Excel trực tiếp ↗"** ở góc phải khi cần thao tác đầy đủ trong Excel Online.

## Xem dashboard

Mở trực tiếp file `index.html`, hoặc truy cập GitHub Pages của repo này.

## Lưu ý truy cập

Dữ liệu **không nằm trong repo** — trang chỉ nhúng liên kết tới Excel Online trên SharePoint của VGSI.
Vì vậy ai muốn xem dữ liệu **phải đăng nhập tài khoản Microsoft có quyền truy cập file gốc**.
Repo không chứa số liệu doanh thu, công nợ hay bất kỳ dữ liệu kinh doanh nào.

## Cập nhật dữ liệu

Chỉnh sửa trực tiếp trên file Excel (SharePoint) → dashboard tự hiển thị bản mới sau tối đa 5 phút, **không cần sửa code**.

## Hiển thị trên laptop & điện thoại

Trang đã được tối ưu **responsive**:
- Chiều cao dùng `100dvh` → không bị lệch khi thanh địa chỉ mobile ẩn/hiện.
- Header co lại, nút to hơn, chữ nhỏ hơn trên màn hình ≤ 640px.
- Hỗ trợ **tai thỏ iPhone** (safe-area insets) và chế độ nằm ngang.
- Nút **"Mở Excel đầy đủ ↗"** mở Excel Online toàn trang — cách thao tác dễ nhất trên điện thoại.
- Nút **"↻ Tải lại"** + tự làm mới 5 phút một lần, và làm mới khi quay lại tab (mobile hay treo nền).
- Có thể "Thêm vào màn hình chính" (Add to Home Screen) để dùng như app.

## Triển khai

Trang tĩnh, không cần build. Có thể:
- bật **GitHub Pages** (Settings → Pages → branch `main`, thư mục `/`)
- hoặc copy `index.html` lên bất kỳ web server / hosting tĩnh nào
