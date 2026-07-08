---
title: "Worklog tuần 1"
date: 2026-04-25
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Mục tiêu tuần 1:
* Phân tích và dự toán tài nguyên hệ thống (RDS, ECS) cho dự án "Mini Social Network".
* Thiết lập môi trường container hóa (Docker) để chuẩn bị cho việc triển khai ứng dụng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nhận Database Schema và tính toán tài nguyên <br>&emsp; + Phân tích cấu trúc DB từ team Backend <br>&emsp; + Tính toán dung lượng RAM/CPU sơ bộ cho RDS và ECS để tối ưu chi phí | 20/04/2026 | 21/04/2026 | Tài liệu nhóm |
| 4 | - Xây dựng kịch bản triển khai (Containerization) <br>&emsp; + Viết file `docker-compose.yml` tạm cho Frontend, Backend và Database <br>&emsp; + Tối ưu hóa Dockerfile Backend (Maven build, JRE) và Frontend (Nginx) | 22/04/2026 | 23/04/2026 | Docker Docs |
| 6 | - Kiểm tra và đóng gói <br>&emsp; + Chạy thử nghiệm hệ thống bằng Docker Compose <br>&emsp; + Kiểm tra cấu hình port và kết nối giữa các container | 24/04/2026 | 25/04/2026 

### Kết quả đạt được tuần 1:
* Đã hoàn thành bảng dự toán cấu hình RAM/CPU cho hạ tầng AWS.
* Thiết lập thành công file `docker-compose.yml` cho phép khởi chạy toàn bộ hệ thống (Frontend, Backend, DB) bằng một lệnh duy nhất.
* Dockerfile được tối ưu hóa, đảm bảo kích thước ảnh nhỏ gọn (sử dụng alpine images).

### Minh chứng thực hiện:

#### 1. Bảng theo dõi tiến độ công việc
Ghi nhận hoàn thành (DONE) các nhiệm vụ kỹ thuật trong tuần 1.
![Bảng tiến độ tuần 1](/images/Tuan1.png)

Gửi file docker-compose.yaml lên nhóm zalo.
![Đã gửi lên zalo](/images/Tuan1-1.png)

#### 2. Kịch bản triển khai (Infrastructure Code)
File `docker-compose.yml` được cấu hình để quản lý liên kết giữa các thành phần hệ thống.
![File docker-compose.yml](/images/Tuan1-3.png)

#### 3. Kết quả Docker hóa
Terminal thể hiện quá trình build thành công các image Backend và Frontend.
![Terminal build Docker](/images/Tuan1-2.png)