# 🎓 AI-Driven Student Performance Prediction System

## 📌 Project Overview

The **AI-Driven Student Performance Prediction System** is a Machine Learning-based project designed to predict student academic performance using academic, attendance, study habits, engagement, and support-related factors.

The system classifies students into three performance categories:

- **0 – Low Performer**
- **1 – Average**
- **2 – High Performer**

The main objective of this project is to use Artificial Intelligence and Machine Learning to identify students who may require additional academic support at an early stage.

---

## 🎯 Project Objectives

- Analyze student academic and behavioral data.
- Perform Exploratory Data Analysis (EDA).
- Check missing values and duplicate records.
- Create meaningful features using feature engineering.
- Train multiple Machine Learning classification models.
- Compare model performance using different evaluation metrics.
- Select the best-performing model.
- Predict the performance level of a new student.
- Save the trained Machine Learning model for future use.

---

## 🔄 Project Workflow

Student Data
     ↓
Data Understanding
     ↓
Data Cleaning & Quality Check
     ↓
Exploratory Data Analysis (EDA)
     ↓
Feature Engineering
     ↓
Train-Test Split
     ↓
Data Preprocessing
     ↓
Model Training
     ↓
Model Comparison
     ↓
Model Evaluation
     ↓
Best Model Selection
     ↓
New Student Prediction
     ↓
Model Saving
     ↓
Final Conclusion
📊 Dataset

The project uses a generated student performance dataset containing 2,500 student records.

The dataset includes academic, demographic, attendance, study-habit, engagement, and support-related attributes.

Main Features
Feature	Description
Student_ID	Unique student identifier
Age	Student age
Gender	Student gender
Study_Hours_Per_Day	Average daily study hours
Attendance_Percentage	Student attendance percentage
Previous_Semester_Score	Previous semester academic score
Assignment_Average	Average assignment marks
Internal_Test_Average	Average internal test marks
Sleep_Hours	Average daily sleep
Class_Participation_Percentage	Classroom participation
Extracurricular_Hours_Per_Week	Weekly extracurricular activity
Internet_Study_Hours_Per_Day	Daily internet-based study hours
Family_Support	Level of family support
Learning_Mode	Online, Offline or Hybrid
Academic_Background	Academic background
Financial_Stress	Level of financial stress
Final_Score	Final academic score
Performance_Level	Target variable
🎯 Target Variable

The target variable is:

Performance_Level

It contains three classes:

0 → At Risk
1 → Average
2 → High Performer
🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Joblib
Jupyter Notebook / Google Colab
🤖 Machine Learning Models

The project trains and compares three Machine Learning classification algorithms.

1. Logistic Regression

Logistic Regression is used as a simple and interpretable baseline classification model.

2. Decision Tree

Decision Tree is a rule-based Machine Learning algorithm that makes predictions using a sequence of decision rules.

3. Random Forest

Random Forest is an ensemble Machine Learning algorithm that combines multiple decision trees to improve prediction performance and handle non-linear relationships.

⚙️ Data Preprocessing

The project uses a Machine Learning preprocessing pipeline.

Numerical Features

Numerical features are standardized using:

StandardScaler
Categorical Features

Categorical features are converted into numerical form using:

OneHotEncoder

A ColumnTransformer and Pipeline are used to apply preprocessing consistently during training and prediction.

🧠 Feature Engineering

Additional features are created to improve the prediction process.

Academic Average

Calculated using:

Previous Semester Score
Assignment Average
Internal Test Average
Study Efficiency

Study hours are adjusted according to the student's attendance.

Engagement Score

Calculated using:

Class Participation
Attendance
Support Index

Represents the combined effect of:

Family Support
Financial Stress
📈 Exploratory Data Analysis

The project performs Exploratory Data Analysis to understand relationships between student characteristics and academic performance.

The analysis includes:

Performance level distribution
Attendance vs Final Score
Study Hours vs Final Score
Previous Semester Score vs Performance
Internal Test Performance
Correlation Heatmap
Student engagement analysis
Student support analysis
📊 Model Evaluation

The Machine Learning models are evaluated using multiple performance metrics:

Accuracy
Precision
Recall
F1 Score
ROC-AUC
Confusion Matrix
Classification Report

The models are compared based on their overall performance, and the best-performing model is selected for the final prediction stage.

🔍 Student Performance Prediction

After selecting the best-performing model, the system can predict the performance category of a new student.

Example student information:

Age: 21
Study Hours: 5 hours/day
Attendance: 88%
Previous Semester Score: 78
Assignment Average: 82
Internal Test Average: 80
Sleep Hours: 7
Class Participation: 85%
Family Support: High
Learning Mode: Hybrid
Financial Stress: Low

The trained model generates:

Predicted Performance Level

along with prediction probabilities for:

low Performer
Average
High Performer

💾 Model Saving

The trained Machine Learning pipeline is saved using Joblib.

joblib.dump(best_model, "student_performance_prediction_model.joblib")

The saved model can later be loaded and used for predictions without rebuilding the complete Machine Learning pipeline.

🏫 Applications

This system can help educational institutions to:

Identify potentially at-risk students.
Plan remedial classes.
Monitor attendance and study habits.
Support academic counselling.
Prioritize students who may need additional support.
Make data-driven academic decisions.
Develop an academic early-warning system.
⚠️ Limitations

The prediction generated by this system should be treated as a decision-support indicator, not as a permanent judgment about a student.

Student performance can change due to academic, personal, social, and environmental factors that may not be included in the dataset.

🚀 Future Enhancements

The project can be further developed into:

Interactive Streamlit Dashboard
Web-Based Student Prediction System
College Academic Early-Warning System
Real-Time Student Performance Monitoring
Student Performance Visualization Dashboard
REST API for Predictions
Integration with Real College/Student Databases
Automated Academic Recommendations


📁 Project Structure
AI-Driven-Student-Performance-Prediction/
│
├── AI_Driven_Student_Performance_Prediction_System.ipynb
├── student_performance_dataset.csv
├── student_performance_prediction_model.joblib
└── README.md


▶️ How to Run the Project
Step 1: Clone the Repository
git clone YOUR_GITHUB_REPOSITORY_URL
Step 2: Open the Notebook

Open:

AI_Driven_Student_Performance_Prediction_System.ipynb

using Jupyter Notebook or Google Colab.

Step 3: Install Required Libraries
pip install pandas numpy matplotlib seaborn scikit-learn joblib
Step 4: Run the Notebook

Run all cells from beginning to end.

The notebook will:

Generate the student dataset.
Perform data quality checks.
Perform Exploratory Data Analysis.
Create engineered features.
Train Machine Learning models.
Compare model performance.
Evaluate the best model.
Predict a new student's performance.
Save the trained model.


📌 Conclusion

The AI-Driven Student Performance Prediction System demonstrates how Artificial Intelligence and Machine Learning can be applied to educational analytics.

The project follows a complete Machine Learning workflow, including:

Data Preparation → EDA → Feature Engineering → Preprocessing → Model Training → Model Evaluation → Best Model Selection → Prediction

The system can serve as a foundation for developing an intelligent academic early-warning and student-support platform.

👨‍💻 Author

Swayam Sharma

MBA – IBM

AI & Machine Learning Project
