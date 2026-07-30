---
title: "Chia Sẻ & Góp Ý"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 7. </b> "
---

## Chia Sẻ & Góp Ý Chương Trình

Chuyên mục này tổng hợp những góc nhìn, trải nghiệm cá nhân và đóng góp ý kiến của mình sau khi hoàn thành chương trình **Workforce Bootcamp - First Cloud AI Journey** tại **Công ty TNHH Amazon Web Services Việt Nam**. Toàn bộ các nhận định dưới đây được đúc kết từ quá trình mình tự học các dịch vụ đám mây AWS, tích cực giao lưu tại các sự kiện công nghệ và trực tiếp xây dựng dự án **Hệ thống Tự động hóa Đánh giá Rủi ro cho AI Coding Agent trên AWS SageMaker**.

---

## Đánh Giá Tổng Quan Chương Trình

### 1. Môi trường trải nghiệm & Định hướng học tập
Chương trình mang lại một không gian học tập linh hoạt và đề cao tính tự chủ. Thay bị gò bó trong các bài thực hành có sẵn, sinh viên được tự do nghiên cứu các dịch vụ AWS, thử nghiệm các ý tưởng kỹ thuật và tự định hình một sản phẩm thực tế từ bước sơ khai đến bản hoàn thiện. Điều này giúp mình rèn luyện tư duy tự chịu trách nhiệm và chủ động giải quyết vấn đề.

### 2. Sự đồng hành từ Ban tổ chức & Cộng đồng
Mặc dù làm việc theo mô hình tự nghiên cứu, mình vẫn nhận được sự hỗ trợ rất lớn từ tài liệu kỹ thuật chuẩn của AWS, các buổi Workshop thực hành và các sự kiện kết nối cộng đồng FCAJ. Các buổi hội thảo giúp mình cập nhật góc nhìn thực tế về quy trình vận hành Cloud, MLOps, Security, Data Analytics và Generative AI từ các chuyên gia hàng đầu.

### 3. Mức độ phù hợp với Chuyên ngành học
Kỳ thực tập cực kỳ gắn kết với ngành Khoa học Máy tính mà mình đang theo học tại trường Đại học. Chương trình tạo điều kiện để mình xâu chuỗi các kiến thức về Lập trình, Xử lý dữ liệu, Machine Learning, Thiết kế API và Kiến trúc hệ thống; từ đó hiện thực hóa các lý thuyết học đường trên hạ tầng điện toán đám mây enterprise của AWS.

### 4. Cơ hội phát triển năng lực & Kỹ năng
- **Kỹ năng chuyên môn:** Làm chủ quy trình vận hành các dịch vụ AWS như S3, SageMaker (Processing, Training, HPO, Pipelines, Registry, Endpoint, Model Monitor), AWS Lambda, API Gateway, IAM Roles, Data Capture và CloudWatch.
- **Kỹ năng mềm:** Rèn luyện tư duy quản trị MLOps, ý thức kiểm soát chi phí tài nguyên, kỹ năng đóng gói tài liệu kỹ thuật song ngữ và phương pháp kiểm thử khoa học, minh bạch.

### 5. Văn hóa kết nối & Tinh thần cộng đồng
Văn hóa chia sẻ tri thức là một điểm sáng lớn. Thông qua các sự kiện lớn do chương trình tổ chức, kỳ thực tập không chỉ dừng lại ở phạm vi một dự án cá nhân mà còn mở ra cơ hội giao lưu, lắng nghe chia sẻ nghề nghiệp từ các anh chị đi trước, giúp mình định hình rõ ràng hơn về con đường phát triển sự nghiệp MLOps/Cloud Engineer.

### 6. Khả năng ứng biến & Quy mô dự án
Việc tự quản lý dự án đòi hỏi khả năng thích ứng cao trước các rào cản kỹ thuật. Khi gặp rào cản về quota tài nguyên SageMaker Training tại vùng `ap-southeast-1`, mình đã linh hoạt triển khai phương án phụ trợ trước khi chính thức được duyệt tài nguyên tại vùng `us-east-1`. Trải nghiệm này dạy mình bài học về tư duy ứng biến linh hoạt trong kỹ thuật mà vẫn đảm bảo tính toàn vẹn của kiến trúc tổng thể.

