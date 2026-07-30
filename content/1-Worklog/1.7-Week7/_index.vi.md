---
title: "Tuần 7: Cân bằng tải ALB & Auto Scaling"
date: 2026-07-13
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

## 13/07/2026 - 19/07/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Cấu hình Application Load Balancer (ALB) và chính sách Auto Scaling đảm bảo tính sẵn sàng cao cho dịch vụ đánh giá rủi ro.

## Bối cảnh

Tuần 7 tập trung vào việc phân phối lưu lượng truy cập và tự động mở rộng tài nguyên khi số lượng yêu cầu đánh giá tăng đột biến.

## Trọng tâm học tập AWS

- **Application Load Balancer (ALB):** Listener Rules, Target Groups và Health Checks.
- **Target Tracking Scaling:** Tự động tăng/giảm số lượng Task dựa trên mức sử dụng CPU hoặc số lượng Request.
- **High Availability:** Kiểm thử khả năng chịu lỗi khi một AZ gặp sự cố.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 13/07/2026 | Khởi tạo Application Load Balancer trên các Public Subnets. |
| 14/07/2026 | Cấu hình Target Group trỏ đến ECS Fargate Tasks kèm Health Check path `/health`. |
| 15/07/2026 | Thiết lập chính sách Target Tracking Auto Scaling (ngưỡng CPU 70%). |
| 16/07/2026 | Gửi tải giả lập để kiểm thử khả năng tự động Scale-out từ 1 lên 4 Tasks. |
| 17/07/2026 | Tự động Scale-in giảm số Task khi hết tải. |
| 18/07/2026 - 19/07/2026 | Thu thập thông số CloudWatch và cập nhật tài liệu. |

## Hoạt động kỹ thuật

- Dùng ALB phân phối lưu lượng HTTP vào Target Group của ECS.
- Thử nghiệm gửi lượng lớn Request để xác nhận hệ thống tự mở rộng tài nguyên.

## Kết quả đạt được (Deliverables)

- **Application Load Balancer hoạt động kèm Health Checks.**
- **Chính sách Auto Scaling mở rộng tự động thành công.**
- **Báo cáo kiểm thử tải trọng và độ sẵn sàng cao.**

## Thách thức & Giải pháp

**Thách thức:** Target Group báo trạng thái Unhealthy khi mới tạo.

**Giải pháp:** Sửa lại URL Health Check (`/health`) và mở đúng Port Container trong Security Group.

## Đóng góp cho Dự án

Đảm bảo dịch vụ AI Agent không bị gián đoạn hay quá tải khi nhận nhiều yêu cầu đánh giá cùng lúc.


## Tài liệu tham khảo

- [Elastic Load Balancing Guide](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html)
- [Target Tracking Scaling Policies](https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scaling-target-tracking.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.8-week8/)
