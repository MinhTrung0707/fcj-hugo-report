---
title: "Worklog tuần 7"
date: 2026-06-07
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7:
* Khái quát hóa và hoàn thiện sơ đồ kiến trúc hệ thống chuẩn 3-Tier Architecture trên nền tảng AWS.
* Trực quan hóa các luồng giao thông mạng (Data Plane & Control Plane) phục vụ cho đợt triển khai "The Big Move".
* Soạn thảo chi tiết kịch bản bài thuyết trình bảo vệ kiến trúc dự án.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 2 | - Hoàn thiện Sơ đồ Kiến trúc <br>&emsp; + Thiết kế sơ đồ bao gồm ranh giới VPC, Public/Private Subnets, ALB, ECS Fargate, RDS và NAT Gateway. | 01/06/2026 | 03/06/2026 | [AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |
| 5 | - Phân tích Luồng Dữ liệu (Traffic Flows) <br>&emsp; + Bóc tách luồng User Access (1-7) và luồng CI/CD & Monitoring (8-10, A-B). | 04/06/2026 | 05/06/2026 | [AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |
| 7 | - Viết kịch bản Thuyết trình <br>&emsp; + Đóng gói toàn bộ tài liệu thành bài viết thảo luận chuyên sâu về kiến trúc Mạng xã hội quy mô nhỏ. | 06/06/2026 | 07/06/2026 |  |

### Kết quả đạt được tuần 7:
* Hoàn thiện 100% sơ đồ kiến trúc hệ thống mạng nội bộ cô lập chuẩn AWS.
* Thiết lập rõ ràng lộ trình phân phối giao diện web tĩnh qua S3 và cơ chế xử lý API nội bộ.
* Hoàn tất kịch bản thuyết trình chi tiết làm tài liệu đối chiếu cho nhóm tiến hành dựng hạ tầng thực tế bằng CloudFormation.

### Minh chứng thực hiện:

#### 1. Hoàn thiện Bản vẽ Sơ đồ Kiến trúc (Architecture Diagram)
Đã thiết kế thành công sơ đồ kiến trúc tổng thể, minh họa rõ nét mô hình 3-Tier Architecture lồng ghép trong môi trường VPC của AWS.
![Sơ đồ Kiến trúc Mạng xã hội quy mô nhỏ - AWS 3-Tier Architecture](/images/Tuan7.png)

![Hình ảnh Worklog Tuần 7 ](/images/Tuan7-1.png)