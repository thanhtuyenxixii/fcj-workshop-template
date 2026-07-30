---
title: "Tuần 11: Giám sát CloudWatch & Quản lý Chi phí"
date: 2026-08-10
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

## 10/08/2026 - 16/08/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Xây dựng hệ thống giám sát bằng Amazon CloudWatch, cảnh báo sự cố tự động, rà soát bảo mật và tối ưu hóa chi phí vận hành Cloud.

## Bối cảnh

Khi hệ thống đã chạy End-to-End, Tuần 11 tập trung chuẩn bị cho tiêu chuẩn vận hành thực tế: Giám sát hiệu năng, phát hiện lỗi tự động và kiểm soát ngân sách.

## Trọng tâm học tập AWS

- **Amazon CloudWatch Dashboards & Alarms:** Bắt các chỉ số (Độ trễ API, tỷ lệ lỗi Lambda, số lượt gọi SageMaker Endpoint).
- **Chiến lược Tối ưu Chi phí:** Phân tích AWS Cost Explorer, thiết lập S3 Lifecycle và điều chỉnh kích thước Instance.
- **Rà soát Bảo mật (Security Audit):** Kiểm tra lại phân quyền IAM, đảm bảo S3 không bị lộ Public.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 10/08/2026 | Cấu hình CloudWatch Log Groups cho toàn bộ dịch vụ. |
| 11/08/2026 | Tạo CloudWatch Alarms cho tỷ lệ lỗi Lambda (>5%) và độ trễ API (>2 giây). |
| 12/08/2026 | Xây dựng CloudWatch Dashboard tập trung theo dõi toàn hệ thống theo thời gian thực. |
| 13/08/2026 | Phân tích chi phí bằng AWS Cost Explorer. |
| 14/08/2026 | Lập lịch tự động xóa/tạo lại SageMaker Endpoint ngoài giờ làm việc để tiết kiệm tiền. |
| 15/08/2026 - 16/08/2026 | Rà soát tổng thể bảo mật IAM và cấu hình S3 Block Public Access. |

## Hoạt động kỹ thuật

- Tạo CloudWatch Dashboard hiển thị lưu lượng, độ trễ và tỷ lệ lỗi.
- Cấu hình gửi thông báo Email qua Amazon SNS khi có Cảnh báo (Alarm).

## Kết quả đạt được (Deliverables)

- **CloudWatch Dashboard vận hành trực quan.**
- **Cảnh báo CloudWatch Alarms & Thông báo SNS Email sẵn sàng.**
- **Báo cáo tối ưu chi phí AWS Cost Explorer.**

## Thách thức & Giải pháp

**Thách thức:** SageMaker Endpoint ngốn nhiều chi phí nhất khi để chạy không tải liên tục.

**Giải pháp:** Dùng EventBridge kết hợp Lambda tự động tắt Endpoint vào buổi tối và bật lại vào sáng hôm sau.

## Đóng góp cho Dự án

Đảm bảo hệ thống tuân thủ các trụ cột về Vận hành xuất sắc, Bảo mật và Tối ưu chi phí theo tiêu chuẩn AWS Well-Architected Framework.


## Tài liệu tham khảo

- [Amazon CloudWatch User Guide](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html)
- [AWS Cost Optimization Pillar](https://docs.aws.amazon.com/wellarchitected/latest/cost-optimization-pillar/welcome.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.12-week12/)
