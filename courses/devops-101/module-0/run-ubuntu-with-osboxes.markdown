---
title:  "Hướng dẫn tạo máy ảo Ubuntu trên VirtualBox"
date:   2024-07-22 00:00:00 +0700
breadcrumbs: true

toc: true
toc_label: "Có gì trong bài này?"
toc_icon: "cog"
---

## Giới Thiệu
osboxes.org cung cấp các máy ảo cài sẵn nhiều hệ điều hành khác nhau, bao gồm Ubuntu. Sử dụng máy ảo từ [osboxes.org](https://www.osboxes.org/ubuntu/) giúp tiết kiệm thời gian cài đặt và cấu hình.

## Yêu Cầu Hệ Thống
- Hệ điều hành: Windows 7 SP1, 8, 10 hoặc Windows 11.
- Bộ xử lý: CPU 1.5 GHz hoặc nhanh hơn.
- RAM: 2 GB trở lên (khuyến nghị 4 GB hoặc nhiều hơn).
- Dung lượng ổ cứng: 10 GB hoặc nhiều hơn (tùy thuộc vào kích thước máy ảo).

## Thực hiện
### Bước 1: Tải VirtualBox
1. Nếu chưa cài đặt VirtualBox, truy cập trang chủ [VirtualBox](https://www.virtualbox.org/) và tải về phiên bản cho Windows.
2. Cài đặt VirtualBox theo hướng dẫn cài đặt tại [Hướng dẫn cài đặt VSCode trên HĐH Windows](./install-virtualbox.html)

### Bước 2: Tải Máy Ảo Ubuntu từ osboxes.org
1. Mở trình duyệt web và truy cập trang chủ của [osboxes.org](https://www.osboxes.org/ubuntu/).
2. Chọn phiên bản Ubuntu bạn muốn tải về.
3. Nhấp vào liên kết tải về phù hợp với VirtualBox.
4. Giải nén file tải về (.7z) bằng phần mềm giải nén như 7-Zip.

### Bước 3: Cấu Hình Máy Ảo Ubuntu trong VirtualBox
1. Mở VirtualBox.
2. Nhấp vào nút **New** để tạo một máy ảo mới.
3. Đặt tên cho máy ảo và chọn **Type** là `Linux` và **Version** là `Ubuntu (64-bit)`.
4. Nhấp **Next** và chọn dung lượng RAM cấp phát cho máy ảo (khuyến nghị ít nhất 2 GB).
5. Chọn **Use an existing virtual hard disk file** và duyệt đến file .vdi bạn vừa giải nén từ osboxes.org.
6. Nhấp **Create** để hoàn tất việc tạo máy ảo.

### Bước 4: Khởi Động và Cấu Hình Máy Ảo Ubuntu
1. Chọn máy ảo Ubuntu từ danh sách máy ảo trong VirtualBox và nhấp vào **Start** để khởi động.
2. Đăng nhập vào Ubuntu sử dụng thông tin tài khoản cung cấp bởi osboxes.org (thường là `osboxes.org` cho cả username và password).
3. Cập nhật hệ điều hành và các gói phần mềm cần thiết bằng cách mở terminal và chạy lệnh:
    ```bash
    sudo apt update && sudo apt upgrade
    ```

### Bước 5: Tối Ưu Hóa Máy Ảo (Tùy Chọn)
1. Cài đặt Guest Additions để cải thiện hiệu suất và trải nghiệm sử dụng.
2. Chọn **Devices** > **Insert Guest Additions CD image...** từ menu của VirtualBox.
3. Làm theo hướng dẫn cài đặt trong máy ảo Ubuntu.

## Kết Luận
Bằng cách làm theo các bước trên, bạn đã tải về và sử dụng thành công máy ảo Ubuntu từ osboxes.org trên VirtualBox chạy trên Windows. Máy ảo giúp bạn dễ dàng trải nghiệm và phát triển phần mềm trên hệ điều hành Ubuntu mà không cần cài đặt trực tiếp lên máy tính.

## Tài Liệu Tham Khảo
- [Trang chủ VirtualBox](https://www.virtualbox.org/)
- [Trang chủ osboxes.org](https://www.osboxes.org/)
- [Hướng dẫn sử dụng VirtualBox](https://www.virtualbox.org/manual/UserManual.html)
