# 📉 Customer Churn Prediction App

A Machine Learning–powered web application that predicts whether a customer is likely to **churn** (leave a service) based on their demographic, account, and usage details.

This project demonstrates an **end-to-end ML workflow**: data preprocessing, model training, serialization, and deployment using a web framework.

---

## 🚀 Features

* Predicts **customer churn (Yes/No)**
* Uses **Machine Learning classification model**
* Handles **categorical & numerical features** using preprocessing pipelines
* Clean and simple **web interface**
* Scalable and production-ready structure

---

## 🧠 Machine Learning Workflow

1. **Data Cleaning & Preprocessing**

   * Handling missing values
   * Encoding categorical variables (One-Hot Encoding)
   * Feature scaling using StandardScaler

2. **Model Training**

   * Algorithm used: `Logistic Regression / Random Forest / XGBoost` *(configurable)*
   * Model evaluation using accuracy, precision, recall

3. **Pipeline Creation**

   * `ColumnTransformer` for numerical & categorical columns
   * End-to-end `Pipeline` to avoid data leakage

4. **Model Serialization**

   * Trained model saved using `pickle`

5. **Deployment**

   * Flask-based backend
   * HTML templates for UI

---

## 🛠️ Tech Stack

* **Programming Language**: Python
* **Libraries**:

  * pandas
  * numpy
  * scikit-learn
  * pickle
* **Web Framework**: Flask
* **Frontend**: HTML, CSS (optional Bootstrap)

---

## 📂 Project Structure

```
churn-app/
│
├── model/
│   └── churn_model.pkl
│
├── templates/
│   └── index.html
│
├── static/
│   └── style.css
│
├── application.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/churn-prediction-app.git
cd churn-prediction-app
```

### 2️⃣ Create Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application

```bash
python application.py
```

Open browser and go to:

```
http://127.0.0.1:5000/
```

---

## 📥 Input Parameters

The model expects the following customer details:

* Gender
* Senior Citizen
* Partner
* Dependents
* Tenure
* Phone Service
* Internet Service
