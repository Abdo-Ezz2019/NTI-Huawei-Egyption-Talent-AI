

👕 Fashion MNIST - Image Classification with CNN (TensorFlow/Keras)
A deep learning model using Convolutional Neural Networks (CNNs) built with Keras to classify fashion items (e.g., shirts, shoes, bags) from the Fashion MNIST dataset.

📦 Dataset Info
60,000 training images

10,000 testing images

Image size: 28x28 grayscale

10 fashion classes:
0 = T-shirt/top
1 = Trouser
2 = Pullover
3 = Dress
4 = Coat
5 = Sandal
6 = Shirt
7 = Sneaker
8 = Bag
9 = Ankle boot

🧠 Model Architecture
Layer	Output Shape	Parameters
Conv2D (32 filters)	(26, 26, 32)	320
MaxPooling2D	(13, 13, 32)	0
Conv2D (64 filters)	(11, 11, 64)	18,496
MaxPooling2D	(5, 5, 64)	0
Conv2D (64 filters)	(3, 3, 64)	36,928
MaxPooling2D	(1, 1, 64)	0
Flatten	(64,)	0
Dense (ReLU)	(64,)	4,160
Dense (Softmax)	(10,)	650
Total Params		60,554

⚙️ Preprocessing
Normalization: Pixel values scaled to [0, 1]

One-hot Encoding: For categorical labels

Input Reshape: (28, 28) → (28, 28, 1) for Conv2D layers

📈 Training Results
Epochs: 10

Batch Size: 64

Optimizer: Adam (lr=0.001)

Loss Function: Categorical Crossentropy

Final Accuracy:

Training: ~91.6%

Validation: ~88.7%

📊 Accuracy Curve
A plot showing accuracy progression over epochs for both training and validation sets:

python
Copy
Edit
plt.plot(model.history.history['accuracy'])
plt.plot(model.history.history['val_accuracy'])
plt.title('Model Accuracy')
plt.xlabel('Epoch')
plt.ylabel('Accuracy')
plt.legend(['Train', 'Test'])
🧪 How to Use
bash
Copy
Edit
python fashion_mnist_cnn.py
Or run it in Google Colab or Jupyter Notebook for visualization.

📚 Notes
Can be extended with:

Dropout layers to reduce overfitting

BatchNormalization for better convergence

Data Augmentation using ImageDataGenerator

Try experimenting with different optimizers like SGD, RMSProp

 
