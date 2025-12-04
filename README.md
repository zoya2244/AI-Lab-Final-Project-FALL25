# AI Fake Image Detection

**AI-Lab Final Project — Fall 2025**

---

## 📌 Overview

This project focuses on detecting whether an image is real or artificially generated. With the rapid growth of AI-based image-generation tools and digital editing techniques, it has become increasingly difficult to rely on visual content as proof of authenticity. The goal of this project is to design a model that can analyze an image and classify it as **Real** or **Fake** using machine learning methods.

The system is simple to use, lightweight, and demonstrates how deep learning can be applied to the problems of misinformation, digital manipulation, and media forensics.

---

## 🎯 Objective

The purpose of this project is to build an automated image-classification system capable of identifying patterns typically found in:

* AI-generated images (GAN-generated)
* Deepfake-style content
* Edited or manipulated visuals
* Naturally captured real images

This project shows how machine learning helps strengthen digital trust and protect against misleading visual content.

---

## ✨ Features

* **Real vs Fake Image Classification**
  Uses a pre-trained model (`ai_detector_1100.h5`) to classify any input image.

* **Beginner-Friendly Scripts**
  `project.py` and `testing.py` can be run easily without modifying the code structure.

* **Dataset Support**
  A dataset folder is included for retraining or experimentation.

* **Lightweight & Fast**
  Model runs smoothly even on normal hardware without heavy GPU requirements.

* **Extensible Design**
  Can be expanded with more datasets, improved architectures, or web-based interfaces.

---

## 📂 Project Structure

```
AI-Lab-Final-Project-FALL25/
│
├── dataset/                 # Training and testing images (Real & Fake)
├── ai_detector_1100.h5      # Pretrained machine learning model
├── project.py               # Main detection script
├── testing.py               # Script for testing the model
├── .gitattributes           # Git configuration file
└── README.md                # Project documentation
```

---

## 🚀 Installation & Setup

Follow the steps below to run the project on your system:

### 1. Clone the repository

```bash
git clone https://github.com/zoya2244/AI-Lab-Final-Project-FALL25.git
cd AI-Lab-Final-Project-FALL25
```

### 2. (Optional) Create a virtual environment

```bash
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # macOS/Linux
```

### 3. Install required dependencies

(If you have `requirements.txt`, run this:)

```bash
pip install -r requirements.txt
```

Otherwise install manually:

* TensorFlow / Keras
* OpenCV
* NumPy
* PIL (Pillow)

---

## ▶️ How to Use

### **To detect an image (main script):**

```bash
python project.py
```

Inside the script, you can choose or modify the input image path.

### **To test the model using test samples:**

```bash
python testing.py
```

The script loads the pretrained model, analyzes the image, and prints the result as either:

```
Real Image
```

or

```
Fake Image
```

---

## 🔍 How It Works

1. An input image is preprocessed (resized, normalized).
2. The trained model (`ai_detector_1100.h5`) extracts visual features.
3. The model compares features with patterns it learned from training data.
4. A probability score is generated.
5. The system classifies the image as **Real** or **Fake**.

This demonstrates how convolutional neural networks identify subtle details in textures, noise patterns, and inconsistencies that often appear in AI-generated or manipulated content.

---

## 📊 Future Improvements

This project can be expanded with:

* A larger and more diverse training dataset
* Web or mobile-based interface for instant detection
* More advanced model architectures
* Explainability features (e.g., Grad-CAM visualizations)
* Support for additional fake image types

---

## 👤 Author

**Zoya**
AI-Lab Final Project — Fall 2025
GitHub: [zoya2244](https://github.com/zoya2244)

---



If you have any questions or want help improving the project, feel free to reach out!
