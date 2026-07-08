---
title: "Worklog tuần 6"
date: 2026-05-31
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:
* Chuyển đổi thiết kế hạ tầng mạng thành mã (Infrastructure as Code - IaC) thông qua AWS CloudFormation.
* Tự động hóa quá trình khởi tạo và đồng bộ các tài nguyên cốt lõi của mạng lưới để chuẩn bị cho quá trình đưa ứng dụng lên mây (Pre-flight Check).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Viết kịch bản IaC cơ bản <br>&emsp; + Viết script `infrastructure.yaml` định nghĩa tài nguyên mạng ảo VPC (10.0.0.0/16) và Internet Gateway. <br>&emsp; + Khai báo cấu hình 2 Public Subnets và 2 Private Subnets trải đều ở các Availability Zones (AZ) khác nhau. | 25/05/2026 | 26/05/2026 | [AWS CloudFormationn](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks?filteringText=&filteringStatus=active&viewNested=true) |
| 4 | - Cấu hình định tuyến và bảo mật <br>&emsp; + Khởi tạo Route Table để định tuyến cho mạng Public Subnet thông ra Internet. <br>&emsp; + Viết thông số khởi tạo các Security Groups tách biệt: ALB (mở Port 80) và Backend (mở Port 8080). | 27/05/2026 | 28/05/2026 | [AWS CloudFormationn](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks?filteringText=&filteringStatus=active&viewNested=true) |
| 6 | - Triển khai tự động tài nguyên <br>&emsp; + Bổ sung khối tài nguyên Application Load Balancer (ALB) vào file YAML. <br>&emsp; + Tải file `infrastructure.yaml` lên AWS CloudFormation, đặt tên stack là `MiniSocial-Tuan6-Infra` và thực thi lệnh khởi tạo. | 29/05/2026 | 31/05/2026 | Tài Liệu Nhóm |

### Kết quả đạt được tuần 6:
* Hoàn tất kịch bản mã IaC chuẩn xác, liên kết thành công Load Balancer, các lớp Subnets và Security Group.
* Quá trình triển khai stack CloudFormation thành công 100% với trạng thái `CREATE_COMPLETE`.
* Giải mã và nắm vững cơ chế đồng bộ tài nguyên (Consistency check) của hệ thống AWS toàn cầu trong quá trình khởi tạo.

### Minh chứng thực hiện:

#### 1. Triển khai hạ tầng tự động qua CloudFormation
Đã thực hiện upload template `infrastructure.yaml` và cấu hình thành công Stack mang tên `MiniSocial-Tuan6-Infra` trên AWS Console.
Hệ thống đã triển khai hoàn tất và trả về trạng thái **CREATE_COMPLETE**.
*(Ghi chú kỹ thuật: Các đoạn màu nâu trên biểu đồ hiển thị trạng thái "Consistency check" - quá trình AWS tạm dừng vài giây để rà soát và đồng bộ dữ liệu trên hệ thống toàn cầu. Điểm kết thúc chuyển sang màu xanh lá chứng tỏ tài nguyên đã vượt qua bài kiểm tra và được tạo thành công 100%.)*

Kết quả sẽ ra: CREATE_COMPLETE: 
![Hình ảnh Worklog Tuần 6 ](/images/Tuan6.png) 

![Hình ảnh Worklog Tuần 6 ](/images/Tuan6-1.png)

2. Gửi Tai_Lieu_CloudFormation_MiniSocial lên nhóm zalo.

![Hình ảnh Worklog Tuần 6 ](/images/Tuan6-2.png) 