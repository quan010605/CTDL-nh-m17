
# Quản Lý Album Ảnh

## Giới thiệu

Đây là chương trình quản lý album ảnh đơn giản được viết bằng ngôn ngữ lập trình C. Dự án cho phép bạn thêm, sửa, xoá, tìm kiếm và hiển thị ảnh,phát hiện và xóa ảnh trùng lặp, khôi phục ảnh với các thông tin như: mã ảnh (ID), ngày chụp, giờ chụp, địa điểm chụp.

## Cấu trúc dữ liệu

- Sử dụng danh sách liên kết đơn (`linked list`) để lưu trữ các ảnh.
- Mỗi ảnh được lưu dưới dạng một `struct Image` với các trường:
  - `int id`: mã ảnh duy nhất.
  - `char ngay[11]`: ngày chụp.
  - `char gio[9]`: giờ chụp.
  - `char diaDiem[30]`: địa điểm chụp.

## Các chức năng chính

| STT | Chức năng                | Mô tả ngắn gọn                                  |
|-----|---------------------------|--------------------------------------------------|
| 1️⃣ | Thêm ảnh                  | Thêm một ảnh mới vào cuối danh sách              |
| 2️⃣ | Hiển thị danh sách ảnh   | In toàn bộ thông tin ảnh trong album             |
| 3️⃣ | Tìm ảnh theo ID          | Tìm kiếm và hiển thị ảnh có ID cụ thể            |
| 4️⃣ | Xoá ảnh theo ID          | Xoá ảnh khỏi danh sách theo ID                   |
| 5️⃣ | Sửa thông tin ảnh        | Cập nhật thông tin ảnh dựa trên ID               |
| 6️⃣ | Đọc/Ghi file             | Lưu và nạp dữ liệu album từ file văn bản         |
| 7️⃣ | Tìm ảnh trùng lặp (sắp thêm) | Phát hiện và xử lý các ảnh có nội dung trùng lặp |
| 8️⃣ | Khôi phục thùng rác (sắp thêm) | Lưu các ảnh đã xoá tạm thời để phục hồi nếu cần |

## Cách sử dụng

1. **Biên dịch chương trình:**
   ```bash
   gcc main.c -o album
   ```
2. **Chạy chương trình:**
   ```bash
   ./album
   ```
3. **Làm theo hướng dẫn trong menu để thao tác với album ảnh.**

## Mở rộng

- Chuyển từ danh sách liên kết sang mảng động hoặc `vector` (nếu chuyển sang C++).
- Thêm giao diện người dùng bằng đồ họa.
- Kết nối với cơ sở dữ liệu.

## Tác giả

- Họ tên: Hà Trọng Quân, Nguyễn Hà Phương, Vũ Bá Minh Phúc
