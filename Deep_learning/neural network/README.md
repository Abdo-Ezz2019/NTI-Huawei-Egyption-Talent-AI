🔢 Handwritten Digit Recognition using Neural Network (MNIST)
This project demonstrates how to train a fully-connected neural network on the MNIST dataset using TensorFlow/Keras. It includes preprocessing, model training, and evaluation using confusion matrix and performance metrics.

📌 Project Features
✅ Load and preprocess MNIST dataset (grayscale 28x28 images)

✅ Normalize and flatten images for neural network input

✅ Build a multi-layer neural network using Dense layers

✅ Use sigmoid and softmax activation functions

✅ Evaluate accuracy and loss across epochs using custom callbacks

✅ Predict and visualize results using a confusion matrix

🔢 Dataset Overview
Training samples: 60,000

Test samples: 10,000

Image shape: 28x28 (grayscale)

Classes: Digits from 0 to 9

⚙️ Model Architecture
Layer	Type	Neurons	Activation
Input	Flatten (28×28) → 784	-	-
Dense	Hidden	50	Sigmoid
Dense	Hidden	50	Sigmoid
Dense	Output	10	Softmax

🧪 Training Results
Training Accuracy: ~99.6%

Test Accuracy (after training): ~99.3%

Initially the model had poor performance (accuracy ~10%) before training. After 10 epochs, it improved significantly.

📊 Confusion Matrix
The model was evaluated using a confusion matrix on the test set, which shows excellent classification performance across all digits.


(If exporting to GitHub, save the figure as an image and link it here.)

📈 Visualization
plt.imshow(x_train[0]): Display a handwritten digit

plt.hist(x_train[0]): Histogram showing pixel intensities

sns.heatmap(cm): Visual heatmap of confusion matrix

📦 Requirements
bash
Copy
Edit
pip install tensorflow numpy pandas matplotlib seaborn scikit-learn
▶️ How to Run
bash
Copy
Edit
python your_script_name.py
Replace your_script_name.py with the filename containing your code.

📚 Learning Objectives
Understand how to preprocess image data for neural networks

Use dense layers with different activations (sigmoid, softmax)

Track performance using callbacks and evaluate with confusion matrix

Identify performance bottlenecks and improve through normalization

📝 Notes
You can improve results further using CNN layers (Conv2D, MaxPooling2D)

Try ReLU instead of sigmoid for faster convergence

Use Dropout layers to reduce overfitting
