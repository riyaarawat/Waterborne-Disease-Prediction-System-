# Waterborne Disease Prediction System
An interactive Machine Learning-powered web application that predicts possible waterborne diseases based on user-selected symptoms. Built using Streamlit and a Random Forest Classifier, the system provides real-time disease predictions, confidence scores, risk categorization, and interpretable symptom importance insights.

## Features

1. **Symptom-Based Disease Prediction**

Select symptoms from an interactive multi-column checklist
Get instant predictions for possible waterborne diseases

2. **Confidence Score & Risk Analysis**

Displays prediction confidence percentages
Categorizes predictions into High Risk, Medium Risk, Low Risk

3. **Machine Learning Model**
Random Forest Classifier with:

    * 500 estimators
    * Class-weight balancing
    * Stratified train-test split
    * Hyperparameter tuning

* 📈 **Explainable AI**

  * Shows per-symptom feature importance
  * Helps users understand model decisions

* ⚙️ **Dynamic Prediction Threshold**

  * User-configurable confidence threshold slider
  * Filters low-confidence predictions

* 📦 **Optimized Performance**

  * Uses `@st.cache_data` to avoid redundant model retraining
  * Faster response times across sessions

* 📋 **Dataset Insights Dashboard**

  * Disease distribution visualization
  * Symptom inventory overview

* 🌐 **Production-Ready Deployment**

  * Configured with Gunicorn and runtime setup

---

## 🛠️ Tech Stack

* **Frontend & Deployment**

  * Streamlit
  * Gunicorn

* **Machine Learning**

  * Scikit-learn
  * Random Forest Classifier

* **Data Processing**

  * Pandas
  * NumPy

* **Visualization**

  * Matplotlib / Plotly (if applicable)

---

## 📂 Project Structure

```bash
Waterborne-Disease-Prediction-System/
│
├── app.py                  # Main Streamlit application
├── model/
│   └── trained_model.pkl   # Saved ML model
├── dataset/
│   └── disease_data.csv    # Dataset used for training
├── requirements.txt        # Project dependencies
├── runtime.txt             # Runtime configuration
├── Procfile                # Gunicorn deployment config
└── README.md
```

---

## ⚡ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/waterborne-disease-prediction-system.git
cd waterborne-disease-prediction-system
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

### 3️⃣ Activate Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Mac/Linux

```bash
source venv/bin/activate
```

### 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 5️⃣ Run the Application

```bash
streamlit run app.py
```

---

## 🧪 Machine Learning Workflow

1. Data preprocessing and symptom encoding
2. Stratified train-test split
3. Handling class imbalance using class weights
4. Hyperparameter tuning:

   * `n_estimators = 500`
   * `max_depth`
   * `min_samples_split`
5. Model training using Random Forest
6. Real-time inference through Streamlit UI

---

## 📊 Example Predictions

| Symptoms                  | Predicted Disease | Confidence |
| ------------------------- | ----------------- | ---------- |
| Fever, Vomiting, Diarrhea | Cholera           | 92%        |
| Abdominal Pain, Nausea    | Typhoid           | 85%        |


---

## 👨‍💻 Author

**Riya Rawat**
Machine Learning .......

---

## ⭐ Future Improvements

* Deep Learning-based prediction models
* Multi-language support
* Patient history integration
* Cloud database integration
* Mobile-responsive UI
* Docker containerization

