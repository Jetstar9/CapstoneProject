# Facial Emotion Recognition with CNN  
*MIT Applied Data Science Capstone Project*

## 🧠 Overview
This project applies deep learning and computer vision techniques to classify human facial emotions from images. Using Convolutional Neural Networks (CNNs), the model detects one of four emotions:

- Happy  
- Sad  
- Neutral  
- Surprise

The project explores multiple CNN architectures and transfer learning approaches to determine which performs best on real-world emotion data.

---

## 📊 Dataset
- **Source:** [FER2013 Dataset (Kaggle)](https://www.kaggle.com/datasets/msambare/fer2013)
- Focused subset of 4 emotional categories for multi-class classification
- Grayscale and RGB input channels tested

---

## 🛠️ Technologies & Tools
- Python  
- TensorFlow / Keras  
- CNNs (Sequential API)  
- Transfer Learning (VGG16, ResNet20V2, EfficientNetB0)  
- Matplotlib, Sklearn (for evaluation)

---

## 🔍 Model Development Workflow

### 1. **Data Preparation**
- Used `tf.image_from_file` data loaders  
- Data normalization (within Sequential pipeline)  
- Data augmentation applied via custom Keras preprocessing  
- One-hot encoded labels for multi-class classification  

### 2. **Model Selection & Compilation**
- Evaluated 7 models: baseline CNN, RGB CNN, VGG16, ResNet20V2, EfficientNetB0, and custom model ("Derek's Model")  
- Used ReLU activations, Conv2D layers, MaxPooling, Flatten, Dense output  
- Adjusted parameters for transfer learning (freezing/unfreezing layers)

### 3. **Training**
- Used callbacks (EarlyStopping, ModelCheckpoint)  
- Saved model weights  
- Logged training history for visualization  

### 4. **Evaluation**
- Accuracy and loss plots (training/validation curves)  
- Confusion matrix on test set  
- Classification report (precision, recall, F1)

---

## 📈 Results
[Capstone Presentation - Facial Recognition.pdf](https://github.com/user-attachments/files/21536650/Capstone.Presentation.-.Facial.Recognition.pdf)


