
# 🍎 Fruits CNN Classifier

A deep learning project that classifies fruit images using a Convolutional Neural Network (CNN) built with TensorFlow/Keras. The model is trained on the Fruits-360 dataset and can predict the type of fruit from an uploaded image.

---

## 🚀 Features

* 📦 Automatic dataset download using KaggleHub
* 🧠 CNN-based image classification model
* 🔄 Data augmentation for better generalization
* 📊 Training & validation performance visualization
* 💾 Model saving (`.keras` format)
* 🖼️ Custom image prediction with confidence score

---

## 🛠️ Tech Stack

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Pillow
* KaggleHub

---

## 📂 Project Structure

```
├── train.py / notebook.ipynb   # Main training & prediction code
├── fruit_model.keras           # Saved trained model
├── output.png                  # Training graphs / predictions
├── kaggle.json                 # Kaggle API key (not included in repo)
└── README.md                   # Project documentation
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/fruits-cnn-classifier.git
cd fruits-cnn-classifier
```

### 2️⃣ Install Dependencies

```bash
pip install tensorflow matplotlib numpy pillow kagglehub
```

### 3️⃣ Add Kaggle API Key

* Download `kaggle.json` from your Kaggle account
* Place it in the project directory

---

## 📥 Dataset

The dataset is automatically downloaded using KaggleHub:

* Dataset: **Fruits-360**
* Contains multiple fruit categories with labeled images

---

## 🧠 Model Architecture

* Conv2D → MaxPooling
* Conv2D → MaxPooling
* Conv2D → MaxPooling
* Flatten
* Dense (256 units)
* Dropout (0.5)
* Output Layer (Softmax)

---

## 🏋️ Training

```python
model.fit(
    train_gen,
    validation_data=val_gen,
    epochs=EPOCHS,
    callbacks=[EarlyStopping(patience=2, restore_best_weights=True)]
)
```

---

## 📊 Evaluation

* Accuracy and loss graphs are generated and saved as `output.png`
* Model performance is evaluated on test data

---

## 💾 Save Model

```python
model.save("fruit_model.keras")
```

---

## 🔍 Prediction

Upload an image and get predictions:

```python
predict_fruit("image.jpg")
```

Output:

* Predicted fruit label
* Confidence score
* Visualization of result

---

## 📸 Example Output

```
🍎 Apple (98.3%)
```


## 👨‍💻 Author

Developed by **Chanaksh Choudhari**


## 📌 Future Improvements
- Add transfer learning (ResNet, MobileNet)
- Deploy using Flask/Streamlit
- Add real-time camera prediction

---
