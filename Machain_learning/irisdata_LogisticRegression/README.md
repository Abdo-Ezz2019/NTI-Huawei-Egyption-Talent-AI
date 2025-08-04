🌸 Iris Flower Classification using Logistic Regression
This project utilizes the classic Iris dataset to train a Logistic Regression classifier that accurately predicts the species of iris flowers based on their physical features.

📌 Objectives
📊 Load and explore the Iris dataset

🧪 Split into training and testing sets

🤖 Train a Logistic Regression model

✅ Evaluate performance using:

Classification Report

Confusion Matrix

Accuracy, Precision, Recall, F1-score

📈 Visualize results using Seaborn heatmaps

🛠️ Tools & Libraries
bash
Copy
Edit
pandas
numpy
scikit-learn
matplotlib
seaborn
🌼 Dataset Info
📦 Source: sklearn.datasets.load_iris()

🔢 Samples: 150

🧬 Features:

sepal length (cm)

sepal width (cm)

petal length (cm)

petal width (cm)

🎯 Target: Flower species (0 = Setosa, 1 = Versicolor, 2 = Virginica)

🤖 Model Used
python
Copy
Edit
LogisticRegression(max_iter=200)
🎯 Evaluation Results
Classification Report:

Metric	Class 0	Class 1	Class 2
Precision	1.00	1.00	1.00
Recall	1.00	1.00	1.00
F1-score	1.00	1.00	1.00

Accuracy: 100%
✅ All test predictions were correct.

🔍 Confusion Matrix
lua
Copy
Edit
[[10  0  0]
 [ 0  9  0]
 [ 0  0 11]]
Visualized as:

(if saved)

📈 How to Run
bash
Copy
Edit
python iris_classification.py
📚 Notes
This project shows the simplicity yet effectiveness of Logistic Regression in solving multi-class classification.

Consider comparing it with other classifiers like:

K-Nearest Neighbors

Decision Tree

Support Vector Machines (SVM)

 
