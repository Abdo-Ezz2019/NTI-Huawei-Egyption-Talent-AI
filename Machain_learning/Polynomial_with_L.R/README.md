🏠 Boston Housing Price Prediction using Regression Models
This project demonstrates how to predict housing prices using various regression techniques on the Boston Housing dataset, including:

Linear Regression

Polynomial Regression

Lasso Regression

📊 Dataset Overview
Source: housing.csv (Boston Housing dataset)

Samples: 506

Features: 13 (e.g., crime rate, number of rooms, distance to employment centers)

Target: Median house price (MEDV)

⚙️ Workflow
Load and Preprocess Data

Read dataset with sep='\s+' (space-separated values)

Normalize features using StandardScaler

Linear Regression

Train a base linear model

Evaluate performance using MSE and R²

Polynomial Regression (degree=2)

Use PolynomialFeatures to expand input

Fit and evaluate using training & test splits

Lasso Regression

Add regularization with Lasso(alpha=0.03)

Compare against polynomial regression

📈 Model Performance
✅ Linear Regression (Baseline)
Metric	Value
Train R²	~0.74
MSE (train)	Moderate

📐 Polynomial Regression (degree=2)
Set	MSE	R²
Train	5.60	0.939
Test	11.14	0.829

📏 Lasso Regression on Polynomial Features
Set	MSE	R²
Train	7.02	0.924
Test	10.12	0.844

✅ Lasso helped reduce overfitting slightly while maintaining good generalization.

📦 Requirements
bash
Copy
Edit
pip install pandas numpy scikit-learn
▶️ How to Run
bash
Copy
Edit
python housing_regression.py
Ensure the file housing.csv is in the same directory.

📚 Key Learnings
Normalize features before training for better results

Polynomial regression improves fitting but risks overfitting

Lasso adds regularization to improve model generalization

Always compare models using both training and test sets

📌 Future Improvements
Try Ridge Regression as another regularization method

Visualize residual errors or prediction scatter plots

Deploy the trained model via Flask or Streamlit
