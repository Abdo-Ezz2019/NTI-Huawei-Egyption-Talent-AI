🧠 Activation Functions Visualizer
This project provides a hands-on implementation and visualization of popular activation functions used in neural networks. It’s designed to help beginners and intermediate learners understand how different functions behave mathematically and visually.

📌 Features
✅ Custom implementation of key activation functions:

Sigmoid

Tanh

ReLU

Leaky ReLU

Softmax

Swish

📈 Visualization of function outputs and their derivatives (where applicable)

🖼️ Simple image normalization using activation functions

🧪 Built using NumPy, Matplotlib, and Pandas

🧩 Activation Functions Implemented
Function	Description
my_sigmode(x)	Returns: \( \frac{1}{1 + e^{-x}} \)
my_tanh(x)	Returns: \( \tanh(x) \)
my_relu(x)	Returns: \( \max(0, x) \)
my_leaky_relu(x)	Returns: \( \max(0.01x, x) \)
my_softmax(x)	Returns: softmax values for vector x
my_swish(x)	Returns: \( x \cdot \text{sigmoid}(x) \)

📚 Use Case
Useful for:

Students learning deep learning

Visualizing how activation functions work

Comparing function outputs for model design

📝 Notes
The Softmax function is applied to a vector, not a single value, so it behaves differently in plots.

All functions are implemented manually using NumPy for better educational understanding.

