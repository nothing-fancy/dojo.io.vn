---
title:  "Hướng dẫn cài đặt VirtualBox trên HĐH Windows"
date:   2024-07-22 00:00:00 +0700
breadcrumbs: true

toc: true
toc_label: "Có gì trong bài này?"
toc_icon: "cog"
---

## Giới Thiệu
VirtualBox là một phần mềm ảo hóa mã nguồn mở được phát triển bởi Oracle, cho phép bạn chạy nhiều hệ điều hành trên một máy tính duy nhất. Nó hỗ trợ nhiều hệ điều hành khách như Windows, Linux, macOS và nhiều hơn nữa.

## Yêu Cầu Hệ Thống
- Hệ điều hành: Windows 7 SP1, 8, 10 hoặc Windows 11.
- Bộ xử lý: CPU 1.5 GHz hoặc nhanh hơn.
- RAM: 2 GB trở lên (khuyến nghị 4 GB hoặc nhiều hơn).
- Dung lượng ổ cứng: 200 MB cho cài đặt cơ bản (thêm dung lượng cho các máy ảo).

## Cài đặt
### Bước 1: Tải VirtualBox
1. Mở trình duyệt web và truy cập trang chủ của VirtualBox tại [virtualbox.org](https://www.virtualbox.org/).
2. Nhấp vào nút **Download VirtualBox**.
3. Chọn phiên bản dành cho Windows để tải file cài đặt.

### Bước 2: Cài Đặt VirtualBox
1. Sau khi tải về, nhấp đúp vào file cài đặt `VirtualBox-x.x.x-xxxxxx-Win.exe`.
2. Cửa sổ cài đặt VirtualBox sẽ hiện ra. Nhấp vào **Next** để bắt đầu.
3. Chọn các thành phần muốn cài đặt (giữ nguyên mặc định nếu không chắc chắn), sau đó nhấp **Next**.
4. Chọn thư mục cài đặt (hoặc giữ nguyên mặc định) và nhấp **Next**.
5. Bạn sẽ thấy một cảnh báo về việc cài đặt các driver mạng. Nhấp **Yes** để tiếp tục.
6. Nhấp **Install** để bắt đầu quá trình cài đặt.
7. Khi quá trình cài đặt hoàn tất, nhấp **Finish** để kết thúc. VirtualBox sẽ tự động khởi động.

### Bước 3: Cài Đặt Extension Pack (Tùy Chọn)
1. Truy cập trang tải về của VirtualBox và tìm **VirtualBox Extension Pack**.
2. Tải file `Oracle_VM_VirtualBox_Extension_Pack-x.x.x.vbox-extpack`.
3. Mở VirtualBox và vào **File** > **Preferences** > **Extensions**.
4. Nhấp vào biểu tượng thêm mới (hình dấu cộng) và chọn file Extension Pack vừa tải về.
5. Làm theo hướng dẫn để cài đặt Extension Pack.

### Bước 4: Tạo Máy Ảo Mới
1. Mở VirtualBox.
2. Nhấp vào nút **New** để tạo một máy ảo mới.
3. Đặt tên cho máy ảo và chọn hệ điều hành khách (Windows, Linux, macOS, v.v.).
4. Chọn dung lượng RAM cấp phát cho máy ảo (khuyến nghị ít nhất 2 GB).
5. Tạo ổ cứng ảo mới hoặc chọn ổ cứng ảo đã có.
6. Làm theo hướng dẫn để hoàn tất quá trình tạo máy ảo.

## Kết Luận
VirtualBox là một công cụ mạnh mẽ và linh hoạt cho việc ảo hóa. Bằng cách làm theo các bước trên, bạn đã cài đặt thành công VirtualBox trên máy tính Windows của mình và có thể bắt đầu tạo và quản lý các máy ảo.

## Tài Liệu Tham Khảo
- [Trang chủ VirtualBox](https://www.virtualbox.org/)
- [Hướng dẫn sử dụng VirtualBox](https://www.virtualbox.org/manual/UserManual.html)
