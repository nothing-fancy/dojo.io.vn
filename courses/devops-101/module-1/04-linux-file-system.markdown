---
title:  "Giới thiệu về hệ thống thư mục trong Linux"
date:   2024-07-22 00:00:00 +0700
breadcrumbs: true

toc: true
toc_label: "Có gì trong bài này?"
toc_icon: "cog"
---
## Bạn sẽ tìm hiểu được kiến thức gì sau bài này

Sau khi hoàn thành bài viết này, bạn sẽ có kiến thức về:
- Tổng quan về hệ thống thư mục trong hệ điều hành Linux.
- Cấu trúc cây thư mục và vai trò của từng thư mục chính.
- Cách sử dụng các lệnh liên quan đến hệ thống thư mục.
- Hiểu biết sâu hơn về cách quản lý và duy trì hệ thống thư mục trong Linux.

## Chương 1: Tổng quan về hệ thống thư mục trong hệ điều hành Linux

### 1.1 Khái niệm hệ thống thư mục
Hệ thống thư mục trong Linux là một cấu trúc cây được tổ chức từ thư mục gốc (root directory) và các thư mục con. Nó cung cấp một cách tổ chức dữ liệu và các tài nguyên trên hệ thống.

### 1.2 Thư mục gốc (Root Directory)
Thư mục gốc, ký hiệu là `/`, là điểm bắt đầu của hệ thống thư mục. Mọi thư mục và tệp tin khác đều nằm trong thư mục gốc hoặc các thư mục con của nó.

### 1.3 Tầm quan trọng của hệ thống thư mục
Hệ thống thư mục giúp tổ chức và quản lý dữ liệu một cách hiệu quả, giúp người dùng và hệ thống dễ dàng truy cập và quản lý tệp tin.

## Chương 2: Cấu trúc cây thư mục

### 2.1 Thư mục `/bin`
Thư mục này chứa các chương trình thực thi (binaries) thiết yếu của hệ thống mà tất cả người dùng cần dùng, như các lệnh `ls`, `cp`, `mv`, `rm`.

### 2.2 Thư mục `/sbin`
Thư mục này chứa các chương trình thực thi cần thiết cho quản trị hệ thống, như `fsck`, `reboot`, `shutdown`.

### 2.3 Thư mục `/etc`
Thư mục này chứa các tập tin cấu hình hệ thống và các script khởi động.

### 2.4 Thư mục `/home`
Thư mục này chứa các thư mục cá nhân của người dùng, mỗi người dùng có một thư mục riêng trong `/home`, ví dụ: `/home/user1`, `/home/user2`.

### 2.5 Thư mục `/lib`
Thư mục này chứa các thư viện chia sẻ cần thiết cho các chương trình trong `/bin` và `/sbin`.

### 2.6 Thư mục `/usr`
Thư mục này chứa các ứng dụng và tệp tin được sử dụng bởi người dùng, bao gồm các chương trình, thư viện, và tài liệu.

### 2.7 Thư mục `/var`
Thư mục này chứa các tệp tin thay đổi thường xuyên như nhật ký (log files), hàng đợi thư (mail spool), và tệp tin tạm thời.

### 2.8 Thư mục `/tmp`
Thư mục này chứa các tệp tin tạm thời được tạo ra bởi hệ thống và người dùng.

### 2.9 Thư mục `/dev`
Thư mục này chứa các tệp đặc biệt đại diện cho các thiết bị phần cứng, như ổ đĩa, thiết bị đầu vào/đầu ra.

### 2.10 Thư mục `/proc`
Thư mục này chứa thông tin về các tiến trình đang chạy và trạng thái hệ thống.

### 2.11 Thư mục `/mnt` và `/media`
Thư mục này được sử dụng để gắn kết các hệ thống tệp tin bên ngoài, như ổ đĩa CD, USB, hoặc các phân vùng khác.

## Chương 3: Quản lý hệ thống thư mục

### 3.1 Tạo và xóa thư mục
- **Tạo thư mục**: Sử dụng lệnh `mkdir` để tạo thư mục mới, ví dụ: `mkdir /home/user/newdir`.
- **Xóa thư mục**: Sử dụng lệnh `rmdir` để xóa thư mục trống, hoặc `rm -r` để xóa thư mục và tất cả nội dung bên trong.

### 3.2 Di chuyển và đổi tên thư mục
- **Di chuyển thư mục**: Sử dụng lệnh `mv` để di chuyển hoặc đổi tên thư mục, ví dụ: `mv /home/user/olddir /home/user/newdir`.

### 3.3 Thay đổi quyền truy cập thư mục
- **Thay đổi quyền truy cập**: Sử dụng lệnh `chmod` để thay đổi quyền truy cập của thư mục, ví dụ: `chmod 755 /home/user/newdir`.
- **Thay đổi chủ sở hữu**: Sử dụng lệnh `chown` để thay đổi chủ sở hữu của thư mục, ví dụ: `chown user:group /home/user/newdir`.

### 3.4 Kiểm tra và quản lý dung lượng đĩa
- **Kiểm tra dung lượng đĩa**: Sử dụng lệnh `df` để kiểm tra dung lượng đĩa, ví dụ: `df -h`.
- **Kiểm tra dung lượng thư mục**: Sử dụng lệnh `du` để kiểm tra dung lượng thư mục, ví dụ: `du -sh /home/user/newdir`.

## Chương 4: Các công cụ và lệnh quản lý hệ thống thư mục

### 4.1 `ls`
Lệnh `ls` liệt kê nội dung của thư mục, ví dụ: `ls /home/user`.

### 4.2 `cd`
Lệnh `cd` thay đổi thư mục hiện tại, ví dụ: `cd /home/user`.

### 4.3 `pwd`
Lệnh `pwd` in ra đường dẫn của thư mục hiện tại.

### 4.4 `find`
Lệnh `find` tìm kiếm các tệp tin và thư mục trong hệ thống, ví dụ: `find /home/user -name "*.txt"`.

### 4.5 `cp`
Lệnh `cp` sao chép tệp tin và thư mục, ví dụ: `cp -r /home/user/newdir /home/user/backupdir`.

### 4.6 `ln`
Lệnh `ln` tạo liên kết đến tệp tin hoặc thư mục, ví dụ: `ln -s /home/user/newdir /home/user/linktodir`.

## Những điểm cần nhớ (Key Take-aways)

- **Cấu trúc cây thư mục**: Linux sử dụng cấu trúc cây thư mục bắt đầu từ thư mục gốc `/`.
- **Thư mục quan trọng**: Các thư mục chính như `/bin`, `/sbin`, `/etc`, `/home`, `/lib`, `/usr`, `/var`, `/tmp`, `/dev`, `/proc`, `/mnt`, và `/media` có vai trò quan trọng trong hệ thống.
- **Quản lý thư mục**: Sử dụng các lệnh như `mkdir`, `rmdir`, `mv`, `chmod`, `chown`, `df`, `du` để quản lý và duy trì hệ thống thư mục.
- **Công cụ và lệnh**: Các lệnh như `ls`, `cd`, `pwd`, `find`, `cp`, `ln` giúp người dùng thao tác và quản lý hệ thống thư mục hiệu quả.
- **Bảo mật và quyền truy cập**: Hiểu và sử dụng đúng các quyền truy cập và quyền sở hữu là yếu tố quan trọng trong việc bảo vệ dữ liệu và duy trì an ninh hệ thống.

