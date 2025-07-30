# 🏥 Hospital Readmission Risk Prediction

## 🔍 Project Overview

This project performs an in-depth **exploratory data analysis (EDA)** on a real-world hospital dataset to identify the **key factors driving patient readmissions within 30 days**. The goal is to uncover patterns in demographics, diagnoses, treatments, and hospital operations that contribute to readmission risks. These insights can guide healthcare systems to improve patient outcomes and reduce unnecessary hospital utilization.

---

## 📂 Dataset Details

- **Name**: Diabetes 130-US hospitals for years 1999–2008
- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/brandao/diabetes)
- **Records**: 100,000+ patient encounters
- **Features**: Age, race, gender, diagnoses, procedures, medications, admission & discharge details, readmission flag

---

## 🧠 Project Goals

- Clean, structure, and analyze hospital visit records
- Identify **high-risk factors** influencing readmission
- Explore **diagnostic patterns**, **medication behavior**, and **admission/discharge operations**
- Build a ready-to-model dataset for future machine learning applications

---

## 🛠️ Tools and Technologies

- **Python**: Data manipulation and cleaning (`pandas`, `numpy`)
- **Visualization**: `matplotlib`, `seaborn`
- **Missing Data Analysis**: `missingno`
- **Notebook**: Jupyter

---

## 📊 Key EDA Highlights

### 🎯 Target Variable Transformation
- Converted `readmitted` field into a binary classification:  
  `1 = Readmitted within 30 days`, `0 = Otherwise`

### 👤 Demographic Analysis
- Age groups 60–90 show highest readmission rates
- Slightly higher readmission observed in male patients
- Racial disparities minimal, but some skew toward certain groups

### 🩺 Diagnosis Insights
- Grouped diagnosis codes into medical categories:
  - **Diabetes**, **Circulatory**, **Neoplasms**, **Injury**, etc.
- Patients with circulatory or diabetes complications were most at risk

### 💊 Medication Behavior
- Patients with **no change in insulin levels** were more likely to be readmitted
- Specific medication combinations correlated with longer hospital stays

### 🏥 Hospital Metrics
- Longer stays and **more procedures** didn’t always increase risk — but **more inpatient visits** did
- Emergency admissions had significantly higher readmission probability

### 📈 Correlation Analysis
- Features like `number_inpatient`, `number_emergency`, and `num_procedures` showed moderate correlations with readmission
- Feature engineering performed to group diagnoses and bin age ranges

---

## 📝 Key Takeaways

- ✅ **Demographics**: Age and prior hospital use are strong predictors
- ✅ **Diagnosis Type**: Chronic conditions like diabetes, circulatory disease carry higher risks
- ✅ **Operational Flow**: Admission type (emergency) and discharge status impact readmission odds
- ✅ **Medication Use**: Insulin regulation needs further clinical attention

---

## 📁 Project Structure


[diabetic_data.csv](https://github.com/user-attachments/files/21516727/diabetic_data.csv)
