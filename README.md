# Predictive Policing & Spatial Analytics: CABA Crime Map Case Study

## 📌 Project Overview
This project provides a data-driven analysis of urban insecurity in **Palermo**, the district with the highest incidence of robberies and thefts in Buenos Aires (CABA). By merging **Spatial Statistics** with **Supervised Machine Learning**, we analyzed territorial patterns to identify high-risk zones and evaluate the predictive power of different algorithmic approaches.



---

## 🛠️ Key Technical Highlights

### 1. Spatial Feature Engineering
We moved beyond raw data by transforming geographic coordinates and urban Points of Interest (POI) into predictive features. 
* **Variable Creation:** Distance to subway stations, proximity to commercial avenues, and neighborhood density.
* **Geoprocessing:** Handled with the `sf` and `rgdal` packages in R to manage projections and spatial joins.

### 2. Machine Learning Pipeline
We implemented a comparative framework to determine the most accurate model for urban security forecasting:
* **Logistic Regression:** Established a statistical baseline for interpretability.
* **Random Forest:** Utilized to capture non-linear interactions between urban features.
* **XGBoost:** Fine-tuned via **Hyperparameter Optimization** (Learning Rate, Tree Depth, and Subsampling) to maximize precision and recall in imbalanced datasets.

---

## 📊 Model Comparison & Results
| Model | Approach | Key Benefit |
| :--- | :--- | :--- |
| **Logistic Regression** | Linear Baseline | High interpretability of feature coefficients. |
| **Random Forest** | Ensemble (Bagging) | Robust against outliers and spatial noise. |
| **XGBoost** | Boosting | Superior predictive power through iterative error correction. |

---

## 💻 Tech Stack
* **Language:** R
* **Spatial Analysis:** `sf`, `tmap`, `sp`
* **Machine Learning:** `tidymodels`, `xgboost`, `randomForest`, `caret`
* **Data Visualization:** `ggplot2`, `leaflet`

---

## 📂 Repository Structure
* `data/`: datasets.
* `scripts/`: R scripts for EDA, Spatial Engineering, and Modeling.
