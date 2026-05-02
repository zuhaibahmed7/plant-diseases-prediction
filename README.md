# 🌿 Plant Disease Prediction

A deep learning web application that predicts plant diseases from uploaded images. Built with TensorFlow and Streamlit, this app allows users to upload a photo of a plant leaf and instantly get a prediction of the disease affecting it.

---

## 📌 Introduction

Plant diseases are a major threat to agriculture and food security. This project uses a trained Convolutional Neural Network (CNN) model to identify plant diseases from leaf images. The goal is to help farmers and researchers quickly diagnose plant health issues using AI.

This is a university/college group project built using Python, TensorFlow, and Streamlit.

---

## 🛠️ Technologies Used

- Python 3.11
- TensorFlow 2.17.0
- Streamlit 1.40.0
- NumPy 1.26.4
- Pillow 10.4.0
- Docker

---

## ⚙️ Installation

### Prerequisites
Make sure you have the following installed:
- [Python 3.11](https://www.python.org/downloads/release/python-3119/)
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- Git

### Clone the Repository
```bash
git clone https://github.com/zuhaibahmed7/plant-diseases-prediction.git
cd plant-diseases-prediction
```

### Download the Model
Download the trained model file `plant_disease_prediction_model.h5` and place it in:
```
app/trained_model/plant_disease_prediction_model.h5
```

### Install Dependencies
```bash
cd app
py -3.11 -m pip install -r requirements.txt
```

---

## 🚀 How to Run

### Option 1 — Run Locally
```bash
cd app
py -3.11 -m streamlit run main.py
```
Then open your browser at: `http://localhost:8501`

### Option 2 — Run with Docker
**Build the image:**
```bash
cd app
docker build -t plant-diseases-prediction-images:v1.0 .
```

**Run the container:**
```bash
docker run -p 80:80 plant-diseases-prediction-images:v1.0
```

Then open your browser at: `http://localhost:80`

---

## 📂 Project Structure

```
AI Project/
├── app/
│   ├── trained_model/          # Trained model (.h5 file)
│   ├── test_images/            # Sample test images
│   ├── main.py                 # Main Streamlit app
│   ├── requirements.txt        # Python dependencies
│   ├── Dockerfile              # Docker configuration
│   ├── config.toml             # Streamlit config
│   └── credentials.toml        # Streamlit credentials
├── model_training_notebook/    # Jupyter notebook for model training
└── README.md
---

## 📜 License

This project is for educational purposes only.
