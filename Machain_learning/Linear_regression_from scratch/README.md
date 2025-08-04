📈 Student Performance Prediction using Linear Regression
This project demonstrates how to apply both Simple Linear Regression and Multiple Linear Regression to predict student exam scores based on study hours, attendance, and assignment completion.

📌 Objectives
✅ Understand linear relationships in educational data

✅ Apply manual linear regression using mathematical formulas

✅ Use scikit-learn's LinearRegression for training models

✅ Evaluate model accuracy using metrics like R² and MSE

📊 Dataset Overview
Simple Regression:
Hours_Studied	Score
1	50
...	...
10	97

Multiple Regression:
Hours_Studied	Attendance	Assignments_Completed	Score
1	60	1	52
...	...	...	...
10	95	6	96

🧮 Simple Linear Regression
📌 Formula-Based (Manual):
python
Copy
Edit
Slope (m)     = 5.21  
Intercept (b) = 47.07
Predicted Score (for 11 hours):
Score = 5.21 * 11 + 47.07 = 104.33

📌 Using Scikit-Learn:
python
Copy
Edit
Accuracy (R²): 0.9858
🤖 Multiple Linear Regression
python
Copy
Edit
Features Used: ['Hours_Studied', 'Attendance', 'Assignments_Completed']
📈 Evaluation Metrics:
Mean Squared Error (MSE): 1.72

R-squared (R²): 0.995

📌 Model Coefficients:
Feature	Coefficient
Hours_Studied	3.48
Attendance	0.20
Assignments_Completed	1.28

Intercept: 33.46

📦 Requirements
bash
Copy
Edit
pip install pandas numpy matplotlib scikit-learn
▶️ How to Run
bash
Copy
Edit
python your_script_name.py
Replace your_script_name.py with your actual script file name.

📚 Educational Use Case
This project is ideal for:

Understanding regression in real-life academic data

Teaching students how input features affect performance

Visualizing and interpreting regression coefficients
