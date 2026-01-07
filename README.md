# Satellite Imagery Based Property Valuation

## 📌 Overview
This project builds a multimodal regression pipeline to predict property prices using:
1. Tabular housing attributes
2. Satellite imagery fetched using geographic coordinates

The objective is to enhance traditional valuation models by incorporating visual environmental context.

---

## 📂 Dataset
- train(1).xlsx — contains target column `price`
- test2.xlsx — contains features only

---

## 🧠 Methodology
1. Exploratory Data Analysis (EDA)
2. Feature Engineering
3. Baseline Regression Models
4. XGBoost on Tabular Data
5. Satellite Image Acquisition using Mapbox API
6. CNN Feature Extraction (ResNet50)
7. Multimodal Feature Fusion
8. Final Model Evaluation

---

## 🏗️ Project Structure
- `data_fetcher.py` — downloads satellite images
- `preprocessing.ipynb` — EDA and feature engineering
- `model_training.ipynb` — model training and evaluation
- `outputs/enrollno_final.csv` — final predictions
- `outputs/enrollno_report.pdf` — project report

---

## ⚙️ Setup Instructions
```bash
pip install -r requirements.txt