---

## Trải Nghiệm Hài Lòng Nhất

Điều khiến mình tự hào nhất là đã biến một ý tưởng trên giấy thành một **Hệ thống MLOps hoàn chỉnh (End-to-End Workflow)** chạy thực tế trên AWS. Tự tay thiết lập trọn vẹn luồng dữ liệu từ khâu xử lý log hành vi, huấn luyện mô hình XGBoost, tối ưu HPO, tự động hóa bằng SageMaker Pipelines, cấu hình cổng kiểm duyệt Quality Gates, triển khai API thời gian thực và thiết lập hệ thống cảnh báo CloudWatch là một cột mốc rất ý nghĩa.

Bên cạnh đó, mình rất coi trọng tính trung thực trong nghiên cứu. Việc chủ động đưa mô hình ra kiểm thử trên tập dữ liệu thực tế bên ngoài (OOD) và minh bạch báo cáo kết quả suy giảm chỉ số đã giúp mình hiểu sâu sắc giá trị của khâu phê duyệt thủ công (Manual Approval) và các quy tắc bảo mật cứng (Hard Safety Rules) trong môi trường thực tế.

---

## Ý Kiến Đóng Góp Cải Thiện

1. **Khảo sát Quota ban đầu:** Nên bổ sung một tài liệu hướng dẫn kiểm tra và xin cấp phát Quota tài nguyên (đặc biệt là SageMaker Training và Endpoints) ngay từ tuần đầu tiên để sinh viên chủ động chuẩn bị.
2. **Checklist kiểm soát chi phí (Cost Control):** Cung cấp danh mục kiểm tra tài nguyên có phát sinh chi phí duy trì (như SageMaker Endpoint, NAT Gateway) giúp sinh viên có thói quen dọn dẹp (Clean-up) đúng cách, tránh phát sinh chi phí ngoài ý muốn.
3. **Mẫu kiến trúc tham khảo:** Bổ sung thêm các tài liệu mẫu chuẩn hóa (Reference Architectures) về cách kết hợp S3, SageMaker, Lambda và API Gateway cho các bài toán MLOps căn bản.
4. **Các cột mốc đánh giá định kỳ (Milestones):** Bổ sung 1-2 buổi Review ngắn giữa kỳ để sinh viên nhận phản hồi trực tiếp từ các anh chị mentor trước khi bước vào giai đoạn hoàn thiện báo cáo cuối cùng.

---

## Khuyên Dùng Chương Trình (Recommendation)

Mình chắc chắn sẽ giới thiệu chương trình **First Cloud AI Journey** đến các bạn sinh viên có mong muốn dấn thân vào lĩnh vực Cloud và AI. Đây là một bệ phóng tuyệt vời cho những ai đã có nền tảng lập trình cơ bản và muốn trải nghiệm cách thức đưa một mô hình trí tuệ nhân tạo lên hạ tầng đám mây thực tế. Chương trình đòi hỏi tính tự giác cao, nhưng chính điều đó sẽ giúp sinh viên trưởng thành nhanh chóng về cả tư duy kỹ thuật lẫn tác phong làm việc chuyên nghiệp.

---

## Định Hướng Phát Triển Trong Tương Lai

Nếu tiếp tục mở rộng dự án **AI Coding Agent Risk Scorer**, mình sẽ tập trung vào các hướng phát triển sau:
- Mở rộng thu thập tập dữ liệu hành vi agent thực tế đa dạng hơn với sự gán nhãn độc lập từ các chuyên gia con người.
- Phát triển thêm các bộ chuyển đổi (Adapters) hỗ trợ nhiều Framework AI Agent khác nhau.
- Tối ưu hóa các ngưỡng phân loại rủi ro, đồng bộ triệt để môi trường Runtime và thiết lập quy trình triển khai an toàn (Canary/Rollback Deployment) sau khi mô hình được phê duyệt thủ công trên Model Registry.
