# Sổ Thu Chi Shipper

Web app ghi thu nhập và chi phí hằng ngày cho shipper ShopeeFood. Cài lên màn hình chính điện thoại như một app, mở được khi không có mạng.

## Có gì trong app

- **Sổ**: nhập khoản thu và chi, gõ nhanh `35`, `35k`, `35.000,50`. Sửa hoặc xoá khoản đã nhập. Xem lãi ròng theo ngày, tuần, tháng.
- **Thống kê**: biểu đồ lãi ròng từng ngày, mục tiêu, chi và thu theo từng khoản.
- **Xe**: ghi km mỗi ngày, số km trên đồng hồ, tiền xăng mỗi km, nhắc thay nhớt và bảo dưỡng.
- **Cài đặt**: thêm, đổi tên, xoá danh mục. Đặt mục tiêu. Chọn giao diện sáng hoặc tối. Sao lưu, khôi phục, xuất CSV cho Excel.

## Đưa lên GitHub Pages (làm được ngay trên điện thoại)

1. Vào github.com, đăng nhập, bấm dấu **+** rồi **New repository**. Đặt tên, ví dụ `so-thu-chi`. Chọn **Public**. Bấm **Create repository**.
2. Trong repo vừa tạo, bấm **uploading an existing file** (hoặc **Add file** rồi **Upload files**).
3. Chọn đủ 6 file này và tải lên, để tất cả nằm cùng một cấp, không bỏ vào thư mục con:
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `icon-180.png`
   - `icon-192.png`
   - `icon-512.png`
4. Kéo xuống bấm **Commit changes**.
5. Vào **Settings**, chọn **Pages** ở menu bên trái. Ở mục **Build and deployment**, chọn **Deploy from a branch**. Chọn nhánh `main`, thư mục `/ (root)`, bấm **Save**.
6. Chờ khoảng 1 đến 2 phút. Tải lại trang Pages, địa chỉ app hiện ra, dạng `https://TEN-CUA-BAN.github.io/so-thu-chi/`.

## Cài lên điện thoại

- **Android (Chrome)**: mở địa chỉ app, bấm dấu ba chấm, chọn **Cài đặt ứng dụng** hoặc **Thêm vào màn hình chính**.
- **iPhone (Safari)**: mở địa chỉ app, bấm nút Chia sẻ, chọn **Thêm vào Màn hình chính**.

## Lưu ý quan trọng về dữ liệu

- Sổ chỉ lưu trong trình duyệt của điện thoại, không gửi lên máy chủ nào.
- Mỗi địa chỉ web có một kho dữ liệu riêng. Nếu đổi tên repo hoặc đổi địa chỉ, app sẽ trống. Hãy sao lưu trước khi đổi.
- Xoá dữ liệu trình duyệt hoặc gỡ app có thể làm mất sổ. Vào **Cài đặt** rồi **Tải bản sao lưu** mỗi tuần, và gửi file cho chính mình qua Zalo hoặc email.
- Muốn chuyển sang máy mới: sao lưu ở máy cũ, mở app ở máy mới, vào **Cài đặt** rồi **Khôi phục từ file sao lưu**.

## Cập nhật app sau này

Khi có bản `index.html` mới, tải đè lên file cũ trong repo. Đổi `VERSION` trong `sw.js` (ví dụ từ `v1` thành `v2`) để điện thoại tải bản mới. Dữ liệu trong sổ không bị mất khi cập nhật.
