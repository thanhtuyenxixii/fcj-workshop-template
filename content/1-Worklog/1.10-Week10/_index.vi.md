---
title: "Tuần 10: Tích hợp Hệ thống AI End-to-End"
date: 2026-08-03
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

## 03/08/2026 - 09/08/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Kết nối API Gateway, AWS Lambda và SageMaker Endpoint để tạo thành tuyến API đánh giá rủi ro AI hoàn chỉnh (End-to-End).

## Bối cảnh

Tuần 10 tập trung ghép nối tất cả các mô-đun độc lập đã xây dựng từ các tuần trước thành một hệ thống đồng nhất: `Client -> API Gateway -> Lambda -> SageMaker Endpoint -> S3/CloudWatch`.

## Trọng tâm học tập AWS

- **Lambda Boto3 SageMaker Runtime:** Dùng SDK `boto3` gọi hàm `invoke_endpoint()` trong Lambda.
- **Biến đổi Dữ liệu (Data Transformation):** Nhận JSON từ Client, trích xuất đặc trưng, gọi SageMaker và phân loại cấp độ rủi ro (`LOW`, `MEDIUM`, `HIGH`).
- **Phân quyền IAM:** Bổ sung quyền `sagemaker:InvokeEndpoint` cho IAM Role của Lambda.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 03/08/2026 | Cập nhật mã nguồn Lambda tích hợp thư viện `boto3` SageMaker Runtime. |
| 04/08/2026 | Bổ sung quyền `sagemaker:InvokeEndpoint` vào IAM Execution Role của Lambda. |
| 05/08/2026 | Lập trình logic phân loại mức độ rủi ro (`LOW`/`MED`/`HIGH`) dựa trên điểm số trả về. |
| 06/08/2026 | Đấu nối API Gateway `POST /eval-risk` với hàm Lambda cập nhật. |
| 07/08/2026 | Tiến hành kiểm thử End-to-End toàn hệ thống bằng Postman. |
| 08/08/2026 - 09/08/2026 | Kiểm tra log lưu trữ tại S3 và vết thực thi trên CloudWatch. |

## Hoạt động kỹ thuật

- Ghép nối thành công API Gateway, Lambda và SageMaker Endpoint.
- Nhận log AI Agent thời gian thực và trả về kết quả phân tích rủi ro dạng JSON chuẩn hóa.

## Kết quả đạt được (Deliverables)

- **Tuyến dịch vụ AI Risk Scoring End-to-End hoạt động hoàn hảo.**
- **Mô-đun Lambda cầu nối tới SageMaker vận hành ổn định.**
- **Bộ test Postman tích hợp thành công 100%.**

## Thách thức & Giải pháp

**Thách thức:** Độ trễ (Latency) tăng cao do hiện tượng Cold Start của Lambda khi gọi SageMaker.

**Giải pháp:** Tăng dung lượng RAM cho Lambda lên 1024MB và khởi tạo kết nối Boto3 Client bên ngoài hàm Handler.

## Đóng góp cho Dự án

Hoàn thiện sản phẩm MVP hoàn chỉnh, cho phép ứng dụng bên ngoài chỉ cần gọi 1 API duy nhất để kiểm tra mức độ an toàn của AI Agent.


## Tài liệu tham khảo

- [Invoke SageMaker Endpoints using AWS Lambda](https://aws.amazon.com/blogs/machine-learning/call-an-amazon-sagemaker-model-endpoint-from-an-aws-lambda-function/)
- [AWS SDK for Python (Boto3) SageMaker Runtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.11-week11/)
