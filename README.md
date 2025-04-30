# 🍛 Bangla Food Image Classification Using CNN+BiLSTM / LSTM+BiLSTM

This project implements two deep learning models to classify Bangla food images using two architectures:
1. CNN + BiLSTM
2. LSTM + BiLSTM

---

## 🧠 Model 1: CNN + BiLSTM
🔧 Architecture
Conv2D (32 filters)

MaxPooling2D

Conv2D (64 filters)

MaxPooling2D

Conv2D (128 filters)

MaxPooling2D

Flatten

Dense (128 units, ReLU)

Dropout (0.5)

Reshape → (1, 128)

Bidirectional LSTM (128 units)

Dropout (0.5)

Dense (softmax output layer)

🏋️ Training Settings
Image size: 128x128

Batch size: 32

Epochs: 500

Optimizer: Adam (learning_rate=0.001)

Loss: categorical_crossentropy

📦 Output
Saved model: hybrid_cnn_bilstm_model.h5

Training and validation accuracy/loss plots

Test set evaluation

## 🧠 Model 2: LSTM + BiLSTM (No CNN)
🔧 Architecture
Reshape input to (128, 384)

LSTM (128 units, return_sequences=True)

Bidirectional LSTM (128 units)

Dropout (0.5)

Dense (128 units, ReLU)

Dropout (0.5)

Dense (softmax output layer)

🏋️ Training Settings
Same as Model 1.

## 📦 Output
Saved model: lstm_bilstm_model.h5

Training and validation accuracy/loss plots

Test set evaluation

## 🧪 Evaluation
Models are evaluated on:

Test Accuracy

Test Loss

