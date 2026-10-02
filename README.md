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

## Triển khai

Trang tĩnh, không cần build. Có thể:
- bật **GitHub Pages** (Settings → Pages → branch `main`, thư mục `/`)
- hoặc copy `index.html` lên bất kỳ web server / hosting tĩnh nào
