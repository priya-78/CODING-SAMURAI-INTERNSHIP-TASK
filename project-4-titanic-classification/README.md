Project 4: Logistic Regression on Titanic Dataset
📌 Overview
This project applies Logistic Regression to the Titanic dataset to predict passenger survival.
Building on the exploratory data analysis from Project 3, this project demonstrates:

Data preprocessing and cleaning

Feature engineering for better predictions

Logistic Regression model training and evaluation

Performance analysis using multiple metrics

📂 Dataset
Source: Kaggle – Titanic: Machine Learning from Disaster

Files Used:

train.csv → Training dataset with survival labels

(Optional: test.csv if you extend for Kaggle submission)

Target Variable:

Survived (0 = Did not survive, 1 = Survived)

🛠️ Skills Demonstrated
Logistic Regression (classification)

Data preprocessing and wrangling

Feature engineering and encoding

Model evaluation: Accuracy, Precision, Recall, F1-score, ROC-AUC

Data visualization (Seaborn, Matplotlib)

🔍 Feature Engineering
To improve prediction power, the following new features were created:

FamilySize = SibSp + Parch + 1

IsAlone = 1 if passenger traveled alone, else 0

Title = extracted from Name (Mr, Mrs, Miss, Master, Rare)

AgeGroup = binned into Child, Teen, Adult, Senior

FareBin = binned into Low, Medium, High, Very High

These features capture social and demographic influences on survival chances.

📊 Model Training & Evaluation
Steps
Preprocessed missing values (Age, Embarked) and dropped Cabin.

Encoded categorical variables with one-hot encoding.

Split data into training (80%) and testing (20%) sets.

Trained Logistic Regression model using scikit-learn.

Results (Sample Run)
Accuracy: ~80%

Confusion Matrix: Model predicts non-survivors more accurately than survivors.

Classification Report:

Precision (Survived = 0.77, Not Survived = 0.82)

Recall (Survived = 0.74, Not Survived = 0.85)

F1-Score balanced around 0.80

ROC Curve & AUC: Showed strong classification ability (~0.82 AUC).

📦 Deliverables
Titanic_LogisticRegression.ipynb → Jupyter/Colab notebook with full analysis

README.md → This project report

(Optional)

requirements.txt → Python dependencies

results/ → Folder for plots and figures

🚀 How to Run
Clone the repository:
git clone <your-repo-link>
cd Titanic-LogisticRegression

Open the notebook in Google Colab or Jupyter Notebook.

Run all cells to train the model and see evaluation results.

🙌 Acknowledgments
Dataset: Kaggle Titanic Competition

Internship Project: Coding Samurai Data Science Internship – Project 4
