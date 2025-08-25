# 🧠 Stroke Data Preprocessing Project

## 📌 Introduction
This project focuses on **data cleaning and preprocessing** for a **stroke prediction dataset**.  
The goal is to handle missing values, encode categorical features, and normalize numerical attributes so the data can be used effectively in machine learning models for stroke prediction.

## 🛠️ Workflow

1. **Data Loading**  
   - Source: `data_dotquy.csv`  
   - Loaded using `pandas`.

2. **Data Cleaning**
   - Remove duplicate records based on `id`.
   - Handle missing values:
     - Apply **KNN Imputer** to fill missing values in the `bmi` column.
   - Drop unnecessary columns (`id`).

3. **Categorical Encoding**
   - Gender (`gender`): Male → 0, Female → 1 (drop *Other*).
   - Marital status (`ever_married`): No → 0, Yes → 1.
   - Work type (`work_type`): Encoded using **LabelEncoder**.
   - Residence type (`Residence_type`): Rural → 0, Urban → 1.

4. **Numerical Normalization**
   - Age (`age`), average glucose level (`avg_glucose_level`), and BMI (`bmi`) normalized using **Min-Max Scaling**.
## 📚 Technologies Used
- Python
- pandas, numpy
- scikit-learn (KNN Imputer, LabelEncoder, MinMaxScaler)
- matplotlib / seaborn (for data visualization)

## 🚀 Future Development
- Apply machine learning models (Logistic Regression, Random Forest) to predict stroke risk.
- Perform deeper data visualization (histograms, correlation heatmaps).
- Optimize preprocessing pipeline for scalability.

## 👩‍💻 Contributors
- Hien
- Chau
- Chi
- Giang
- Hoang
