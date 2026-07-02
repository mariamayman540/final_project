# 🩺 AI Radiology Assistant

An end-to-end **Deep Learning** medical image diagnosis platform that assists healthcare professionals in analyzing multiple medical imaging modalities using state-of-the-art computer vision models and an AI-powered medical assistant.

The application supports:

- 🧠 Brain MRI Tumor Classification
- 🫁 Chest X-ray Pneumonia Detection
- 🫀 Chest CT COVID-19 Detection
- 🤖 Context-aware Medical AI Chat Assistant powered by Llama 3.3 (70B)

---

## 🚀 Live Demo

**Hugging Face Space:**
https://huggingface.co/spaces/PhilopateerSharl/radiology_assistant

---

## 📌 Features

- Multi-modal medical image analysis.
- Brain MRI tumor classification using EfficientNetB0.
- Chest X-ray pneumonia detection using EfficientNetB3.
- Chest CT COVID-19 detection using EfficientNetB4.
- Interactive Gradio web interface.
- AI medical assistant powered by Groq API (Llama 3.3 70B).
- Dynamic diagnostic cards with confidence scores.
- SVG-based probability visualization.
- Session history tracking.
- Responsive Light/Dark UI.

---

# 🏗️ System Architecture

The project consists of three main components:

### 1. Frontend

- Gradio
- HTML5
- CSS3
- SVG Visualization

### 2. AI Inference Engine

- TensorFlow
- Keras
- Transfer Learning
- EfficientNet Models

### 3. AI Medical Assistant

- Groq API
- Llama 3.3 (70B)

---

# 🧠 Deep Learning Models

| Scan Type   | Model          | Input Size | Task                   |
| ----------- | -------------- | ---------- | ---------------------- |
| Brain MRI   | EfficientNetB0 | 224×224    | 4-Class Classification |
| Chest X-Ray | EfficientNetB3 | 384×384    | Pneumonia vs Normal    |
| Chest CT    | EfficientNetB4 | 380×380    | COVID-19 vs Normal     |

---

# 🔄 Processing Pipeline

```text
User Upload
      │
      ▼
Image Preprocessing
      │
      ▼
Model Inference
      │
      ▼
Confidence Calibration
      │
      ▼
Diagnostic Results
      │
      ├── SVG Confidence Chart
      └── Medical AI Assistant
```

---

# ⚙️ Data Preprocessing

- RGB image conversion
- Image resizing
- EfficientNet preprocessing
- Pixel normalization
- Confidence calibration

Input resolutions:

- Brain MRI → 224 × 224
- Chest X-Ray → 384 × 384
- Chest CT → 380 × 380

---

# 📦 Tech Stack

### AI & Deep Learning

- TensorFlow
- Keras
- EfficientNet
- NumPy

### User Interface

- Gradio
- HTML5
- CSS3
- SVG

### AI Assistant

- Groq API
- Llama 3.3 (70B)

### Image Processing

- Pillow (PIL)

---

# 📂 Project Structure

```text
AI-Radiology-Assistant/
│
├── app.py
├── requirements.txt
├── README.md
│
├── models/
│   ├── brain_model.keras
│   ├── Pneumonia_EfficientNetB3_Inference.keras
│   └── covid_ct_model.keras
│
└── notebooks/
    ├── Brain_MRI_Classification.ipynb
    ├── Chest_Xray_Pneumonia_Classification_EfficientNetB3.ipynb
    └── Chest_CT_COVID_Classification.ipynb
```

---

# ▶️ Installation

Clone the repository

```bash
git clone https://github.com/mariamayman540/final_project.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

---

# 🔑 Environment Variables

Set your Groq API Key before running the application.

```bash
export GROQ_API_KEY="YOUR_API_KEY"
```

or create a `.env` file depending on your deployment platform.

---

# 📈 Model Outputs

Each prediction includes:

- Predicted Disease
- Confidence Score
- Diagnostic Severity
- AI-generated Medical Explanation
- Interactive Confidence Visualization

---

## 👥 Contributors

- **Mariam Ayman**
- **Philopateer Sharl**
- **Kerolos Farag**
- **Kermina Shenoda**
- **Sahrab Ehab**

---

## 📄 License

This project is intended for educational and research purposes only and is **not** a substitute for professional medical diagnosis.
