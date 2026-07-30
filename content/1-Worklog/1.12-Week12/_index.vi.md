---
title: "Tuần 12: Dọn dẹp Tài nguyên, Hoàn thiện Báo cáo & Tổng kết"
date: 2026-08-17
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

## 17/08/2026 - 23/08/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Tiến hành dọn dẹp sạch sẽ toàn bộ tài nguyên đã tạo trên AWS để tránh phát sinh chi phí, hoàn thiện website báo cáo Hugo và viết tự đánh giá/phản hồi thực tập.

## Bối cảnh

Tuần cuối cùng của hành trình 12 tuần thực tập tập trung vào việc hủy bỏ hạ tầng an toàn, tổng hợp minh chứng dự án và hoàn thiện toàn bộ tài liệu báo cáo.

## Trọng tâm học tập AWS

- **Quy trình Hủy bỏ Tài nguyên (Decommissioning):** Xóa SageMaker Endpoints, ECS Clusters, NAT Gateways, ECR Images và S3 Buckets đúng trình tự.
- **Tổng kết & Đánh giá (Retrospective):** Đánh giá các mục tiêu đã đạt được, bài học kinh nghiệm và định hướng phát triển tiếp theo.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 17/08/2026 | Xóa SageMaker Endpoints, Endpoint Configurations và Models. |
| 18/08/2026 | Hủy ECS Services, Fargate Tasks, ECR Repositories và NAT Gateways. |
| 19/08/2026 | Dọn dẹp dữ liệu S3 Buckets tạm và các CloudWatch Log Groups. |
| 20/08/2026 | Rà soát và hoàn thiện nội dung các file Markdown trên Hugo cho cả 8 phần báo cáo. |
| 21/08/2026 | Hoàn thành Phần 6 (Tự đánh giá) và Phần 7 (Phản hồi/Đánh giá từ Mentor). |
| 22/08/2026 - 23/08/2026 | Kiểm thử Build trang Hugo tĩnh và nộp báo cáo thực tập chính thức. |

## Hoạt động kỹ thuật

- Hủy bỏ toàn bộ tài nguyên có tính phí trên AWS, xác nhận số dư không phát sinh thêm qua AWS Cost Explorer.
- Build và xuất bản trang báo cáo Hugo hoàn chỉnh.

## Kết quả đạt được (Deliverables)

- **Toàn bộ Worklog 12 tuần hoàn thành chi tiết.**
- **Tài khoản AWS được dọn dẹp sạch 100%.**
- **Báo cáo thực tập & Bản tự đánh giá hoàn thành.**

## Thách thức & Giải pháp

**Thách thức:** Đảm bảo không bỏ sót các tài nguyên ẩn (Elastic IPs, EBS Snapshots) gây phát sinh chi phí ngầm.

**Giải pháp:** Sử dụng công cụ AWS Resource Groups & Tag Editor để rà soát và xóa triệt để mọi tài nguyên còn sót lại.

## Đóng góp cho Dự án

Khép lại kỳ thực tập AWS First Cloud AI Journey với một báo cáo đầy đủ, khoa học và hạ tầng tài khoản được quản lý chuyên nghiệp.


## Tài liệu tham khảo

- [AWS Deleting Resources Guide](https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html)
- [Hugo Static Site Generator Docs](https://gohugo.io/documentation/)

---

[Quay lại Worklog](/1-worklog/)
