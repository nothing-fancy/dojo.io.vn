---
title:  "Khóa học DevOps 101"
date:   2024-07-22 00:00:00 +0700
breadcrumbs: true

toc: true
toc_label: "Có gì trong bài này?"
toc_icon: "cog"
---

Khóa học DevOps được thiết kế nhằm cung cấp cho học viên những kiến thức và kỹ năng cần thiết để áp dụng các nguyên tắc DevOps trong quá trình phát triển phần mềm và quản lý hệ thống. DevOps, sự kết hợp giữa Development (Phát triển) và Operations (Vận hành), tập trung vào việc cải thiện sự hợp tác giữa các đội phát triển phần mềm và đội vận hành để tăng cường hiệu suất, chất lượng và tốc độ triển khai phần mềm.

## Mục tiêu khóa học
Hiểu rõ các nguyên tắc và triết lý của DevOps.
Nắm vững các công cụ và công nghệ phổ biến trong DevOps như Docker, Kubernetes, Jenkins, Ansible, Terraform, và các công cụ CI/CD khác.
Phát triển kỹ năng tự động hóa quy trình triển khai và quản lý hạ tầng.
Học cách giám sát và quản lý hiệu suất hệ thống.
Tăng cường khả năng làm việc nhóm và cải thiện quy trình làm việc giữa các đội phát triển và vận hành.


## Đối tượng tham gia
Các nhà phát triển phần mềm muốn mở rộng kiến thức về quy trình triển khai và vận hành.
Các quản trị hệ thống muốn nắm bắt các kỹ thuật và công cụ DevOps.
Các chuyên gia IT muốn nâng cao kỹ năng và hiệu suất làm việc thông qua các phương pháp DevOps.
Sinh viên ngành công nghệ thông tin muốn chuẩn bị cho sự nghiệp trong lĩnh vực DevOps.


## Nội dung khóa học

### Module 0: Cài đặt các công cụ
1. [Hướng dẫn cài đặt VSCode trên HĐH Windows](./module-0/install-vscode.html)
2. [Hướng dẫn cài đặt VirtualBox trên HĐH Windows](./module-0/install-virtualbox.html)
3. [Hướng dẫn tạo máy ảo Ubuntu trên VirtualBox](./module-0/run-ubuntu-with-osboxes.html)

### Module 1: Làm quen với Linux
* [Tài liệu tham khảo](./module-1/00-references.html)
* [Hệ điều hành là gì?](./module-1/01-what-is-an-operating-system.html)
* [Kiến trúc hệ điều hành Linux](./module-1/02-linux-architecture.html)
* [Quản lý truy cập và xác thực trong HĐH Linux](./module-1/03-linux-authentication-and-authorization.html)
* [Giới thiệu về hệ thống thư mục trong Linux](./module-1/04-linux-file-system.html)
* [Shell là gì?](./module-1/05-what-is-a-shell.html)

### Module 2: Mạng máy tính
* Tìm hiểu về mô hình OSI và mô hình TCP/IP
* Tìm hiểu về IP, địa chỉ mạng và quản trị mạng
* Tìm hiểu về giao thức HTTP
* Tìm hiểu về cơ chế phân giải tên miền
* Tìm hiểu về giao thức SSL/TLS
* Tìm hiểu về VPN
* Tìm hiểu về một số công cụ troubleshoot mạng

### Module 3: Ansible – Configuration Managment
* Tìm hiểu về Ansible và các khái niệm xung quanh Ansible
* Làm quen với các thao tác với Ansible
* Thực hành: Dùng Ansible cài đặt ứng dụng lên máy chủ Linux

### Module 4: Làm quen với Docker
* Tìm hiểu Docker và các khái niệm xung quanh Docker
* Tìm hiểu tập lệnh cơ bản của docker: ps, logs, exec, run, start, stop, cp, publish port
* Dockerfile
* Docker Registry
* Docker compose
* Thực hành: 
  * Sử dụng Ansible cài đặt ứng dụng Docker lên máy chủ Linux
  * Đóng gói ứng dụng thành docker image và chạy dưới dạng docker container

### Module 5: Git
* Tổng quan về Git và các câu lệnh cơ bản
* Giới thiệu về GitHub và thực hiện tạo remote repository
* Giới thiệu về Gitflow

### Module 6: Tích hợp liên tục với Jenkins
* Giới thiệu về tích hợp liên tục (Continuous Integration - CI)
* Cài đặt Jenkins
* Cấu hình Jenkins Agent
* Tạo và thực thi Jenkins Job đầu tiên
* Thực hành: Build Docker Image và lưu vào Docker Repository
* Tích hợp Jenkins với GitHub và cấu hình Jenkins Job được kích hoạt thực thi dựa trên sự kiện GitHub pull request
* Thực hành: Tạo Jenkins Job: Dựa trên pull request, chạy kiểm thử và gửi kết quả về pull request 
* Thực hành: Tạo Jenkins Job: Dựa vào sự kiện merge lên nhánh `master`, chạy kiểm thử và build docker image và lưu vào Docker Repository

### Module 7: Kubernetes
* Giới thiệu kiến trúc Kubernetes Cài đặt Kubernetes
* Sử dụng kubectl với các lệnh: run, create, describe, get Các khái niệm Pods, RepicaSet, Deployment
* Kubernetes Services: ClusterIP, NodePort, LoadBalancer
* Sử dụng file YAML để triển khai Kubernetes
* Kubernetes dashboard
* DaemonSets, Label, Selectors
* Triển khai RollingUpdate Healthchecks
* ConfigMaps, Secrets Ingress
* Thực hành: Triển khai ứng dụng lên cụm K8s

### Module 8: Triển khai liên tục với ArgoCD
* Giới thiệu về triển khai liên tục (Continuous Deployment - CD)
* Triển khai liên tục lên cụm Kubernetes với ArgoCD
* Thực hành

### Module 9: Thực hành: Xây dựng luồng CI/CD
* Chuẩn bị hạ tầng Linux, K8s
* Tạo git với mã nguồn
* Tạo job CI trên Jenkins
* Cấu hình CD với ArgoCD
* Hoàn tất cấu hình và kiểm tra
