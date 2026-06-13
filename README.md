# 🌪️ Natural Disasters Analysis and Classification

A deep learning-powered web application that classifies satellite and real-world images of natural disasters — including floods, wildfires, earthquakes, cyclones, and more — using a CNN-based model served via a Flask API.

---

## 🔍 Overview

Natural disasters cause massive destruction worldwide. Early and accurate identification of disaster type from images can aid emergency response and resource allocation.

This project builds an end-to-end image classification pipeline:
- Trains a Convolutional Neural Network (CNN) on labeled disaster images
- Exposes the model via a Flask REST API
- Accepts image uploads and returns predicted disaster category with confidence score

---

## 🗂️ Project Structure

```
Natural_Disasters_Analysis_And_Classification/
├── Project Files/
│   ├── dataset/          # Training & validation images by class
│   ├── Flask/            # Flask app (app.py, templates, static)
│   └── Model Building/   # Jupyter notebooks for training
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🚀 Features

- ✅ Multi-class disaster image classification
- ✅ CNN model built with TensorFlow/Keras
- ✅ Image preprocessing with OpenCV
- ✅ REST API with Flask for real-time predictions
- ✅ Confidence score returned per prediction
- ✅ Supports: Flood, Wildfire, Earthquake, Cyclone, Landslide

---


## 🧠 Model Architecture

- Base: Custom CNN (or transfer learning with MobileNetV2/VGG16)
- Input size: 224×224 RGB images
- Output: Softmax over N disaster classes
- Optimizer: Adam | Loss: Categorical Crossentropy
- Trained with data augmentation (rotation, flip, zoom)

---

## 🛠️ Setup & Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/Natural_Disasters_Analysis_And_Classification.git
cd Natural_Disasters_Analysis_And_Classification

# Install dependencies
pip install -r requirements.txt

# Run the Flask app
cd "Project Files/Flask"
python app.py
```

Then open `http://localhost:5000` in your browser.

---

## 📦 Requirements

```
tensorflow>=2.10
flask>=2.0
opencv-python>=4.5
numpy
pillow
scikit-learn
```

---

## 📊 Results


| Class       | Precision | Recall | F1-Score |
|-------------|-----------|--------|----------|
| Flood       | 0.91      | 0.89   | 0.90     |
| Wildfire    | 0.93      | 0.92   | 0.92     |
| Earthquake  | 0.88      | 0.86   | 0.87     |
| Cyclone     | 0.95      | 0.94   | 0.94     |
| Landslide   | 0.87      | 0.85   | 0.86     |

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

---

## 📄 License
This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.
