# 🏥 HeartSmart AI: Predicting Cardiovascular Risk with ML

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-360/)
[![Flask](https://img.shields.io/badge/flask-%23000.svg?style=flat&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)

![Heart Disease Dashboard](assets/dashboard_screenshot.png)

## 📌 Objective

**HeartSmart AI** is a machine learning-powered application designed to assess an individual's risk of cardiovascular disease (CVD). By analyzing key lifestyle, demographic, and clinical factors—such as BMI, smoking habits, physical activity, and diabetes status—the system provides an instant risk probability score.

This project aims to demonstrate the power of **Early Detection** and **Preventive Healthcare** through accessible AI technology, leveraging a robust **Random Forest Classifier** trained on over 900,000 health records.

## 📁 Project Structure

```bash
Predict-Heart-Disease/
│
├── frontend/               # Frontend Application Logic
│   ├── src/
│   │   ├── app.py          # Main Flask Application
│   │   ├── db.py           # Database Connection Logic
│   │   ├── templates/      # HTML Templates (UI)
│   │   └── static/         # CSS/JS Assets
│   └── __init__.py
│
├── assets/                 # Project Assets (Visuals)
│   └── dashboard_screenshot.png
│
├── models/                 # ML Models (Auto-downloaded)
│   └── Random_forest.pkl   # Trained Model (Ignored in Git)
│
├── render.yaml             # Render Deployment Config
├── requirements.txt        # Python Dependencies
├── run.bat                 # Windows Start Script
└── README.md               # Project Documentation
```

## 🧠 Features Used

The model uses **21 Key Indicators** to predict heart disease risk, including:

*   **Demographics**: Age, Sex, Education, Income
*   **Vitals**: BMI (Body Mass Index)
*   **Medical History**: High Blood Pressure, High Cholesterol, Stroke, Diabetes
*   **Lifestyle**: Smoker, Alcohol Consumption, Physical Activity, Diet (Fruits/Veggies)
*   **Health Status**: General Health, Mental Health, Physical Health, Difficulty Walking
*   **Access**: Any Healthcare, Doctor Cost Concerns

## ⚙️ Tech Stack

*   **Python 3.x**: Core logic and scripting.
*   **Flask**: Web framework for the application.
*   **Scikit-Learn**: Machine Learning model implementation (Random Forest).
*   **Pandas & NumPy**: Data processing and manipulation.
*   **MySQL**: Database for storing user predictions (optional integration).
*   **Render**: Cloud platform for deployment.

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/YourUsername/Predict-Heart-Disease.git
cd Predict-Heart-Disease
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Application

**Windows:**
Double-click `run.bat` or run:
```bash
python frontend/src/app.py
```

**Mac/Linux:**
```bash
python3 frontend/src/app.py
```

Visit **http://127.0.0.1:10000** in your browser.

## 🎥 Live Demo
render live : https://predict-heart-disease-fn9m.onrender.com

> **Note**: The application will automatically download the trained `Random_forest.pkl` model from Google Drive on the first run.

## 📈 Evaluation

The **Random Forest Classifier** was selected for its high accuracy and ability to handle complex, non-linear relationships in medical data.

*   **Input Data**: BRFSS 2015 dataset (approx. 400k records)
*   **Preprocessing**: Cleaning, normalization, and feature encoding.
*   **Metric**: The model focuses on minimizing false negatives to ensure high sensitivity in detecting potential heart risks.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
