# 🍎 Fruits CNN Classifier

A deep learning project that classifies fruit images using Convolutional Neural Networks (CNN).

## 🚀 Features
- Multi-class fruit classification
- Built using TensorFlow/Keras
- Uses Fruits-360 dataset

## 📂 Dataset
Download from:
https://www.kaggle.com/moltean/fruits

Place inside:
dataset/fruits-360_100x100/

## ▶️ Run Project

### 1. Install dependencies
pip install -r requirements.txt

### 2. Train model
cd src
python train.py

### 3. Predict
python predict.py

## 🧠 Model Architecture
- Conv2D + MaxPooling layers
- Fully connected dense layers
- Softmax output

## 📊 Accuracy
~90%+ depending on epochs

## 📌 Future Improvements
- Add transfer learning (ResNet, MobileNet)
- Deploy using Flask/Streamlit
- Add real-time camera prediction

---