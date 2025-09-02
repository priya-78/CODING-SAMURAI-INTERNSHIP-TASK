# 🚢 Project 4: Logistic Regression on Titanic Dataset  

## 📌 Overview  
This project applies **Logistic Regression** to the Titanic dataset to predict passenger survival.  
Building on the exploratory data analysis from **Project 3**, this project demonstrates:  

- 🔹 Data preprocessing and cleaning  
- 🔹 Feature engineering for better predictions  
- 🔹 Logistic Regression model training and evaluation  
- 🔹 Performance analysis using multiple metrics  

---

## 📂 Dataset  
- **Source**: [Kaggle – Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data)  
- **Files Used**:  
  - `train.csv` → Training dataset with survival labels  
  - *(Optional: `test.csv` for Kaggle submission)*  

- **Target Variable**: `Survived` (0 = Did not survive, 1 = Survived)  

---

## 🛠️ Skills Demonstrated  
- Logistic Regression (Classification)  
- Data Preprocessing & Wrangling  
- Feature Engineering & Encoding  
- Model Evaluation (Accuracy, Precision, Recall, F1-score, ROC-AUC)  
- Data Visualization (Seaborn, Matplotlib)  

---

## 🔍 Feature Engineering  
To improve prediction power, the following features were created:  
- 👨‍👩‍👧 **FamilySize** = `SibSp + Parch + 1`  
- 🧍 **IsAlone** = 1 if passenger traveled alone, else 0  
- 🏷️ **Title** = extracted from `Name` (Mr, Mrs, Miss, Master, Rare)  
- 🎂 **AgeGroup** = binned into Child, Teen, Adult, Senior  
- 💰 **FareBin** = binned into Low, Medium, High, Very High  

---

## 📊 Model Training & Evaluation  

### 🔹 Steps  
1. Preprocessed missing values (`Age`, `Embarked`) and dropped `Cabin`  
2. Encoded categorical variables with one-hot encoding  
3. Split data into training (80%) and testing (20%) sets  
4. Trained **Logistic Regression** model using scikit-learn  

### 🔹 Results (Sample Run)  
- ✅ **Accuracy**: ~80%  
- ✅ **Confusion Matrix**: Model predicts non-survivors more accurately than survivors  
- ✅ **Classification Report**:  
  - Precision (Survived = 0.77, Not Survived = 0.82)  
  - Recall (Survived = 0.74, Not Survived = 0.85)  
  - F1-Score balanced ~0.80  
- ✅ **ROC Curve & AUC**: ~0.82 (strong classification ability)  

---

## 📦 Deliverables  
- 📓 `Titanic_LogisticRegression.ipynb` → Full analysis notebook  
- 📘 `README.md` → Project documentation  

*(Optional additions)*  
- 📂 `results/` → Confusion Matrix, ROC Curve plots  
- 📄 `requirements.txt` → Dependencies for reproducibility  

---

## 🚀 How to Run  
1. Clone the repository:  
   ```bash
   git clone <your-repo-link>
   cd Titanic-LogisticRegression
