# Machine-Learning-in-Healthcare

Dự án ứng dụng các mô hình học máy (Machine Learning) trong lĩnh vực y tế nhằm hỗ trợ chẩn đoán và phát hiện sớm bệnh tim. Dự án triển khai quy trình từ tiền xử lý dữ liệu, huấn luyện nhiều mô hình phân loại khác nhau cho đến đánh giá hiệu năng chi tiết.

---

## 📌 Tính năng nổi bật

*   **Tiền xử lý dữ liệu nghiêm ngặt:** Kiểm tra & xử lý giá trị thiếu (missing values), loại bỏ các mẫu trùng lặp và chuẩn hóa dữ liệu bằng `StandardScaler`.
*   **Thử nghiệm đa mô hình:** Triển khai và so sánh hiệu năng của nhiều thuật toán phổ biến như:
    *   Random Forest
    *   Support Vector Machine (SVM)
    *   Logistic Regression
    *   *(Và các mô hình học máy khác...)*
*   **Đánh giá toàn diện:** Sử dụng các chỉ số đo lường thực tế trong y tế bao gồm **Precision**, **Recall**, và **F1-Score** để đảm bảo giảm thiểu tối đa tỷ lệ bỏ sót bệnh nhân.

---

## 🛠️ Quy trình triển khai

### 1. Tiền xử lý dữ liệu (Data Preprocessing)
*   **Missing Values:** Kiểm tra và xử lý các ô dữ liệu trống nhằm tránh làm nhiễu mô hình.
*   **Deduplication:** Loại bỏ hoàn toàn các mẫu dữ liệu bị trùng lặp để đảm bảo tính khách quan khi huấn luyện.
*   **Feature Scaling:** Áp dụng `StandardScaler` để đưa các đặc trưng về cùng một phân phối chuẩn (mean = 0, variance = 1), giúp các thuật toán như SVM hay Logistic Regression hội tụ nhanh và chính xác hơn.

### 2. Huấn luyện mô hình (Model Training)
Dự án được chia nhỏ thành các notebook thực nghiệm công khai:
*   `Heart_disease_detection_with_RandomForest.ipynb`: Tập trung tối ưu hóa thuật toán Random Forest.
*   `Heart_disease_detection_with_multiple_models.ipynb`: Thử nghiệm, so sánh và đánh giá chéo giữa các mô hình SVM, Logistic Regression,...

### 3. Tiêu chí đánh giá (Evaluation Metrics)
Trong bài toán y tế, việc cân bằng giữa nhận diện đúng người mắc bệnh và tránh báo động giả là cực kỳ quan trọng. Do đó, các mô hình được tối ưu dựa trên:
*   **Precision (Độ chính xác):** Tỷ lệ người thực sự mắc bệnh trong số những người được mô hình dự đoán là mắc bệnh.
*   **Recall (Độ nhạy):** Tỷ lệ người được mô hình phát hiện mắc bệnh trong số tất cả những người thực tế có bệnh (chỉ số này càng cao càng giúp tránh bỏ sót bệnh nhân).
*   **F1-Score:** Giá trị trung bình điều hòa giữa Precision và Recall, đại diện cho hiệu năng tổng thể của mô hình.

---

## 💻 Hướng dẫn cài đặt & Chạy dự án

1. **Clone repository này về máy:**
   ```bash
   git clone [https://github.com/AnNguyenAI/Machine-Learning-in-Healthcare.git](https://github.com/AnNguyenAI/Machine-Learning-in-Healthcare.git)
   cd Machine-Learning-in-Healthcare
