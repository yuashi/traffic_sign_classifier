# 🚦 Traffic Sign Classification using CNN

A deep learning-based Traffic Sign Classifier built using Convolutional Neural Networks (CNN) and a simple Tkinter GUI. This project classifies traffic signs into 43 categories.

---

## 📌 Features

- 🧠 CNN-based image classification model
- 🖼️ Supports image upload via GUI
- ⚡ Real-time prediction of traffic signs
- 🎯 43 traffic sign classes (GTSRB dataset)
- 🖥️ Simple and interactive Tkinter interface

---

## 🗂️ Project Structure

```
Traffic-Sign-Classifier/
│
├── dataset/
├── train.ipynb             # Model training
├── app.py                  # Tkinter GUI application
├── requirements.txt
└── README.md
```

---

## 🧠 Model Architecture

The CNN model consists of:

- 2 × Conv2D (32 filters, 5x5) + ReLU
- MaxPooling + Dropout
- 2 × Conv2D (64 filters, 3x3) + ReLU
- MaxPooling + Dropout
- Flatten layer
- Dense (256 neurons) + Dropout
- Output layer (43 classes, Softmax)

---

## 📊 Dataset

[German Traffic Sign Recognition Benchmark (GTSRB)](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)

---

## ⚙️ Installation

### 1. Clone the repository

```
git clone https://github.com/yuashi/traffic_sign_classifier.git
cd traffic_sign_classifier
```

### 2. Create virtual environment (recommended)

```
python -m venv .venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

### 3. Install dependencies

```
pip install -r requirements.txt
```

---

## ▶️ How to Run

### 1. Download the Dataset

Download the dataset, unzip and keep all the sub folders and files inside dataset/

### 2. Train the model

Run all the cells of train.ipynb in order. At the end you will have the trained model saved as **classifier.keras**

### 3. Run the GUI application

```
python app.py
```

---

## 🖥️ GUI Usage

1. Click **"Upload an Image"**
2. Select a traffic sign image
3. Click **"Classify Image"**
4. View prediction result instantly

---

## 🧪 Model Training Details

- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Epochs: 15
- Batch Size: 64
- Train-Test Split: 80-20

---

## 📈 Results

- Achieved high accuracy on test dataset ~ 95%
- Capable of correctly identifying most traffic signs

---

## 🚀 Future Improvements

- 🔄 Data augmentation for better generalization
- 📱 Convert to web app using Streamlit or Flask
- 🎥 Real-time traffic sign detection using webcam

---

## 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- PIL (Pillow)
- Tkinter

---

## 💻 Author

https://github.com/yuashi
