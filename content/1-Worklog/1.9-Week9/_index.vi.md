---
title: "Tuần 9: Huấn luyện PyTorch & Triển khai SageMaker Endpoint"
date: 2026-07-27
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

## 27/07/2026 - 02/08/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Huấn luyện mô hình PyTorch Risk Scoring bằng SageMaker Training Jobs và triển khai mô hình lên SageMaker Real-Time Endpoint.

## Bối cảnh

Tuần 9 thực hiện quy trình MLOps quan trọng: Huấn luyện mô hình PyTorch trên Cloud và đóng gói thành Endpoint phục vụ suy luận thời gian thực (Inference).

## Trọng tâm học tập AWS

- **SageMaker PyTorch Estimator:** Cấu hình file huấn luyện, tham số (Hyperparameters) và Instance Type.
- **Model Artifacts:** Quản lý file trọng số mô hình lưu trên S3 (`model.tar.gz`).
- **SageMaker Endpoints:** Khởi tạo Model, Endpoint Configuration và Real-Time Endpoint.
- **SageMaker Runtime Boto3:** Gọi Endpoint bằng hàm `invoke_endpoint()`.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 27/07/2026 | Lập trình mã nguồn huấn luyện PyTorch (`train.py`) và định nghĩa mạng Neural. |
| 28/07/2026 | Chạy SageMaker Training Job với PyTorch Estimator (`ml.m5.xlarge`). |
| 29/07/2026 | Kiểm tra độ chính xác mô hình và xác nhận file trọng số được lưu trên S3. |
| 30/07/2026 | Tạo SageMaker Model và Endpoint Configuration (`ml.t2.medium`). |
| 31/07/2026 | Triển khai SageMaker Real-Time Endpoint và kiểm tra trạng thái `InService`. |
| 01/08/2026 - 02/08/2026 | Viết script Python `boto3` kiểm thử dự đoán điểm rủi ro từ Endpoint. |

## Hoạt động kỹ thuật

- Huấn luyện mô hình PyTorch bằng SageMaker Training Jobs.
- Khởi chạy Real-Time Endpoint (`ai-agent-risk-score-endpoint`).
- Kiểm thử trả về điểm rủi ro (Risk Score từ 0.0 đến 1.0).

## Kết quả đạt được (Deliverables)

- **SageMaker Training Job hoàn thành 100%.**
- **Model Artifacts được lưu trữ an toàn trên S3.**
- **SageMaker Real-Time Endpoint đạt trạng thái `InService`.**
- **Script kiểm thử bằng Python `boto3` chạy thành công.**

## Thách thức & Giải pháp

**Thách thức:** Endpoint bị lỗi thiếu thư viện khi chạy hàm suy luận.

**Giải pháp:** Thêm file `requirements.txt` vào thư mục `code/` nén cùng file trọng số mô hình.

## Đóng góp cho Dự án

Hoàn thiện "trái tim" AI của hệ thống, giúp tính toán điểm số rủi ro cho hành vi AI Agent theo thời gian thực.

## Tài liệu tham khảo

- [Deploy Models with SageMaker](https://docs.aws.amazon.com/sagemaker/latest/dg/deploy-model.html)
- [SageMaker PyTorch Container SDK](https://sagemaker.readthedocs.io/en/stable/frameworks/pytorch/using_pytorch.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.10-week10/)
