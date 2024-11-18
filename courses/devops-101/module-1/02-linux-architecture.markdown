---
title:  "Kiến trúc hệ điều hành Linux"
date:   2024-07-22 00:00:00 +0700
breadcrumbs: true

toc: true
toc_label: "Có gì trong bài này?"
toc_icon: "cog"
---
## Bạn sẽ tìm hiểu được kiến thức gì sau bài này

Sau khi hoàn thành bài viết này, bạn sẽ có kiến thức về:
- Tổng quan về kiến trúc hệ điều hành Linux.
- Các thành phần chính trong kiến trúc của Linux và chức năng của chúng.
- Cách các thành phần này tương tác và làm việc cùng nhau để quản lý hệ thống.
- Hiểu biết sâu hơn về cách Linux quản lý tài nguyên, tiến trình, bộ nhớ và hệ thống tập tin.

## Chương 1: Tổng quan về kiến trúc hệ điều hành Linux

### 1.1 Khái niệm về hệ điều hành Linux
Linux là một hệ điều hành mã nguồn mở, được phát triển dựa trên nhân Linux. Nó là một hệ điều hành Unix-like, nghĩa là nó có cấu trúc và hành vi tương tự như Unix.

### 1.2 Cấu trúc hệ điều hành Linux
Hệ điều hành Linux có cấu trúc phân tầng, với các thành phần chính bao gồm:
- Kernel (Nhân hệ điều hành)
- System Libraries (Thư viện hệ thống)
- System Utilities (Tiện ích hệ thống)
- User Space (Không gian người dùng)

## Chương 2: Nhân hệ điều hành (Kernel)

### 2.1 Tổng quan về Kernel
Kernel là phần cốt lõi của hệ điều hành Linux. Nó quản lý tài nguyên hệ thống, bao gồm CPU, bộ nhớ và các thiết bị ngoại vi. Kernel là phần mềm trung gian giữa phần cứng và các ứng dụng.

### 2.2 Các thành phần của Kernel
- **Quản lý tiến trình (Process Management)**: Kernel quản lý việc tạo, thực thi và kết thúc các tiến trình. Nó đảm bảo các tiến trình được cấp phát tài nguyên hợp lý và hoạt động hiệu quả.
- **Quản lý bộ nhớ (Memory Management)**: Kernel quản lý bộ nhớ chính của hệ thống, bao gồm việc cấp phát và giải phóng bộ nhớ cho các tiến trình.
- **Quản lý hệ thống tập tin (File System Management)**: Kernel quản lý các hệ thống tập tin, bao gồm việc lưu trữ, tổ chức và truy xuất dữ liệu.
- **Quản lý thiết bị (Device Management)**: Kernel quản lý các thiết bị ngoại vi thông qua các driver thiết bị.

### 2.3 Kernel mode và User mode
Kernel hoạt động ở hai chế độ: Kernel mode (chế độ nhân) và User mode (chế độ người dùng). Kernel mode có quyền truy cập trực tiếp vào phần cứng và tài nguyên hệ thống, trong khi User mode giới hạn quyền truy cập này để bảo vệ hệ thống.

## Chương 3: Thư viện hệ thống (System Libraries)

### 3.1 Vai trò của System Libraries
Thư viện hệ thống cung cấp các hàm cơ bản để các ứng dụng tương tác với kernel. Chúng giúp đơn giản hóa việc phát triển ứng dụng bằng cách cung cấp các API tiêu chuẩn.

### 3.2 Các thư viện phổ biến
- **glibc (GNU C Library)**: Thư viện C chuẩn của GNU, cung cấp các hàm cơ bản như quản lý bộ nhớ, xử lý chuỗi và các hàm hệ thống.
- **libm**: Thư viện toán học chuẩn, cung cấp các hàm toán học như sin, cos, sqrt.

## Chương 4: Tiện ích hệ thống (System Utilities)

### 4.1 Tổng quan về System Utilities
Tiện ích hệ thống bao gồm các chương trình và công cụ giúp quản lý hệ thống, từ các công cụ dòng lệnh đơn giản đến các ứng dụng quản lý hệ thống phức tạp.

### 4.2 Các tiện ích phổ biến
- **bash**: Trình thông dịch dòng lệnh phổ biến trong Linux.
- **cron**: Công cụ lập lịch thực thi các lệnh hoặc kịch bản vào các thời điểm xác định.
- **top**: Công cụ giám sát tiến trình và tài nguyên hệ thống theo thời gian thực.

## Chương 5: Không gian người dùng (User Space)

### 5.1 Tổng quan về User Space
Không gian người dùng là nơi các ứng dụng và quy trình của người dùng chạy. Nó bao gồm tất cả các phần của hệ điều hành mà người dùng tương tác trực tiếp.

### 5.2 Các ứng dụng phổ biến trong User Space
- **Gnome/KDE**: Các môi trường desktop phổ biến trong Linux.
- **Firefox/Chrome**: Các trình duyệt web phổ biến.
- **LibreOffice**: Bộ ứng dụng văn phòng mã nguồn mở.

## Những điểm cần nhớ (Key Take-aways)

- **Kernel**: Là phần cốt lõi của Linux, quản lý tài nguyên hệ thống và cung cấp các dịch vụ cơ bản.
- **System Libraries**: Cung cấp các API tiêu chuẩn giúp ứng dụng tương tác với kernel dễ dàng hơn.
- **System Utilities**: Bao gồm các công cụ và tiện ích giúp quản lý và duy trì hệ thống.
- **User Space**: Là nơi các ứng dụng của người dùng chạy và tương tác với hệ điều hành.
- **Kiến trúc phân tầng**: Linux có kiến trúc phân tầng, giúp tách biệt các chức năng và tăng cường bảo mật cũng như hiệu suất của hệ thống.
