---
title: "Worklog tuần 5"
date: 2026-05-24
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:
* Phác họa trực quan toàn bộ hệ thống hạ tầng dự án "Mini Social Network" lên sơ đồ kiến trúc (AWS Architecture Diagram).
* Thể hiện rõ ràng các lớp ranh giới bảo mật mạng (Network Layer, Subnetting Layer) và đường đi của các luồng dữ liệu (Traffic Flow).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Thiết kế Sơ đồ Kiến trúc Hệ thống <br>&emsp; + Sử dụng công cụ Draw.io với bộ AWS Architecture Icons chuẩn. <br>&emsp; + Phân hoạch 4 lớp rõ ràng: Mạng (VPC), Chia mạng con (Public/Private Subnet) và Lớp lưu trữ ngoài. | 18/05/2026 | 19/05/2026 | [AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |
| 4 | - Quy hoạch Luồng dữ liệu (Traffic Flow) <br>&emsp; + Sử dụng mũi tên màu để mô phỏng luồng truy cập: User -> Internet -> WAF -> ALB -> Fargate -> RDS/S3. <br>&emsp; + Thiết kế Bảng chú giải chi tiết cho từng loại mũi tên. | 20/05/2026 | 21/05/2026 |  [AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |
| 6 | - Xuất bản và Phân tích Kiến trúc <br>&emsp; + Xuất file gốc (.drawio) và file ảnh nét cao (PNG/PDF) viền trong suốt. <br>&emsp; + Hỗ trợ nhóm viết tài liệu giải mã kiến trúc 3-Tier. | 22/05/2026 | 24/05/2026 | [AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |

### Kết quả đạt được tuần 5:
* Hoàn thành 100% bản vẽ sơ đồ kiến trúc mô phỏng chính xác hiện trạng hạ tầng của dự án "Mini Social Network".
* Cung cấp đầy đủ file thiết kế gốc và hình ảnh độ phân giải cao kèm bảng chú thích luồng giao thông mạng.
* Hệ thống hóa thành công lý thuyết bảo mật đa lớp (Defense-in-Depth) vào bản vẽ thực tế.

### Minh chứng thực hiện:

#### 1. Sơ đồ Kiến trúc Hệ thống Mạng xã hội (Mini Social Network)
Bản vẽ phác họa chi tiết mô hình 3-Tier trên AWS, phân tách rõ ràng các luồng Frontend, Backend, Media và CI/CD.
![Sơ đồ Kiến trúc Hệ thống vẽ trên Draw.io](/images/Tuan5.png)
2. Gửi Giải mã kiến trúc lên nhóm zalo để mọi người cùng đọc và góp ý.
![Hình ảnh Worklog Tuần 5 ](/images/Tuan5-1.png) 