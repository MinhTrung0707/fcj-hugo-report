---
title: "Worklog tuần 12"
date: 2026-07-07
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu tuần 12:
* Phân tích, rà soát và chốt bản Final của sơ đồ kiến trúc dự án (Minisocial Architect) dựa trên bài toán giới hạn ngân sách.
* Hoàn thiện 100% nội dung trên Hugo Server & Báo cáo thực tập, thực hiện kiểm tra chéo (Cross-check) cùng đội ngũ.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Phân tích, rà soát sơ đồ kiến trúc Minisocial Architect <br>&emsp; + Đánh giá hiện trạng hạ tầng mạng (VPC, Subnets, Traffic Optimization). <br>&emsp; + Nhận diện các điểm giới hạn của hạ tầng (chỉ sử dụng 1 NAT Gateway ở AZ A và Single-AZ cho RDS). Đánh giá rủi ro và quyết định giữ nguyên cấu trúc này để đảm bảo tối ưu chi phí cho quy mô hiện tại của dự án. | 06/07/2026 | 06/07/2026 | Sơ đồ hệ thống hiện hành |
| 3 | - Chốt sơ đồ Final và nộp báo cáo <br>&emsp; + Tinh chỉnh sơ đồ: Làm gọn layout, căn chỉnh lại các đường line kết nối để làm rõ luồng giao tiếp Logic và Physical (đặc biệt là luồng Outbound Traffic qua NAT Gateway). <br>&emsp; + Hoàn thiện Hugo Server & Báo cáo thực tập, tiến hành kiểm tra chéo (Cross-check) và nộp trước hạn (Deadline 23:59 t3 07/07). | 07/07/2026 | 07/07/2026 | Sơ đồ Draw.io / Nền tảng nội bộ |

### Kết quả đạt được tuần 12:
* Hoàn thành rà soát chuyên sâu và chốt Sơ đồ Kiến trúc Minisocial Architect phiên bản Final (bảo toàn cấu trúc hạ tầng hiện hành để tối ưu ngân sách, hoàn thiện mặt trình bày trực quan).
* Thực hiện nghiêm túc việc kiểm tra chéo (Cross-check) tài liệu theo quy định của nhóm, đảm bảo không có sai sót.
* Hoàn thiện toàn bộ nội dung và nộp thành công Hugo Server cùng Báo cáo thực tập đúng thời hạn (hoàn tất trước 23:59 Thứ Ba, ngày 07/07/2026).

### Hoạt động khác / Minh chứng thực hiện:

#### 1. Bảng phân công nhiệm vụ Tuần 12
Ghi nhận phân công công việc của giai đoạn Graceful Shutdown & Documentation. Các task "Phân tích, rà soát, chỉnh sửa bản final của sơ đồ kiến trúc Minisocial Architect" và hoàn thiện báo cáo đã được xử lý đúng hạn. 

![Bảng theo dõi tiến độ công việc Tuần 12](/images/Tuan12.png)
*(Ghi chú hoạt động ngoại khóa: Nhóm đã linh động tổ chức họp nghiệm thu trực tiếp tại quán cà phê vào Thứ Tư, ngày 08/07 nhằm thống nhất bàn giao và chốt sổ dự án)*.
![Bảng theo dõi tiến độ công việc Tuần 12](/images/Tuan12-1.png)

#### 2. Sơ đồ Kiến trúc (Final Version)
Bản vẽ cuối cùng đã được tinh chỉnh để trình bày trực quan nhất hệ sinh thái của dự án. Sơ đồ tập trung làm rõ các luồng kết nối mạng cốt lõi (VPC Gateway Endpoint cho S3, Outbound Traffic qua NAT Gateway) và quyết định giữ nguyên thiết kế Single-AZ đối với Database để bám sát bài toán tối ưu chi phí của nhóm.

![Bảng theo dõi tiến độ công việc Tuần 12](/images/SoDoKienTrucDaChinhSua.drawio.png)