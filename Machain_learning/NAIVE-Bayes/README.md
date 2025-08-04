🧠 Text Classification using Naive Bayes (MultinomialNB)
This project demonstrates a text classification system using the Naive Bayes algorithm (MultinomialNB). It reads and concatenates multiple .csv files, preprocesses the text, and performs classification based on the content.

📁 Dataset Structure
Folder: /content/dataset/

Each file: .csv format with at least two columns:

CONTENT: the text data (e.g., movie reviews, articles)

CLASS: the target label/category

⚙️ Workflow Summary
Load Dataset:

Load and concatenate all .csv files in a directory

Handle potential empty directories or format errors

Split Data:

Split the dataset into train and test sets (80/20)

Vectorize Text:

Use CountVectorizer to convert raw text to numeric features

Remove English stop words

Model Training:

Train a Multinomial Naive Bayes (MultinomialNB) classifier

Evaluate:

Use accuracy_score to evaluate test performance

Predict class for new, unseen text

📦 Requirements
bash
Copy
Edit
pip install pandas numpy scikit-learn
▶️ How to Run
python
Copy
Edit
# 1. Ensure your dataset is in /content/dataset/
# 2. Each CSV should include 'CONTENT' and 'CLASS' columns
# 3. Run the script using Jupyter Notebook or any Python IDE
🧪 Sample Output
python
Copy
Edit
Accuracy: 0.89
Prediction for "i do not like this movies": ['negative']
🛠️ Troubleshooting
❌ Error: ValueError: No objects to concatenate
Solution:

Ensure that the folder /content/dataset contains .csv files

Each file must have a proper structure with CONTENT and CLASS columns

You can test with a single dummy CSV file to confirm

🔮 Future Improvements
Use TF-IDF Vectorizer for improved text weighting

Add support for Arabic text classification (with appropriate stop words)

Apply GridSearchCV for hyperparameter tuning

Support more ML algorithms (SVM, Random Forest)
