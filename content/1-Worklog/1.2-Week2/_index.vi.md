---
title: "Worklog tuần 2"
date: 2026-04-27
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:
* Nghiên cứu dịch vụ lưu trữ an toàn Amazon ECR và điện toán không máy chủ (Serverless Compute) AWS Fargate.
* Thực hiện đóng gói, đẩy Docker Image lên ECR và khởi chạy ứng dụng độc lập trên AWS Console nhằm khắc phục lỗi chết máy chủ (Downtime).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Thao tác đóng gói tại Local <br>&emsp; + Sử dụng AWS CLI để lấy Token và xác thực quyền truy cập vào AWS ECR. <br>&emsp; + Dùng lệnh `docker build` với cờ `--platform linux/amd64` để tạo Image, giúp ngăn chặn lỗi kiến trúc CPU. | 27/04/2026 | 28/04/2026 | [Tài liệu First Cloud AI Journey](https://cloudjourney.awsstudygroup.com/) |
| 4 | - Push Image lên kho lưu trữ ECR <br>&emsp; + Gắn thẻ (Tag) Image khớp với đường dẫn kho lưu trữ ECR. <br>&emsp; + Dùng lệnh `docker push` đẩy Image Backend an toàn lên hệ thống nội bộ của AWS. | 29/04/2026 | 30/04/2026 | [Tài liệu First Cloud AI Journey](https://cloudjourney.awsstudygroup.com/) |
| 6 | - Khởi chạy trên Amazon ECS <br>&emsp; + Truy cập Amazon ECS tạo Cluster (môi trường mạng logic). <br>&emsp; + Tạo Task Definition với thông số 1 vCPU và 2 GiB RAM, đồng thời cấp quyền `ecsTaskExecutionRole`. <br>&emsp; + Tạo Service chạy ứng dụng và thực hiện tối ưu chi phí bằng cách chỉnh Desired tasks về 0 sau khi test. | 01/05/2026 | 03/05/2026 | [Tài liệu First Cloud AI Journey](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được tuần 2:
* Nắm bắt mô hình Serverless AWS Fargate, qua đó cung cấp môi trường độc lập để gánh vác khối lượng logic phức tạp (giao tiếp API, bảo mật JWT, Socket) mà không cần phụ thuộc vào Firebase hay cơ sở dữ liệu cục bộ SQLite.
* Đẩy thành công Docker Image lên kho lưu trữ Amazon ECR (thay thế cho Docker Hub).
* Hoàn tất cấu hình ECS Service trong chế độ mạng `awsvpc`, thiết lập đúng quyền hạn IAM và quy trình kiểm soát chi phí do AWS Fargate không thuộc Free Tier.

### Minh chứng thực hiện:

#### 1. Bảng theo dõi tiến độ công việc Tuần 2
Ghi nhận hoàn thành (DONE) nhiệm vụ nghiên cứu các dịch vụ ECR & Fargate.
*(Lưu ý: Trong tuần lễ này nhóm có lịch nghỉ (OFF meeting), tuy nhiên các thành viên vẫn chủ động hoàn thành các task cá nhân đúng tiến độ)*.
![Bảng tiến độ tuần 2](/images/worklogtuan2.png)

#### 2. Nộp tài liệu nghiên cứu
Tài liệu phân tích chi tiết về quy trình triển khai, cấu hình dự kiến và ứng dụng thực tiễn của kiến trúc ECR/Fargate đã được soạn thảo thành file Word (`tuan2.docx`) và gửi trực tiếp lên group Zalo chung để nhóm cùng nắm thông tin.
![Minh chứng nộp file báo cáo Tuần 2](/images/worklogtuan2-1.png)