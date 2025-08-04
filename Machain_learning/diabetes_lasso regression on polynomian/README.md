🩺 Diabetes Prediction using Regression Techniques
This project analyzes the diabetes dataset using various regression models to predict the likelihood of diabetes based on medical and demographic features.

📌 Key Objectives
🔍 Explore dataset and understand feature relationships

📊 Apply Linear Regression

📐 Apply Polynomial Regression (degree = 2)

🔒 Apply Lasso Regression for regularization

📈 Compare performance using MSE and R² score

📊 Dataset Overview
Feature	Description
Pregnancies	Number of pregnancies
Glucose	Plasma glucose concentration
BloodPressure	Diastolic blood pressure (mm Hg)
SkinThickness	Triceps skin fold thickness (mm)
Insulin	2-Hour serum insulin (mu U/ml)
BMI	Body Mass Index
DiabetesPedigreeFunction	Genetic predisposition to diabetes
Age	Age (in years)
Outcome (Target)	1 = Diabetic, 0 = Non-diabetic

Samples: 768

Target: Binary classification (0 or 1)

⚙️ Methods Used
🔸 Linear Regression
Train MSE: 0.1546

Train R²: 0.32

Test MSE: 0.1760

Test R²: 0.22

Linear regression doesn't perform well due to the non-linear nature of the problem.

🔸 Polynomial Regression (degree = 2)
Train MSE: 0.1319

Train R²: 0.42

Test MSE: 0.1823

Test R²: 0.19

Improves training performance but slightly overfits on the test data.

🔸 Lasso Regression on Polynomial Features
Intended: To reduce overfitting and improve generalization

Note: Final implementation was partially incomplete in the code
You can finalize with:

python
Copy
Edit
from sklearn.linear_model import Lasso

model_3 = Lasso(alpha=0.01)
model_3.fit(x_train, y_train)
y_pred = model_3.predict(x_test)
print(r2_score(y_test, y_pred))
📦 Requirements
bash
Copy
Edit
pip install pandas numpy matplotlib scikit-learn
▶️ How to Run
bash
Copy
Edit
python diabetes_regression.py
Ensure the file diabetes.csv is in the same directory.

📚 Insights
Regression is not ideal for binary classification; consider logistic regression or classifiers.

Polynomial expansion improves performance but risks overfitting.

Lasso helps in regularization and reducing model complexity.

🚀 Future Work
✅ Apply Logistic Regression or Random Forest Classifier

✅ Use Feature Engineering (e.g., binning age, normalizing insulin)

✅ Evaluate using ROC-AUC, Precision-Recall, and F1-score
