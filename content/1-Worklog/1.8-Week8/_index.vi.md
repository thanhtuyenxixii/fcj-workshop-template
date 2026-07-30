---
title: "Tuần 8: Chuẩn bị Dữ liệu ML & SageMaker Notebooks"
date: 2026-07-20
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

## 20/07/2026 - 26/07/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Chuẩn bị tập dữ liệu cho mô hình Đánh giá Rủi ro, khởi tạo Amazon SageMaker Notebook Instance và xây dựng pipeline trích xuất đặc trưng (Feature Extraction).

## Bối cảnh

Tuần 8 chuyển sang giai đoạn phát triển Machine Learning. Mục tiêu là biến đổi log hành vi thô của AI Coding Agent thành các vector đặc trưng phục vụ huấn luyện mô hình PyTorch.

## Trọng tâm học tập AWS

- **Môi trường Amazon SageMaker:** Notebook Instance, Lifecycle Configurations và tích hợp S3.
- **Trích xuất Đặc trưng (Feature Engineering):** Rút trích chỉ số rủi ro (lệnh shell nguy hiểm, tần suất sửa file, truy cập mạng).
- **IAM Role cho SageMaker:** Phân quyền đọc/ghi vào S3 Bucket dự án.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 20/07/2026 | Phân tích log AI Agent và chọn lọc các đặc trưng đánh giá rủi ro. |
| 21/07/2026 | Khởi tạo SageMaker Notebook Instance (`ml.t3.medium`). |
| 22/07/2026 | Viết script Python trích xuất đặc trưng từ JSON sang Pandas DataFrame. |
| 23/07/2026 | Chia tập dữ liệu Train/Validation và đẩy lên `s3://.../processed-features/`. |
| 24/07/2026 | Kiểm thử đọc dữ liệu S3 bằng SageMaker Python SDK (`sagemaker.s3.S3Uploader`). |
| 25/07/2026 - 26/07/2026 | Tổng hợp thống kê tập dữ liệu và lưu Notebook. |

## Hoạt động kỹ thuật

- Khởi tạo SageMaker Notebook với IAM Execution Role thích hợp.
- Chuẩn hóa log thô thành dạng bảng dữ liệu số sẵn sàng cho PyTorch.

## Kết quả đạt được (Deliverables)

- **SageMaker Notebook Instance sẵn sàng.**
- **Pipeline trích xuất đặc trưng bằng Python hoàn thành.**
- **Tập dữ liệu huấn luyện đã được tải lên Amazon S3.**

## Thách thức & Giải pháp

**Thách thức:** Cấu trúc JSON không đồng nhất giữa các phiên chạy AI Agent khác nhau.

**Giải pháp:** Viết hàm chuẩn hóa dữ liệu (Normalizer) để bù đắp các trường dữ liệu thiếu trước khi trích xuất.

## Đóng góp cho Dự án

Chuyển đổi dữ liệu log thô thành tập Dataset chất lượng cao phục vụ cho bước huấn luyện mô hình.


## Tài liệu tham khảo

- [Amazon SageMaker Developer Guide](https://docs.aws.amazon.com/sagemaker/latest/dg/whatis.html)
- [SageMaker Python SDK](https://sagemaker.readthedocs.io/)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.9-week9/)
