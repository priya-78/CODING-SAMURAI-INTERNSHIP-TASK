# 🚢 Exploratory Data Analysis on the Titanic Dataset  

## 📌 Overview  
This project focuses on performing **Exploratory Data Analysis (EDA)** on the **Kaggle Titanic dataset**.  
The goal of this analysis is to clean the dataset, explore key patterns, and visualize relationships between features and survival outcomes.  

---

## 📂 Dataset  
- **Source**: [Kaggle – Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data)  
- **Files Used**:  
  - `train.csv` → Training data with survival labels  
  - `test.csv` and `gender_submission.csv` (provided in Kaggle, but not required for EDA)  

- **Shape**: `891 rows × 12 columns`  
- **Target Variable**: `Survived` (0 = No, 1 = Yes)  

---

## 🛠️ Skills Demonstrated  
- Data wrangling and handling missing values  
- Exploratory Data Analysis (EDA) using **Pandas**, **Seaborn**, and **Matplotlib**  
- Statistical summaries and correlation analysis  
- Data visualization: histograms, bar plots, boxplots, heatmaps  

---

## 🔍 Analysis Workflow  

1. **Data Inspection**  
   - Checked data types, missing values, and statistical summaries.  

2. **Handling Missing Values**  
   - Filled missing `Age` values with the median.  
   - Imputed missing `Embarked` values with the mode.  
   - Dropped `Cabin` due to excessive missing values.  

3. **Univariate Analysis**  
   - Survival count distribution  
   - Passenger class distribution  
   - Age distribution  

4. **Bivariate Analysis**  
   - Survival rates by gender  
   - Survival rates by passenger class  
   - Age distribution by survival outcome  

5. **Correlation Analysis**  
   - Converted categorical variables (Sex, Embarked) into numeric form.  
   - Plotted a correlation heatmap to identify feature relationships.  

---

## 📊 Key Insights  

- **Gender**: Females had a significantly higher chance of survival compared to males.  
- **Passenger Class**: 1st-class passengers survived at a higher rate than those in 2nd or 3rd class.  
- **Fare**: Higher fares showed a positive correlation with survival.  
- **Age**: Younger passengers (especially children) had slightly better survival rates, although correlation with age overall was weak.  
- **Family Size**: Number of siblings/spouses (`SibSp`) and parents/children (`Parch`) showed little correlation with survival.  

---

## 📦 Deliverables  
- `Titanic_EDA.ipynb` → Jupyter Notebook with the full analysis  
- `train.csv` → Dataset used for analysis  
- `README.md` → Project documentation and insights  

---

## 🚀 How to Run  
1. Clone the repository:  
   ```bash
   git clone <your-repo-link>
   cd Titanic-EDA
   ```
2. Open the Jupyter Notebook or Google Colab.  
3. Run cells step-by-step to reproduce the analysis.  

---

## 🙌 Acknowledgments  
- Dataset provided by [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic/data).  
- Analysis inspired by the **Coding Samurai Data Science Internship (Project 3: EDA on Titanic Dataset)**.  
