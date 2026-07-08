---
title: "EVENT 2"
date: 2026-06-20
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---
# Bài thu hoạch: "Cloud Architect"

![Ảnh check-in tại sự kiện](/images/Evt_2.png)


**Vai trò tham dự:** Thí sinh thi đấu (Thành viên nhóm PrimeOps)

### Mục Đích Của Sự Kiện
- Tạo ra một môi trường giả lập áp lực cao, đòi hỏi người tham gia phải vận dụng tư duy của một Kiến trúc sư Hệ thống để giải quyết các bài toán hạ tầng mạng thực tế trên AWS.
- Đánh giá khả năng chuyển hóa kiến thức hàn lâm thành phản xạ thực chiến: Từ việc hiểu dịch vụ cơ bản (Cloud Practitioner) đến thiết kế luồng dữ liệu chuẩn xác (SAA) và tối ưu hóa kiến trúc đa vùng cấp cao (SAP).
- Thử thách năng lực xử lý sự cố, bảo mật hệ thống và tối ưu chi phí hạ tầng (Cost Optimization) trong các giới hạn khắt khe của doanh nghiệp.
- Mở rộng góc nhìn từ việc cấu hình các tài nguyên đơn lẻ sang việc quy hoạch một Sơ đồ Kiến trúc Tổng thể (Architecture Diagram) hoàn chỉnh.

---

### Nội Dung Nổi Bật: Nâng Cấp Tư Duy Hạ Tầng Mạng

Cuộc thi được thiết kế với độ khó tăng dần, mô phỏng đúng quá trình phát triển quy mô của một hệ thống từ lúc khởi tạo đến khi trở thành dự án doanh nghiệp lớn.

#### Vòng Loại: Định Hình Nền Tảng (10 câu hỏi)
- **Cấu trúc:** 7 câu Cloud Practitioner (CP), 2 câu SAA, 1 câu SAP.
- **Tiêu điểm (Infrastructure View):** Đây là vòng "thử tải" nền tảng. Thay vì chỉ học thuộc khái niệm, việc phân định rõ ràng vai trò của từng khối dịch vụ cốt lõi (Compute, Storage, Database) là cực kỳ quan trọng. Sự xuất hiện của 1 câu SAP (50 điểm) ngay đầu hiệp đóng vai trò như một "nút thắt cổ chai", đòi hỏi khả năng đánh giá rủi ro nhanh chóng để quyết định đánh nhanh rút gọn hay đi sâu phân tích kiến trúc.

#### Vòng Bán Kết: Bài Toán Định Tuyến & Mạng Ảo (10 câu hỏi)
- **Cấu trúc:** 5 câu CP, 3 câu SAA, 2 câu SAP.
- **Tiêu điểm (Networking View):** Trọng tâm kiến thức bắt đầu chuyển dịch mạnh sang quy hoạch mạng lưới. Các câu hỏi đòi hỏi sự nhạy bén trong việc bóc tách các lớp mạng ảo (VPC), cấu hình Subnetting, bảng định tuyến (Route Table) và các quy tắc bảo mật đường truyền. Hai bài toán SAP ở vòng này thực sự là "bài test" năng lực nhìn nhận luồng giao thông dữ liệu (Traffic Flow) xem có bị tắc nghẽn ở đâu không.

#### Vòng Chung Kết: Thiết Kế Chuẩn Enterprise & Bảo Mật Đa Lớp (10 câu hỏi)
- **Cấu trúc:** 3 câu CP, 4 câu SAA, 3 câu SAP.
- **Tiêu điểm (Security & Architect View):** Yêu cầu được đẩy lên mức cao nhất. Không chỉ dừng ở việc "hệ thống có chạy được không", mà phải trả lời được: Khả năng chịu lỗi đa vùng (High Availability) ra sao? Cơ chế phòng thủ DDoS thế nào? Các câu hỏi SAP (150 điểm) yêu cầu một cái nhìn bao quát, kết hợp nhuần nhuyễn giữa bộ cân bằng tải, tự động mở rộng (Auto Scaling) và tường lửa WAF.

