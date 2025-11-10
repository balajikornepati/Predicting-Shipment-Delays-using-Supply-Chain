# Shipment Delay Prediction Using Machine Learning  
**Hybrid RF + LSTM Model with SHAP Explainability**

This repository contains the implementation and research artifacts for the MSc Data Analytics thesis project completed by **Balaji Kornepati**.  
The work focuses on predicting last-mile shipment delays using a **hybrid Random Forest + LSTM model**, enhanced with **SHAP** for model interpretability.

---

## 🌍 Problem Overview
Last-mile delivery is the most expensive and most delay-prone stage of logistics.  
Delays negatively affect:

- Customer satisfaction
- Operational efficiency
- Delivery network scheduling
- Transportation cost

This project uses machine learning to **predict whether a delivery will be delayed before it happens**, enabling proactive route planning, resource allocation, and service reliability.

---

## 🎯 Research Objectives

| Goal | Description |
|------|-------------|
| Predict delivery delays | Train ML and DL models on operational, temporal & weather data |
| Develop hybrid model | Combine Random Forest (feature learning) with LSTM (time sequences) |
| Improve transparency | Use **SHAP** to explain *why* model predicts delay |

---

## 🧠 Models Evaluated

| Model | Accuracy | Notes |
|------|---------|------|
| Random Forest | 82–84% | Strong baseline for structured features |
| XGBoost | 83–86% | Good precision, sensitive to tuning |
| MLP Neural Network | ~85% | Detects feature interactions |
| LSTM | High recall but more false positives | Captures time-based behavior |
| **Hybrid RF + LSTM (Final)** | **≈ 87% Accuracy, 0.89 Precision, 0.92 Recall, 0.90 F1** | **Best performance** ✅ |

> The hybrid model achieved the highest balanced performance and interpretability.

---

## 🔍 Key Features Used

- **Operational**: agent age, agent rating, delivery distance
- **Temporal**: order time, pickup time, delivery time duration
- **Environmental**: weather conditions (temp, wind, precipitation)
- **Traffic**: congestion level at delivery time

---

## 📊 Explainability (SHAP Results)

Top factors contributing to delay:

1. Traffic level
2. Delivery distance
3. Weather severity
4. Agent delivery performance characteristics

SHAP plots show **why** a specific delivery is predicted late, increasing trust in the model.

---



