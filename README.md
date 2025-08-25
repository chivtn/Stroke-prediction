# 🧠 Stroke Data Preprocessing Project

## 📌 Giới thiệu
Dự án này thực hiện tiền xử lý dữ liệu về **đột quỵ** (stroke prediction dataset).  
Mục tiêu là làm sạch, xử lý dữ liệu thiếu và chuẩn hóa các thuộc tính trước khi đưa vào các mô hình học máy dự đoán khả năng bị đột quỵ.

## 🛠️ Các bước thực hiện

1. **Đọc dữ liệu**  
   - Nguồn: `data_dotquy.csv`  
   - Sử dụng thư viện `pandas` để tải và thao tác dữ liệu.

2. **Làm sạch dữ liệu**
   - Loại bỏ các bản ghi trùng lặp theo `id`.
   - Xử lý giá trị thiếu:
     - Sử dụng **KNN Imputer** để điền dữ liệu thiếu trong cột `bmi`.
   - Loại bỏ cột không cần thiết (`id`).

3. **Xử lý dữ liệu phân loại**
   - Giới tính (`gender`): Male → 0, Female → 1 (loại bỏ giá trị *Other*).
   - Tình trạng hôn nhân (`ever_married`): No → 0, Yes → 1.
   - Loại công việc (`work_type`): Mã hóa bằng **LabelEncoder**.
   - Nơi ở (`Residence_type`): Rural → 0, Urban → 1.

4. **Chuẩn hóa dữ liệu số**
   - Tuổi (`age`), chỉ số đường huyết trung bình (`avg_glucose_level`), BMI (`bmi`) được chuẩn hóa bằng **Min-Max Scaling**.

## 📚 Công nghệ sử dụng
- Python
- pandas, numpy
- scikit-learn (KNN Imputer, LabelEncoder, MinMaxScaler)
- matplotlib / seaborn (nếu trực quan dữ liệu)

## 🚀 Hướng phát triển
- Áp dụng các mô hình học máy (Logistic Regression, Random Forest, XGBoost, v.v.) để dự đoán nguy cơ đột quỵ.
- Trực quan dữ liệu chi tiết hơn (histogram, correlation heatmap).
- Tối ưu pipeline xử lý dữ liệu.

## 👩‍💻 Nhóm thực hiện
- Hien
- Chau
- Chi
- Giang
- Hoang
