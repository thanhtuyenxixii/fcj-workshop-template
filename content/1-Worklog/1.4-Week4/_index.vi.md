---
title: "Tuần 4: Serverless API Pipeline với Lambda & API Gateway"
date: 2026-06-22
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

## 22/06/2026 - 28/06/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Phát triển tuyến Serverless API bằng API Gateway và Lambda để tiếp nhận log hành vi từ AI Agent.

## Bối cảnh

Tuần 4 xây dựng cổng tiếp nhận dữ liệu đầu vào cho hệ thống. Mục tiêu là tạo một API HTTP nhẹ để xác thực dữ liệu JSON và ghi log vào S3.

## Trọng tâm học tập AWS

- **Phát triển AWS Lambda:** Viết bằng Python 3.11 sử dụng thư viện `boto3`.
- **Amazon API Gateway:** Cấu hình REST API, Lambda Proxy Integration, Request Validation và CORS.
- **Amazon CloudWatch Logs:** Theo dõi vết thực thi và bắt lỗi tự động.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 22/06/2026 | Định nghĩa cấu trúc dữ liệu JSON log của AI Agent. |
| 23/06/2026 | Lập trình hàm Lambda `agent-risk-ingest-fn` bằng Python. |
| 24/06/2026 | Tạo REST API trên API Gateway với Endpoint `POST /score`. |
| 25/06/2026 | Cấu hình Lambda Proxy Integration và các Response Headers CORS. |
| 26/06/2026 | Phân quyền cho Lambda ghi dữ liệu vào S3 và CloudWatch Logs. |
| 27/06/2026 - 28/06/2026 | Kiểm thử API bằng Postman và cURL. |

## Hoạt động kỹ thuật

- Kết nối API Gateway với AWS Lambda qua kết nối Proxy.
- Viết mã xác thực định dạng JSON để lọc dữ liệu rác trước khi lưu vào S3.

## Kết quả đạt được (Deliverables)

- **API tiếp nhận dữ liệu hoạt động (`POST /score`).**
- **Hàm Lambda xử lý log bằng Python đi vào hoạt động.**
- **Bộ test Postman thành công.**

## Thách thức & Giải pháp

**Thách thức:** Lỗi CORS khi gọi API Gateway từ script bên ngoài.

**Giải pháp:** Bật CORS trong API Gateway và thêm header `Access-Control-Allow-Origin` vào kết quả trả về của Lambda.

## Đóng góp cho Dự án

Xây dựng cổng giao tiếp cho phép các môi trường chạy AI Agent gửi dữ liệu về Cloud để phân tích rủi ro.

## Tài liệu tham khảo

- [AWS Lambda Developer Guide](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
- [Amazon API Gateway Guide](https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.5-week5/)
