# Gold Recovery Prediction

## 📌 Project Description
This project focuses on predicting the gold recovery in a mineral processing plant. The goal is to develop a machine learning model that can accurately estimate the recovery at the final stage based on process parameters measured at different stages of purification.

The datasets provided include training, test, and the full raw data:

- `gold_recovery_train.csv` — training dataset  
- `gold_recovery_test.csv` — test dataset (targets not provided)  
- `gold_recovery_full.csv` — complete raw dataset  

---

## 🎯 Project Objectives
- Preprocess and analyze the data to understand key process variables  
- Identify and handle missing features, anomalies, and distribution differences between training and test sets  
- Explore the relationships between metal concentrations (Au, Ag, Pb) and processing stages  
- Build regression models to predict gold recovery  
- Evaluate model performance using **sMAPE** and cross-validation  
- Select the best-performing model and validate it on the test set  

---

## 📊 Data Description
- Index: `date` (timestamp of measurement)  
- Features: multiple process parameters measured at different stages of purification  
- Target: `rougher.output.recovery` (gold recovery at rougher stage) for training data  

Notes:
- Some features are missing in the test set because they are calculated later in the process  
- Raw data includes all available features for exploration and preprocessing  

---

## ⚙️ Methodology
1. **Data preparation**
   - Load and inspect datasets
   - Check recovery calculations
   - Analyze missing features and their types
   - Preprocess data (handle missing values, anomalies, scaling)

2. **Exploratory Data Analysis**
   - Track metal concentrations (Au, Ag, Pb) across purification stages
   - Compare particle size distributions between train and test
   - Analyze total concentrations and remove anomalies if necessary

3. **Model Building**
   - Define a function to compute final sMAPE
   - Train multiple regression models
   - Validate using cross-validation
   - Evaluate on the test set and report results

---

## 🛠️ Tools & Libraries
- Python
- pandas
- NumPy
- scikit-learn
- matplotlib / seaborn
- Jupyter Notebook

---

## ✅ Outcome
- Fully cleaned and processed datasets ready for modeling  
- Visualizations highlighting differences between stages and datasets  
- Predictive model for gold recovery with validated performance  
- Insights and recommendations for improving process control in mineral processing  

---

## 📌 Author
**Felipe Yánez**  
Data Scientist
