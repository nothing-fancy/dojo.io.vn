---
title:  "Quản lý truy cập và xác thực trong HĐH Linux"
date:   2024-07-22 00:00:00 +0700
breadcrumbs: true

toc: true
toc_label: "Có gì trong bài này?"
toc_icon: "cog"
---

## Bạn sẽ tìm hiểu được kiến thức gì sau bài này

Sau khi hoàn thành bài viết này, bạn sẽ có kiến thức về:
- Tổng quan về xác thực và quản lý quyền hạn trong hệ điều hành Linux.
- Các phương pháp và cơ chế xác thực trong Linux.
- Cách quản lý quyền hạn của người dùng và nhóm người dùng.
- Các công cụ và lệnh quản lý xác thực và quyền hạn.
- Hiểu biết sâu hơn về bảo mật hệ thống thông qua xác thực và quản lý quyền hạn.

## Chương 1: Tổng quan về xác thực và quản lý quyền hạn trong hệ điều hành Linux

### 1.1 Khái niệm về xác thực
Xác thực (authentication) là quá trình kiểm tra và xác nhận danh tính của người dùng hoặc thực thể đang cố gắng truy cập vào hệ thống.

### 1.2 Khái niệm về quản lý quyền hạn
Quản lý quyền hạn (authorization) là quá trình phân quyền và kiểm soát những hành động mà người dùng hoặc nhóm người dùng có thể thực hiện trên hệ thống.

### 1.3 Tầm quan trọng của xác thực và quản lý quyền hạn
Xác thực và quản lý quyền hạn đóng vai trò quan trọng trong việc bảo vệ hệ thống khỏi các truy cập trái phép và bảo đảm an ninh thông tin.

## Chương 2: Các phương pháp xác thực trong Linux

### 2.1 Xác thực bằng mật khẩu
Mật khẩu là phương pháp xác thực phổ biến nhất trong Linux. Mật khẩu của người dùng được lưu trữ dưới dạng mã hóa trong file `/etc/shadow`.

### 2.2 Xác thực bằng SSH keys
SSH keys là một phương pháp xác thực mạnh mẽ hơn mật khẩu. Người dùng tạo ra một cặp khóa (public key và private key) và đăng ký khóa công khai (public key) trên máy chủ.

### 2.3 Xác thực bằng Kerberos
Kerberos là một giao thức xác thực mạng sử dụng vé (tickets) để cho phép các node tin cậy nhau trên mạng không an toàn.

### 2.4 Xác thực bằng PAM (Pluggable Authentication Modules)
PAM là một cơ chế linh hoạt và có thể mở rộng để xác thực người dùng. PAM cho phép quản trị viên cấu hình các phương thức xác thực khác nhau cho các dịch vụ khác nhau.

## Chương 3: Quản lý quyền hạn trong Linux

### 3.1 Người dùng và nhóm người dùng
Linux quản lý quyền hạn thông qua hệ thống người dùng và nhóm người dùng. Mỗi người dùng có một UID (User ID) và mỗi nhóm có một GID (Group ID).

### 3.2 Các quyền truy cập tệp tin
Quyền truy cập tệp tin trong Linux được phân thành ba loại: đọc (read), ghi (write) và thực thi (execute). Các quyền này có thể được thiết lập cho chủ sở hữu (owner), nhóm (group) và những người dùng khác (others).

### 3.3 Quản lý quyền hạn bằng lệnh `chmod`
Lệnh `chmod` (change mode) được sử dụng để thay đổi quyền truy cập của tệp tin và thư mục. Quyền truy cập có thể được thiết lập dưới dạng số hoặc ký tự.

### 3.4 Quản lý quyền hạn bằng lệnh `chown` và `chgrp`
Lệnh `chown` (change owner) và `chgrp` (change group) được sử dụng để thay đổi chủ sở hữu và nhóm của tệp tin và thư mục.

## Chương 4: Các công cụ và lệnh quản lý xác thực và quyền hạn

### 4.1 `passwd`
Lệnh `passwd` được sử dụng để thay đổi mật khẩu của người dùng.

### 4.2 `sudo`
Lệnh `sudo` cho phép người dùng chạy các lệnh với quyền hạn của người dùng khác, thường là quyền hạn của người dùng root.

### 4.3 `usermod`, `useradd` và `userdel`
Các lệnh `usermod`, `useradd` và `userdel` được sử dụng để quản lý người dùng. `usermod` chỉnh sửa các thuộc tính của người dùng hiện có, `useradd` tạo người dùng mới và `userdel` xóa người dùng.

### 4.4 `groupmod`, `groupadd` và `groupdel`
Các lệnh `groupmod`, `groupadd` và `groupdel` được sử dụng để quản lý nhóm người dùng. `groupmod` chỉnh sửa các thuộc tính của nhóm hiện có, `groupadd` tạo nhóm mới và `groupdel` xóa nhóm.

## Những điểm cần nhớ (Key Take-aways)

- **Xác thực**: Quá trình kiểm tra và xác nhận danh tính người dùng thông qua mật khẩu, SSH keys, Kerberos hoặc PAM.
- **Quản lý quyền hạn**: Phân quyền và kiểm soát hành động của người dùng và nhóm người dùng trên hệ thống.
- **Người dùng và nhóm người dùng**: Mỗi người dùng có một UID và mỗi nhóm có một GID.
- **Quyền truy cập tệp tin**: Đọc, ghi và thực thi, được thiết lập cho chủ sở hữu, nhóm và những người dùng khác.
- **Công cụ và lệnh quản lý**: `passwd`, `sudo`, `chmod`, `chown`, `usermod`, `useradd`, `userdel`, `groupmod`, `groupadd`, `groupdel` giúp quản lý xác thực và quyền hạn hiệu quả.
- **Bảo mật hệ thống**: Xác thực và quản lý quyền hạn là yếu tố quan trọng trong việc bảo vệ hệ thống khỏi các truy cập trái phép và bảo đảm an ninh thông tin.
