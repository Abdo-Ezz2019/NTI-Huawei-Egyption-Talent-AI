🌸 Iris Classification using PCA + Logistic Regression
This project demonstrates dimensionality reduction using Principal Component Analysis (PCA) followed by Logistic Regression to classify the well-known Iris dataset into its three species.

📌 Features
✅ Load and explore the Iris dataset

✅ Visualize original variance across features

✅ Apply PCA to reduce dimensionality from 4 to 2

✅ Visualize PCA output in a 2D scatter plot

✅ Train a Logistic Regression model on PCA-transformed data

✅ Evaluate using confusion matrix and classification report

🔢 Dataset Description
The Iris dataset contains 150 samples of three classes:

Setosa

Versicolor

Virginica

Each sample has 4 features:

Sepal length

Sepal width

Petal length

Petal width

📊 Variance Analysis
Before normalization, the petal length had the highest variance.

After standardization, all features have unit variance.

PCA Results:

python
Copy
Edit
Explained Variance Ratio: [0.7296, 0.2285]
This means the first two principal components explain ~95.8% of the total variance.

🎯 Model: Logistic Regression
The model was trained on the reduced 2D data (principal component 1, principal component 2) using an 80/20 train-test split.

✅ Evaluation:
Accuracy: 90%

Precision & Recall: Balanced across classes

Confusion matrix shows strong performance for all classes.

📊 Visualizations
2D scatter plot of PCA components colored by class

Confusion matrix heatmap


(add if exporting as Markdown with images)

📦 Requirements
bash
Copy
Edit
pip install numpy pandas matplotlib seaborn scikit-learn
▶️ How to Run
bash
Copy
Edit
python your_script_name.py
Replace your_script_name.py with your actual file name.

📚 Learning Outcomes
Understand PCA for feature reduction and visualization

Apply logistic regression to transformed data

Evaluate multi-class classification performance

Use confusion matrix to analyze prediction quality