#### Chiến Thuật Vận Hành
Mỗi đội được cung cấp 2 kỹ năng để linh hoạt kiểm soát rủi ro:
1. **Ngôi sao hy vọng (High Risk - High Reward):** Trả lời đúng nhân đôi điểm, sai trừ gấp đôi. Thích hợp dùng khi gặp trúng "tủ" kiến thức về mạng hoặc bảo mật chuyên sâu.
2. **Giảm thiểu rủi ro (Safe Play):** Trả lời đúng cộng 50% điểm, sai không trừ. Một phương án cực kỳ an toàn để dò mìn ở những câu hỏi vượt quá tầm thiết kế hiện tại.

---

### Những Gì Học Được

#### Tư Duy Hệ Thống & Bảo Mật (SysOps/Architect Mindset)
- **Phân hoạch kiến trúc rõ ràng:** Cuộc thi giúp đả thông tư duy từ việc chạy một máy chủ đơn lẻ sang việc thiết kế cả một cụm Cluster hoạt động trơn tru. Nhận ra rằng ranh giới giữa một hệ thống bình thường và một hệ thống cấp độ SAP chính là khả năng tự động hóa và chịu lỗi.
- **Bảo mật đa lớp (Defense-in-Depth):** Khắc sâu tầm quan trọng của việc thắt chặt an ninh từ những lớp thấp nhất như Security Group, Network ACL cho đến các chính sách phân quyền IAM khắt khe (Least Privilege).

#### Kỹ Năng Phân Tích Thực Chiến
- **Dịch ngược đề bài thành Sơ đồ:** Khi đối diện với các đoạn mô tả yêu cầu dài hàng chục dòng của đề SAP, kỹ năng quan trọng nhất học được là khả năng "vẽ lại" sơ đồ kiến trúc ngay trong đầu. Việc xác định ngay đâu là Frontend, Backend, Database và luồng đi của mạng giúp bóc tách các phương án gây nhiễu rất hiệu quả.
- **Đánh giá Trade-off (Đánh đổi):** Học được cách cân nhắc giữa Chi phí (Cost) và Hiệu năng (Performance). Một giải pháp công nghệ hoàn hảo nhưng đắt đỏ chưa chắc đã là đáp án đúng nếu đề bài nhấn mạnh vào việc tối ưu ngân sách.

---

### Trải Nghiệm Trong Event

Tham gia với tư cách là **Thí sinh thi đấu thuộc nhóm PrimeOps**, sự kiện "Cloud Architect" đối với tôi không đơn thuần là một cuộc đua điểm số, mà là một đợt *Security Audit* và *Architecture Review* thu nhỏ cực kỳ căng thẳng. 

#### Bóc tách giới hạn bản thân
Khi thời gian đếm ngược ở vòng Chung kết với 3 câu hỏi cấp độ chuyên gia liên tiếp, áp lực tạo ra giống hệt như lúc phải rà soát hàng ngàn dòng code hạ tầng (YAML) để tìm ra điểm nghẽn mạng. Việc cùng đồng đội trong PrimeOps phải đưa ra quyết định kiến trúc trong tích tắc thực sự rèn luyện cái "đầu lạnh" và khả năng phối hợp nhóm dưới áp lực cao.

#### Mảnh ghép thực tiễn
Trải nghiệm này chứng minh rõ ràng: Lý thuyết là nền tảng, nhưng khả năng tự tay vẽ nên một sơ đồ kiến trúc chi tiết, thấu hiểu tường tận từng kết nối (Endpoints, Load Balancers) mới là chìa khóa để làm chủ cuộc chơi đám mây. Những câu hỏi hóc búa tại sự kiện càng làm tăng thêm động lực để tiếp tục đào sâu vào các bài Lab cấu hình mạng phức tạp, tinh chỉnh hạ tầng container và tối ưu hóa hệ thống trong tương lai.

#### Một số hình ảnh khi tham gia sự kiện

![Ảnh check-in tại sự kiện](/images/event2-1.png)

![Ảnh check-in tại sự kiện](/images/event2.png)

![Ảnh check-in tại sự kiện](/images/AnhEvent2-2.png)