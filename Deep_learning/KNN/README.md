🤖 Diabetes Prediction using K-Nearest Neighbors (KNN)
This project applies a K-Nearest Neighbors (KNN) classification model to predict the likelihood of diabetes in patients using the Pima Indians Diabetes Dataset. It includes data preprocessing, model tuning, and evaluation of results.

📌 Features
✅ Loads and explores the dataset using Pandas and Seaborn

✅ Splits data using Stratified Sampling

✅ Tests multiple values of K to find the optimal number of neighbors

✅ Evaluates model performance using precision, recall, F1-score

📈 Visualizes accuracy vs. different values of K

📊 Dataset Overview
The dataset consists of 768 samples and the following features:

Pregnancies

Glucose

BloodPressure

SkinThickness

Insulin

BMI

DiabetesPedigreeFunction

Age

Outcome (0 = No diabetes, 1 = Diabetes)

⚙️ Workflow
Load & Explore Data

Used pandas to read the .csv file

Previewed basic statistics and data structure

Split Dataset

Train-test split using train_test_split

test_size=0.2, stratify=y, and random_state=2

Model Selection

Tried KNN with values of K = 1 to 30

Plotted accuracy vs. K

Best K found: K = 6

Evaluation

Used classification_report to show precision, recall, and f1-score

Evaluated both training and testing accuracy

📊 Model Performance
Best K = 6

📈 Test Set
Accuracy: 76%

Precision (Class 1): 84%

Recall (Class 1): 39%

F1-Score (Class 1): 53%

🏋️‍♀️ Train Set
Accuracy: 79%

Precision (Class 1): 80%

Recall (Class 1): 54%

F1-Score (Class 1): 65%

The model performs better at predicting non-diabetic cases. Recall for diabetic patients (class 1) could be improved with further feature engineering or balancing techniques.

📦 Requirements
bash
Copy
Edit
pip install pandas numpy matplotlib seaborn scikit-learn
▶️ How to Run
bash
Copy
Edit
python your_script_name.py
Make sure the file diabetes.csv is in the same directory.
