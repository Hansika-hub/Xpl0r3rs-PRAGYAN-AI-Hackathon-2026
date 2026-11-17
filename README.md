# 🏥 Smart Triage -- AI-Powered Clinical Decision Support System

## Overview

Smart Triage is an advanced clinical decision support system that
combines Rule-Based Intelligence and Machine Learning to assess patient
risk in real time. It integrates Explainable AI (XAI) to provide
transparent, interpretable reasoning behind predictions, helping
clinicians make faster and more informed decisions.

## ✨ Key Features

-   **Hybrid AI Engine:** Combines a rule-based safety net for
    identifying immediate life-threatening conditions with an ML
    ensemble (XGBoost, LightGBM, CatBoost) for risk prediction.
-   **Explainable AI (XAI):** Uses SHAP to explain predictions and
    highlight the factors contributing to high-risk classifications.
-   **Dynamic Questioning:** Generates context-aware follow-up questions
    based on patients' initial symptoms.
-   **Multi-Modal Input:** Supports voice dictation, text input, and
    PDF/EHR uploads.
-   **Context-Aware NLP:** Uses TF-IDF vectorization to interpret
    symptom descriptions and distinguish severity.
-   **Relational Disease Mapping:** Provides interactive visualizations
    of relationships between correlated diseases.
-   **Multilingual Support:** Offers localized UI experiences for
    diverse patient populations.

## 🛠️ Technology Stack

### Frontend

-   React + Vite
-   Tailwind CSS
-   Framer Motion
-   Chart.js

### Backend

-   Python
-   FastAPI
-   Pydantic
-   Uvicorn

### Machine Learning & AI

-   Scikit-learn
-   XGBoost
-   LightGBM
-   CatBoost
-   SHAP
-   TF-IDF

## 📦 Installation

### Prerequisites

-   Node.js (v16+)
-   Python (v3.9+)
-   npm

### 1. Clone the Repository

``` bash
git clone https://github.com/StartUpUser/intelligent-triage-system.git
cd intelligent-triage-system
```

### 2. Backend Setup

``` bash
cd backend
python -m venv venv
```

Activate the virtual environment:

**Linux / macOS**

``` bash
source venv/bin/activate
```

**Windows**

``` bash
venv\\Scripts\\activate
```

Install dependencies and start the backend:

``` bash
pip install -r requirements.txt
python app.py
```

Backend server: `http://localhost:8000`

### 3. Frontend Setup

Open a new terminal:

``` bash
cd frontend
npm install
npm run dev
```

Frontend application: `http://localhost:5173`

## 🧠 Model Performance

The current model (v2.0) is optimized for high sensitivity to prioritize
the identification of potentially critical cases.

-   **High-Risk Recall:** 97%
-   **Approach:** Class weighting and oversampling to address class
    imbalance and improve detection of rare medical emergencies.

## ⚠️ Disclaimer

Smart Triage is a clinical decision support prototype and is not a
substitute for professional medical judgment, diagnosis, or emergency
medical care. Predictions should be reviewed by qualified healthcare
professionals.

## 🌱 Vision

To support safer and more efficient clinical decision-making through
intelligent risk assessment, transparent AI, and accessible healthcare
technology.
