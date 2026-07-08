---
title: "Worklog tuần 3"
date: 2026-05-10
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:
* Xây dựng luồng CI/CD tự động bằng công cụ Jenkins (Jenkinsfile) theo chuẩn DevOps.
* Sửa lỗi (Bug Fixes) tồn đọng ở giai đoạn Unit Test và tối ưu luồng Pipeline cho Frontend.
* Đóng gói (Dockerize) thành công mã nguồn và đẩy lên kho lưu trữ Amazon ECR.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Sửa lỗi và thiết lập ECR <br>&emsp; + Fix lỗi `NullPointerException` tại `NotificationServiceTest.java` bằng cách cấu hình lại kết nối Database và mock data. <br>&emsp; + Khởi tạo 2 Repositories Private trên ECR (`minisocial-backend` và `minisocial-frontend`). | 04/05/2026 | 05/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Cấu hình Frontend và Jenkinsfile <br>&emsp; + Áp dụng Multi-stage build và viết thêm file `nginx.conf` cho Frontend để xử lý React Router SPA và Reverse Proxy tránh lỗi CORS. <br>&emsp; + Khởi tạo file Jenkinsfile khai báo biến môi trường AWS, cấu hình bước Checkout, Build Docker, Login ECR và Push Image. | 06/05/2026 | 07/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Tối ưu Pipeline, Deploy tự động và Họp nhóm <br>&emsp; + Xử lý lỗi treo Pipeline bằng cách xóa lệnh `npm ci` ngoài Host, chuyển vào Stage 1 của Docker (Alpine Linux) để tránh nghẽn I/O. <br>&emsp; + Tạo Job Pipeline mới trên Jenkins, trỏ tới kho GitHub và thực thi tự động. <br>&emsp; + Tham gia họp nhóm Offline để tổng kết và trình chiếu kết quả. | 08/05/2026 | 10/05/2026 | Báo cáo nội bộ |

### Kết quả đạt được tuần 3:
* Mã nguồn Backend đã load thành công Application Context và vượt qua toàn bộ 186/186 bài Unit Test.
* Hệ thống CI đã chạy tự động thành công 100%, tốc độ build tăng đáng kể và không còn bị treo.
* Các Image được đóng gói và đẩy tự động thành công lên AWS ECR với dung lượng tối ưu (Backend: 144.02 MB, Frontend siêu nhẹ: 26.33 MB).

### Minh chứng thực hiện:

#### 1. Bảng theo dõi tiến độ công việc Tuần 3
Ghi nhận hoàn thành (DONE) nhiệm vụ đóng gói mã nguồn và đẩy Image lên kho Amazon ECR, kèm theo lịch họp nhóm Offline vào ngày 10/5.
![Bảng tiến độ tuần 3](/images/Tuan3-5.png)

![Lên văn phòng AWS](/images/Tuan3-7.png)

#### 2. Kịch bản triển khai (Infrastructure as Code)
Các cấu hình mã nguồn cho Dockerfile, Nginx và Jenkinsfile đã được thiết lập và tinh chỉnh tối ưu để phục vụ luồng CI/CD.
![Cấu hình Dockerfile](/images/Tuan3.png)

![Cấu hình Nginx phần 1](/images/Tuan3-1.png)

![Cấu hình Nginx phần 2](/images/Tuan3-2.png)

![Cấu hình Jenkinsfile phần 1](/images/Tuan3-3.png)

![Cấu hình Jenkinsfile phần 2](/images/Tuan3-4.png)