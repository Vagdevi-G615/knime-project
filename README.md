# 🌾 Smart Farming: Crop Recommendation Using Machine Learning (KNIME Workflow)

## 📌 Project Overview
This project focuses on developing a crop recommendation system using environmental and soil features such as nitrogen (N), phosphorus (P), potassium (K), temperature, humidity, pH, and rainfall. Multiple machine learning models were trained and compared to identify the most suitable crop based on the given conditions.

## 📁 Dataset
- Source: Kaggle – [Crop Recommendation Dataset](https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset)
- Features:
  - `N`, `P`, `K` – Soil macronutrients
  - `Temperature`, `Humidity` – Weather conditions
  - `pH`, `Rainfall` – Soil chemistry and climate
  - `label` – Target crop class (multi-class classification)

## 🧰 Tools & Environment
- **KNIME Analytics Platform**
- Built-in Learner/Predictor Nodes:
  - Random Forest
  - Naive Bayes
  - Decision Tree
  - k-Nearest Neighbors (KNN)
- **WEKA Integration**:
  - MultiClassClassifier using Weka Predictor

## 🔗 Workflow Highlights
- **Missing Value Handling**: Most Frequent / Mean / Median
- **Normalization**: Min-Max Scaling
- **Partitioning**: Stratified 80% train / 20% test
- **Prediction Comparison**: Scorer node for evaluation

## 🤖 Model Comparison Results

| Model                  | Accuracy     |
|------------------------|--------------|
| 🔍 K-Nearest Neighbors (KNN)        | **97.50%**     |
| 🌲 Random Forest                    | **99.545%**    |
| 🧮 Naive Bayes                      | **99.545%**    |
| 🌳 Decision Tree                    | **97.50%**     |
| 🎯 MultiClassClassifier (Weka)      | **95.227%**    |

> 🔬 Random Forest and Naive Bayes performed the best, achieving nearly 99.5% accuracy.

## 📦 Output Files
- Evaluation metrics from `Scorer` 

## 📈 Future Enhancements
- Deploy this model using **KNIME WebPortal** or **Streamlit**
- Integrate with **real-time weather APIs**
- Add **geolocation-based crop filtering**
- Explainable AI using **LIME** or **SHAP** nodes

## 📄 License
This project is for academic and research purposes. Dataset © Kaggle contributors.
