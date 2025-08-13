

# 🧠 Brain Tumor Detection Web App (Django + TensorFlow)

## 📌 Overview

This is a **Brain Tumor Detection Web Application** that uses **Deep Learning** to analyze MRI scans and detect the presence of brain tumors.
The project integrates:

* **TensorFlow/Keras** → For building and training the CNN model
* **Django** → For the backend logic and routing
* **HTML/CSS** → For the frontend user interface

The app allows users to upload an MRI scan image and get **instant predictions** — either **"Tumor Detected"** or **"No Tumor"**.

---

## 🎯 Motivation

Early detection of brain tumors can significantly improve treatment outcomes. This project demonstrates how **AI and medical imaging** can work together to assist healthcare professionals and provide accessible diagnostic tools.

---

## 🚀 Features

* 📤 **Image Upload** – Upload `.jpg`, `.jpeg`, or `.png` MRI scans
* ⚡ **Real-time Prediction** – Instant results using a trained deep learning model
* 🎯 **High Accuracy** – Trained on labeled MRI images
* 🌐 **Web-based Interface** – No technical skills required for usage
* 🔍 **Scalable** – Can be deployed locally or on the cloud

---

## 🧠 Workflow

1. **Image Upload** – User uploads MRI scan via browser
2. **Preprocessing** – Image resized to **150x150**, normalized (0–1 scale)
3. **Prediction** – CNN model predicts tumor presence
4. **Result Display** – Output is shown on the webpage

---

## 📂 Project Structure

```
brain_tumor_detection/
│── sss/
│   └── brain_tumor_detection_model.h5   # Pre-trained CNN model
│── templates/
│   └── predict.html                      # Frontend template
│── views.py                               # Prediction logic
│── urls.py                                # URL configuration
│── settings.py                            # Django settings
│── manage.py                              # Django entry point
│── README.md                              # Project documentation
```

---

## 📊 Dataset

The CNN model was trained on a **Brain MRI Dataset** containing two classes:

* **Tumor Detected** 🧠
* **No Tumor** ✅

Dataset preparation steps:

* Resized all images to **150×150 pixels**
* Normalized pixel values to range **\[0, 1]**
* Split into **training, validation, and test sets**

---

## 🧠 Model Details

* **Architecture:** Convolutional Neural Network (CNN)
* **Layers:** Conv2D → MaxPooling → Flatten → Dense → Output
* **Input Shape:** 150×150×3
* **Loss Function:** Binary Crossentropy
* **Optimizer:** Adam
* **Metrics:** Accuracy

---

## ⚙️ Installation & Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/brain-tumor-detection.git
cd brain-tumor-detection

# Create a virtual environment
python -m venv venv

# Activate virtual environment
venv\Scripts\activate     # Windows
source venv/bin/activate  # Mac/Linux

# Install dependencies
pip install -r requirements.txt

# Run Django server
python manage.py runserver
```

Open browser → **[http://127.0.0.1:8000/](http://127.0.0.1:8000/)**

---

## 📸 Usage

1. Start the Django server
2. Open the web app in your browser
3. Upload an MRI scan image
4. Click **Predict**
5. View the result instantly

---

## 📈 Results & Accuracy

* Achieved high accuracy on test dataset
* Model performs well on unseen MRI scans
* Prediction speed is optimized for quick results

---

## 🔮 Future Improvements

* Multi-class tumor type classification (e.g., glioma, meningioma, pituitary)
* Heatmap visualization of tumor areas (Grad-CAM)
* REST API for integration with other systems
* Mobile-friendly version

---

## 🤝 Contribution Guidelines

Want to contribute?

1. Fork the repository
2. Create a new branch (`feature-xyz`)
3. Commit changes
4. Push to branch
5. Open a Pull Request


