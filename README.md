# 🎭 Real-Time Face Detection & Emotion Reaction System

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?style=for-the-badge&logo=opencv)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=for-the-badge&logo=tensorflow)
![Accuracy](https://img.shields.io/badge/Accuracy-75%25-brightgreen?style=for-the-badge)

A real-time facial emotion recognition system built using Convolutional Neural Networks (CNN) and OpenCV. The system detects faces from a live webcam feed and classifies them into 7 distinct emotions with sub-100ms latency per frame.

---

## 🚀 Demo

> The system captures live video → detects faces → classifies emotion → displays result in real time.

---

## 🎯 Features

- ✅ Real-time face detection using OpenCV Haar Cascade
- ✅ 7-emotion classification: Happy, Sad, Angry, Surprise, Fear, Disgust, Neutral
- ✅ Trained on FER-2013 dataset (35,000+ labelled facial images)
- ✅ 75% classification accuracy
- ✅ Sub-100ms inference latency per frame
- ✅ Lightweight CNN architecture optimized for real-time use

---

## 🧠 Model Architecture

```
Input (48x48 grayscale image)
    ↓
Conv2D (32 filters) → BatchNorm → ReLU → MaxPool
    ↓
Conv2D (64 filters) → BatchNorm → ReLU → MaxPool
    ↓
Conv2D (128 filters) → BatchNorm → ReLU → MaxPool
    ↓
Flatten → Dense(256) → Dropout(0.5)
    ↓
Output: Softmax (7 classes)
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python 3.8+ | Core programming language |
| OpenCV | Face detection & video capture |
| TensorFlow/Keras | CNN model training & inference |
| NumPy | Array operations |
| Matplotlib | Training visualization |

---

## 📊 Dataset

- **Dataset:** FER-2013 (Facial Expression Recognition)
- **Total Images:** 35,887 labelled facial images
- **Image Size:** 48x48 pixels (grayscale)
- **Classes:** 7 emotions
- **Split:** 80% training / 20% validation

---

## ⚙️ Installation & Setup

```bash
# Clone the repository
git clone https://github.com/DhanushMasanam/emotion-detection.git
cd emotion-detection

# Install required packages
pip install -r requirements.txt

# Run the real-time detection
python detect_emotion.py
```

---

## 📦 Requirements

```
tensorflow>=2.0
opencv-python>=4.0
numpy>=1.19
matplotlib>=3.3
```

---

## 📈 Results

| Metric | Value |
|---|---|
| Training Accuracy | 78% |
| Validation Accuracy | 75% |
| Inference Speed | <100ms per frame |
| Model Size | ~15MB |

---

## 🔮 Future Improvements

- [ ] Improve accuracy using transfer learning (VGG16/ResNet)
- [ ] Add multi-face detection support
- [ ] Deploy as web application using Flask
- [ ] Add emotion history tracking and analytics

---

## 👨‍💻 Developer

**Dhanush M**
- 📧 dhanushmasanam@gmail.com
- 💼 [LinkedIn](https://linkedin.com/in/dhanush-masanam-69a745277)
- 🐙 [GitHub](https://github.com/DhanushMasanam)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
