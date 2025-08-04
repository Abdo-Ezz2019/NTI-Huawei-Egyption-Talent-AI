🏠 Boston Housing Price Prediction using Regression
This project uses the Boston Housing Dataset to predict house prices based on various neighborhood and housing features. It applies different regression techniques to compare their predictive performance.

📌 Objectives
🧼 Preprocess and scale data using StandardScaler

📉 Apply Linear Regression

🧮 Apply Polynomial Regression (degree 2)

🔒 Apply Lasso Regression on polynomial features

📊 Compare performance using Mean Squared Error and R² score

📊 Dataset Overview
📄 Source: housing.csv (assumed to be Boston Housing Data format)

🔢 Records: 506 rows × 14 columns

🏷️ Features:

Feature	Description
CRIM	Crime rate per capita
ZN	Proportion of residential land zoned
INDUS	Proportion of non-retail business acres
CHAS	Charles River dummy variable (1 if tract bounds river, 0 otherwise)
NOX	Nitric oxides concentration (parts per 10 million)
RM	Average number of rooms per dwelling
AGE	Proportion of owner-occupied units built before 1940
DIS	Weighted distance to employment centers
RAD	Index of accessibility to radial highways
TAX	Full-value property-tax rate
PTRATIO	Pupil-teacher ratio by town
B	1000(Bk - 0.63)^2, where Bk is proportion of Black residents
LSTAT	% lower status of the population
MEDV (Target)	Median value of homes in $1000s

🛠️ Tools & Libraries
bash
Copy
Edit
pandas
numpy
matplotlib
scikit-learn
⚙️ Model Summary
🔹 1. Linear Regression
python
Copy
Edit
MSE (Train): 0.7432  
R²   (Train): ~0.74
➡️ أداء جيد، لكن ليس مثاليًا.

🔹 2. Polynomial Regression (Degree 2)
python
Copy
Edit
Training MSE: 5.60  
Training R²:  0.94

Test MSE:     11.14  
Test R²:      0.83
✅ تحسين ملحوظ في الأداء على بيانات التدريب
⚠️ يظهر بعض علامات الـ overfitting على بيانات الاختبار

🔹 3. Lasso Regression on Polynomial Features
python
Copy
Edit
Training MSE: 7.02  
Training R²:  0.92

Test MSE:     10.12  
Test R²:      0.84
✅ أداء عام ممتاز
✅ تقليل الـ overfitting باستخدام regularization
✅ احتفاظ بخصائص متعددة مهمة وتجاهل غير المؤثرة

📈 Performance Comparison
Model	Train R²	Test R²	Remarks
Linear Regression	~0.74	~0.74	Baseline
Polynomial (Deg=2)	0.94	0.83	High variance (overfitting)
Lasso + Polynomial	0.92	0.84	Best generalization so far

📁 How to Run
bash
Copy
Edit
python boston_regression.py
Ensure the file housing.csv is in the same directory.

💡 Future Work
✅ Try Ridge Regression

✅ Use GridSearchCV to optimize alpha in Lasso/Ridge

✅ Feature Engineering: Interaction terms, dimensionality reduction

✅ Evaluate residuals and feature importance visually

📬 Notes
delim_whitespace=True is deprecated, use sep='\s+' instead:

python
Copy
Edit
pd.read_csv("housing.csv", sep='\s+')
