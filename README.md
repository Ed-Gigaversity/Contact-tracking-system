
# 🧬 Contact-Tracing-System

A Machine Learning-based solution to identify and assess the risk of disease transmission based on proximity data and interaction patterns — helping automate and scale contact tracing efforts during infectious disease outbreaks like COVID-19.

---

## 📌 Introduction

Contact tracing is essential in managing infectious disease outbreaks. This project presents a **Contact Tracing System** that applies machine learning techniques to analyze proximity and interaction data between individuals. The goal is to **assess exposure risk**, **identify transmission chains**, and issue **real-time alerts** to prevent the spread of diseases.

By leveraging data such as GPS/Bluetooth signals, timestamps, and contact duration, this system can support public health strategies with predictive intelligence — all while preserving user privacy.

---

## 🎯 Objectives

- 🧠 Build a system that identifies high-risk exposure based on contact history.
- 📡 Analyze proximity, frequency, and duration of contacts to predict infection risk.
- 🔐 Ensure data privacy and security in handling sensitive health information.
- 🤖 Use ML models to classify contacts into **High Risk** or **Low Risk** categories.
- ⏱️ Provide real-time alerts to individuals likely exposed.

---

## 📊 Dataset Description

The model is trained on **real-world or simulated data**, which typically includes the following features:

| Feature              | Description                                         |
|----------------------|-----------------------------------------------------|
| `user_id`            | Unique identifier for each person or device         |
| `timestamp`          | Date and time of interaction                        |
| `location_data`      | GPS or Bluetooth-based location coordinates         |
| `contact_duration`   | Time spent in close contact                         |
| `proximity_distance` | Estimated distance between individuals (in meters)  |
| `infection_status`   | Label: 1 = infected, 0 = not infected               |
| `contact_frequency`  | Number of unique interactions per day/week          |

This is modeled as a **binary classification problem**:
- **Output**: Predict whether a user is at **High Risk** (1) or **Low Risk** (0) of infection.

---

## 🛠️ ML Techniques & Pipeline

- Data Preprocessing: handling missing values, normalizing distances and time
- Feature Engineering: encoding timestamps, distance thresholds, clustering contacts
- Model Training: Logistic Regression, Random Forest, or XGBoost classifiers
- Evaluation: Accuracy, Precision, Recall, F1-Score
- Real-time risk prediction and alerting system (optional extension)

---

## 🔐 Privacy & Security

- All data is anonymized.
- Device/user IDs are hashed or tokenized.
- No personally identifiable information (PII) is stored.
- Bluetooth-only mode can be enabled to avoid GPS tracking.


---

## 🚀 Future Enhancements

- Integration with real-time mobile tracking via BLE
- Exposure notifications through SMS/email
- Heatmaps of high-contact zones
- Federated learning for privacy-preserving model training

---

## 👨‍⚕️ Use Cases

- Government health departments for outbreak control
- Hospitals and campuses for internal contact tracing
- Organizations managing workforce safety

---

## clone repository
```bash
git clone https://github.com/Ed-Gigaversity/Contact-tracking-system.git
```

## change directory
```bash
cd Contact_Tracing_System_Using_ML
```
**Credits**
- numpy
- pandas
- matplotlib
- seaborn
- sklearn
- folium
