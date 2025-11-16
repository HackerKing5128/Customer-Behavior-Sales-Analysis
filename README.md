# 🛒 Customer Behavior & Sales Analysis – Full Stack ML Project#1

This project analyzes customer behavior, segments customers using clustering, and predicts purchase likelihood using machine learning.  
It includes a **full-stack web dashboard** built with **React + Tailwind** and a **FastAPI/Flask backend** serving ML predictions.

---

## 🚀 Project Overview

This mini full-stack ML project combines:

- **Data Cleaning & Feature Engineering**  
- **PCA-based Customer Segmentation**  
- **K-Means Clustering**  
- **Classification Models for Purchase Prediction**  
- **Interactive Dashboard for Visualization**  
- **Backend API for Model Serving**

Datasets used (from Kaggle):

- [**Customer Personality Analysis**](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)
- [**Online Retail Dataset**](https://www.kaggle.com/datasets/carrie1/ecommerce-data)

---

## 📂 Project Structure

```
customer-behavior-ml-app/
│
├── ml-notebooks/           # Notebooks for full ML workflow
│   ├── 01_data_cleaning.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_pca_kmeans.ipynb
│   ├── 04_classification_models.ipynb
│   ├── 05_model_evaluation.ipynb
│   └── 06_export_model.ipynb
│
├── backend/                # FastAPI/Flask API backend
│   ├── main.py
│   ├── model.pkl
│   ├── scaler.pkl
│   ├── pca.pkl
│   ├── requirements.txt
│   └── utils/
│         ├── preprocessing.py
│         ├── evaluation.py
│         └── model_loader.py
│
├── frontend/               # React + Tailwind dashboard
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── tailwind.config.js
│
└── README.md
```
---

## 🧠 Machine Learning Features

### ✔️ 1. PCA for Dimensionality Reduction
- Reduce customer attributes to 2 key components  
- Visualize customer segments clearly  

### ✔️ 2. K-Means Clustering
- Segment customers based on purchasing behavior  
- Visualized on dashboard charts  

### ✔️ 3. Classification Models
The following models are trained and compared:

| Model | Purpose |
|-------|---------|
| Logistic Regression | Baseline prediction |
| Decision Tree | Non-linear learning |
| Naïve Bayes | Probabilistic classification |
| KNN | Distance-based classification |

### ✔️ 4. Model Evaluation
Models are evaluated using:
- Accuracy  
- F1-score  
- Confusion Matrix  
- Comparison Table  

---

## 🖥️ Frontend (React + Tailwind)

The dashboard includes:

- 📊 PCA scatter plot  
- 🟦 K-Means cluster visualization  
- 📈 Model comparison table  
- 📝 Customer input form for predictions  
- 🌙 Dark/Light theme toggle  
- 📱 Fully responsive layout  

Technologies:
- React.js  
- Tailwind CSS  
- Recharts / Chart.js  
- Axios  

---

## 🔧 Backend API (FastAPI)

The backend handles:

- Loading the trained ML model (pickle)  
- Preprocessing (scaling + PCA)  
- Predicting purchase likelihood  
- Exposing REST API endpoints:

### **`POST /predict`**
Input → Customer features  
Output → Purchase probability + label

---

## 🌐 Deployment (Recommended)

| Component | Platform |
|----------|----------|
| **Frontend** | Vercel / Netlify |
| **Backend** | Render / Railway / PythonAnywhere |
| **Model Files** | Stored in backend folder |

---


