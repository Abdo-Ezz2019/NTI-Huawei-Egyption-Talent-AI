🌳 Iris Classification using Decision Tree
This project demonstrates how to build, train, visualize, and evaluate a Decision Tree Classifier using the classic Iris dataset. It includes model saving/loading and a learning curve visualization to assess performance.

📌 Key Features
✅ Use Scikit-learn's DecisionTreeClassifier

✅ Visualize the trained decision tree structure

✅ Evaluate model accuracy and generalization using learning curves

✅ Save and reload model with Pickle

✅ Perform prediction on random input data

📊 Dataset Description
The Iris dataset consists of 150 samples from 3 flower species:

Setosa

Versicolor

Virginica

Each sample includes 4 features:

Sepal Length

Sepal Width

Petal Length

Petal Width

⚙️ Model Workflow
Load Dataset: Using sklearn.datasets.load_iris()

Split Data: 80% training / 20% testing

Train Model: DecisionTreeClassifier(criterion='gini')

Predict & Evaluate: Achieved 100% accuracy

Save/Load Model: Using pickle

Visualize Tree: Using tree.plot_tree(...)

Learning Curve: Shows overfitting/underfitting behavior

Random Prediction: Predict species from synthetic random data

📈 Performance
Test Accuracy: 1.00 (perfect on this simple dataset)

Learning Curve: Shows high training performance and stable cross-validation

📦 Requirements
bash
Copy
Edit
pip install numpy pandas matplotlib scikit-learn
▶️ How to Run
bash
Copy
Edit
python your_script_name.py
Make sure model_1.pkl exists in the directory if you're testing model loading.

📊 Visual Outputs
Decision Tree Diagram: Clearly shows how features split into decisions

Learning Curve: Useful for analyzing model generalization

🧪 Example Prediction
python
Copy
Edit
Prediction for random data [[...]]: virginica
💡 Tips
You can change the splitting criterion to "entropy" for information gain

Try limiting the tree depth to prevent overfitting: max_depth=3

Experiment with export_graphviz or dtreeviz for more advanced visualizations
