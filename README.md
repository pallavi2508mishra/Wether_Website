# Federated Unlearning using Medical Imaging

An implementation of **Federated Unlearning** for medical image analysis.  
This project demonstrates how a trained federated learning model can **remove the influence of a specific client’s data without retraining the entire model from scratch**.

The project focuses on medical imaging datasets (e.g., COVID-19 CT scans) and applies **FedEraser-based unlearning techniques** to ensure data privacy and compliance with data removal requests.

---

## 🚀 Overview

Federated Learning allows multiple institutions to collaboratively train machine learning models without sharing raw data.  
However, once a model is trained, removing a specific client’s contribution is difficult.

**Federated Unlearning** solves this problem by enabling:

- Removal of a client's data influence
- Privacy compliance (GDPR / right to be forgotten)
- Efficient model updates without full retraining

This project implements a **federated unlearning pipeline for medical imaging models**.

---

## 🧠 Key Concepts

- **Federated Learning**
- **Federated Unlearning**
- **FedEraser Algorithm**
- **Medical Image Classification**
- **Privacy-preserving AI**

---

## 📂 Project Structure

```
Federated-Unlearning-using-Medical-Imaging
│
├── Federated unlearning.ipynb      # Main notebook implementing the model
├── dataset/                       # Medical imaging dataset (not uploaded to repo)
├── models/                        # Saved trained models
├── results/                       # Evaluation outputs and plots
└── README.md
```

---

## 📊 Dataset

This project uses **medical imaging data (e.g., COVID-19 CT scan dataset)** for image classification.

Typical dataset structure:

```
dataset/
│
├── covid/
│   ├── img1.png
│   ├── img2.png
│
├── normal/
│   ├── img1.png
│   ├── img2.png
```

Datasets can be obtained from:

- Kaggle
- Medical imaging research repositories
- Open healthcare datasets

---

## ⚙️ Methodology

The pipeline consists of the following steps:

1. **Dataset preprocessing**
2. **Client data partitioning**
3. **Federated model training**
4. **Client contribution tracking**
5. **Federated unlearning using FedEraser**
6. **Model evaluation before and after unlearning**

---

## 🔬 Workflow

```
Medical Images
      ↓
Data Preprocessing
      ↓
Client Data Distribution
      ↓
Federated Training
      ↓
Model Aggregation
      ↓
Unlearning Request
      ↓
FedEraser Unlearning
      ↓
Updated Global Model
```

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/Federated-Unlearning-using-Medical-Imaging.git
cd Federated-Unlearning-using-Medical-Imaging
```

Install dependencies:

```bash
pip install -r requirements.txt
```

If requirements file is not available, install common packages:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow torch
```

---

## ▶️ Running the Project

Open the notebook:

```bash
jupyter notebook
```

Run:

```
Federated unlearning.ipynb
```

Follow the cells to:

- Train the federated model
- Simulate client participation
- Apply federated unlearning
- Evaluate results

---

## 📈 Expected Results

The model should demonstrate:

- Comparable accuracy before and after unlearning
- Successful removal of selected client contributions
- Reduced retraining cost compared to full retraining

Metrics used:

- Accuracy
- Precision
- Recall
- F1 Score

---

## 🛡️ Applications

Federated Unlearning is useful in:

- Healthcare AI
- Privacy-sensitive datasets
- GDPR compliance
- Collaborative hospital AI systems

---

## 📚 References

1. **FedEraser: Enabling Efficient Client-Level Data Removal from Federated Learning Models**
2. Research on Federated Learning for Medical Imaging
3. Privacy-Preserving Machine Learning

---

## 👩‍💻 Contributors

- Pallavi Mishra

---

## 📜 License

This project is open source and available under the **MIT License**.

---

## ⭐ Acknowledgment

This project was developed as part of a research study on **Federated Unlearning in Medical Imaging Systems**.
