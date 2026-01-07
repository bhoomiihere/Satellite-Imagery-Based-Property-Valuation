# Satellite Imagery Based Property Valuation

##  Project Overview

This project implements an **end-to-end multimodal machine learning pipeline** for **property price prediction** by integrating:

- **Structured tabular housing data** (e.g., bedrooms, bathrooms, square footage, construction quality)
- **Satellite imagery** fetched using geographic coordinates to capture environmental and neighborhood context

The objective is to **enhance traditional real estate valuation models** by incorporating visual spatial information that is not present in standard tabular datasets, such as greenery, road density, and proximity to water bodies.

---

##  Dataset Description

### Tabular Data
- **train(1).xlsx** — contains housing features along with the target variable `price`
- **test2.xlsx** — contains the same set of features without the target variable

The dataset includes structural, spatial, temporal, and quality-related attributes commonly used in real estate valuation.

### Satellite Imagery
- Satellite images are fetched using **latitude and longitude coordinates**
- Images are obtained via the **Mapbox Static Images API**
- Each image captures neighborhood-level spatial patterns influencing property value

---

##  Methodology

The project follows a structured and modular machine learning workflow:

1. **Exploratory Data Analysis (EDA)**
   - Analysis of price distribution and skewness
   - Feature relationship exploration
   - Geospatial analysis using latitude and longitude

2. **Feature Engineering**
   - Domain-driven feature creation (house age, renovation indicator, relative size metrics)
   - Removal of redundant and highly correlated features
   - Preparation of clean, model-ready datasets

3. **Baseline Regression Models**
   - Linear Regression
   - Ridge Regression
   - Lasso Regression

4. **XGBoost on Tabular Data**
   - Capturing nonlinear relationships and feature interactions
   - Establishing a strong performance benchmark

5. **Satellite Image Acquisition**
   - Automated image download using the Mapbox API
   - Structured storage of training and testing images

6. **CNN Feature Extraction**
   - Transfer learning using pretrained **ResNet50**
   - Extraction of high-level visual embeddings
   - Dimensionality reduction using PCA

7. **Multimodal Feature Fusion**
   - Early fusion by concatenating tabular and image features
   - Training a unified regression model

8. **Final Model Evaluation**
   - Performance evaluation using **RMSE** and **R²**
   - Comparison of baseline, tabular, and multimodal models


---

##  Key Highlights

- Strong **XGBoost tabular baseline** with high predictive accuracy
- Practical application of **transfer learning** for satellite image analysis
- Demonstrates strengths and limitations of **multimodal learning**
- Clean, modular, and reproducible pipeline suitable for real-world use cases

---

##  Conclusion

This project demonstrates that while structured housing attributes remain the dominant predictors of property value, **satellite imagery provides valuable contextual understanding** of neighborhood environments. The work highlights the importance of feature engineering, data quality, and careful model design in building robust real estate valuation systems.

---

## 👤 Author

**Bhoomi Kaushik**

---

## 📌 Notes

- API tokens are **not included** in the repository for security reasons
- The project is designed to run on **Google Colab** or any Jupyter environment



