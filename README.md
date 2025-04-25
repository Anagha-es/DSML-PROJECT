# DSML-PROJECT
# 🌊 Wave Energy Converters: Power Prediction using Machine Learning

## 📌 Project Overview
This project focuses on building a predictive model to estimate the energy output of wave energy converters located in different regions of Australia. Using machine learning techniques, we aim to analyze environmental and device parameters to forecast power generation accurately.

---

## 📂 Dataset Information

- **Source**: [UCI Machine Learning Repository - Wave Energy Converters Dataset](https://archive.ics.uci.edu/dataset/1047/wave+energy+converters)
- **Type**: CSV files (no headers)
- **Regions Covered**: Adelaide, Perth, Sydney, Tasmania
- **Features**: 48 numerical columns (environmental and device parameters)
- **Target**: col_48 (energy output)

---

## ✅ Project Steps

### 📊 1. Data Collection & Exploration
- Combined datasets from four regions
- Checked for missing values, duplicates, outliers, and skewness
- Performed statistical summaries and visual analysis

### 🧹 2. Data Preprocessing
- Handled missing values and outliers using IQR method
- Addressed skewness with transformations
- Saved a clean version of the dataset

### 📈 3. Exploratory Data Analysis (EDA)
- Created over 10 visualizations (histograms, boxplots, scatter plots, heatmaps)
- Analyzed feature distributions, correlations, and anomalies

### 🧠 4. Feature Engineering & Model Building
- Applied feature scaling and selection
- Tried multiple models: Linear, Ridge, Lasso, Decision Tree, Random Forest
- Hyperparameter tuning with `RandomizedSearchCV`

### 📉 5. Model Evaluation
- Final model: **Random Forest**
- Achieved:
  - **Test R²**: 0.9976
  - **Test RMSE**: 49,199
- Confirmed results using cross-validation and evaluation on unseen data

---

## 🏁 Final Results

| Model             | Test MAE   | Test RMSE  | Test R²  |
|------------------|------------|------------|----------|
| Linear Regression| 59,986     | 75,923     | 0.9943   |
| Ridge Regression | 59,986     | 75,923     | 0.9943   |
| Lasso Regression | 871,756    | 1,009,314  | -0.0000  |
| Decision Tree    | 33,183     | 53,785     | 0.9972   |
| **Random Forest**| **28,634** | **49,199** | **0.9976** |

---

## 🔮 Future Enhancements

- Deploy the model as a web app using Streamlit or Flask
- Try ensemble models like XGBoost, LightGBM
- Integrate real-time sensor data for live predictions
- Scale to global wave energy datasets

---

## ⚠️ Limitations

- Lack of variable names in dataset
- Domain knowledge for deeper insight was limited
- Computation lag on local machine due to dataset size

---



👩‍💻 Author
Anagha E S
Batch: DSML41
email id: anaghaes6@gmail.com
