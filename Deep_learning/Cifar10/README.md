🧠 CIFAR-10 Image Classification with CNN
This project demonstrates a basic yet effective implementation of a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset, which contains 60,000 32×32 color images in 10 different classes.

📌 Features
✅ Loads and preprocesses CIFAR-10 dataset

✅ Builds a CNN using TensorFlow & Keras

✅ Normalizes image data and converts labels to one-hot encoding

✅ Implements early stopping to avoid overfitting

📈 Tracks training and validation accuracy through graphs

🧩 Model Architecture
Layer	Type	Output Shape
Conv2D (32 filters, 3x3)	ReLU	(30, 30, 32)
MaxPooling2D (2x2)	-	(15, 15, 32)
Conv2D (64 filters, 3x3)	ReLU	(13, 13, 64)
MaxPooling2D (2x2)	-	(6, 6, 64)
Flatten	-	(2304,)
Dense (x5)	Sigmoid	(128,)
Output Dense	Sigmoid	(10,)

🔧 Optimizer: Adam
📉 Loss Function: Categorical Crossentropy
📊 Evaluation Metric: Accuracy

🔢 Dataset Overview
python
Copy
Edit
x_train shape: (50000, 32, 32, 3)  
y_train shape: (50000, 1)  
x_test shape: (10000, 32, 32, 3)  
y_test shape: (10000, 1)
📦 Dependencies
bash
Copy
Edit
pip install numpy pandas matplotlib tensorflow scikit-learn
▶️ How to Run
bash
Copy
Edit
python your_script_name.py
Replace your_script_name.py with the actual filename.

🧪 Training Results
The model was trained for 10 epochs with early stopping enabled. Below are some highlights:

Final Training Accuracy: ~74.9%

Final Validation Accuracy: ~64.7%

Loss decreased steadily across epochs

Model avoids overfitting using EarlyStopping callback.

📊 Training vs Validation Accuracy:

(insert if exporting to markdown + image folder)

📚 Useful For:
Beginners learning CNN concepts

Visualizing training history

Building simple image classifiers

Exploring activation functions like ReLU and Sigmoid

📌 Notes
You can experiment with different activation functions (e.g., ReLU vs Sigmoid).

Try adding Dropout layers to further reduce overfitting.

The model uses sigmoid in the output layer, which is uncommon for multi-class classification (usually softmax is used).
