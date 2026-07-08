---
title: "Worklog tuần 10"
date: 2026-06-28
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:
* Đóng băng mã nguồn (Code Freeze) và tiến hành rà soát tổng thể hạ tầng mạng trước khi đưa lên môi trường thật.
* Đánh giá bảo mật và hiệu chỉnh lại toàn bộ file cấu hình hạ tầng (YAML).
* Hoàn thiện bản vẽ Sơ đồ kiến trúc (Architecture Diagram) phiên bản cuối cùng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Rà soát mã nguồn hạ tầng (IaC) <br>&emsp; + Phân tích và kiểm tra toàn bộ file YAML cấu hình mạng (VPC, Subnet, Route Table) do team cung cấp. <br>&emsp; + Tổng hợp các điểm chưa hợp lý, đối chiếu cấu trúc và lập báo cáo đánh giá, đề xuất chỉnh sửa file YAML. | 22/06/2026 | 23/06/2026 | |
| 4 | - Hoàn thiện Sơ đồ Kiến trúc <br>&emsp; + Cập nhật và tinh chỉnh sơ đồ kiến trúc (Minisocial Architect) phiên bản chốt hạ dựa trên hạ tầng thực tế sau khi Rebuild. <br>&emsp; + Bổ sung đầy đủ các luồng kết nối và dịch vụ mới (NAT Gateway, S3 VPC Endpoint) vào bản vẽ. | 24/06/2026 | 25/06/2026 | 	[AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |
| 6 | - Đánh giá bảo mật luồng mạng đám mây (Network Security Review) <br>&emsp; + Rà soát lại toàn bộ Inbound/Outbound rules của Security Group và Network ACL trên VPC để đảm bảo không bị hở các port không cần thiết ở lớp Public Subnet. <br>&emsp; + Kiểm tra luồng kết nối mạng nội bộ giữa cụm Compute (Amazon ECS Fargate) và Database (Amazon RDS) để đảm bảo tính an toàn dữ liệu. | 26/06/2026 | 26/06/2026 |  |

### Kết quả đạt được tuần 10:
* Hoàn thành báo cáo đánh giá và chỉnh sửa thành công các lỗi cấu hình trong file YAML.
* Xuất bản thành công Sơ đồ Kiến trúc (Architecture Diagram) phiên bản hoàn chỉnh nhất, phản ánh chính xác 100% hạ tầng mạng hiện tại.
* Hoàn tất rà soát bảo mật hạ tầng mạng, cập nhật trạng thái công việc thành hoàn tất (DONE) đúng thời hạn (Deadline 23:59 ngày 23/06).

### Minh chứng thực hiện:

#### 1. Hoàn thành Task phân công Tuần 10
Đã hoàn tất các hạng mục "Phân tích và kiểm tra toàn bộ file YAML" và "Hoàn thiện sơ đồ Architect". Trạng thái công việc trên hệ thống theo dõi của nhóm đã chuyển sang xanh (DONE). 

*(Ghi chú: Nhóm đã chủ động tổ chức họp trực tiếp bên ngoài (Cafe Sync-up) vào ngày 26/06 để chốt hạ các lỗi trong file YAML và thống nhất bản vẽ kiến trúc cuối cùng trước khi đưa lên môi trường thật. Bảng trạng thái cập nhật DONE dưới đây là minh chứng cho kết quả của buổi làm việc)*.
![Bảng theo dõi tiến độ công việc Tuần 10](/images/Tuan10-1.png)

![Đã gửi lên group zalo](/images/Tuan10.png)

#### 2. Sơ đồ Kiến trúc Hệ thống (Bản cập nhật cuối cùng)
Bản vẽ kiến trúc mạng tổng thể đã được tinh chỉnh, bổ sung các thành phần mới sau quá trình Rebuild và Security Audit. Đây là thành quả trực tiếp từ quá trình rà soát hạ tầng, sẵn sàng làm tài liệu chính thức cho buổi bảo vệ dự án.
![Sơ đồ kiến trúc đã chỉnh sửa chi tiết](/images/SoDoKienTrucDaChinhSua.drawio.png)