# Netflix Content Intelligence & Rating Predictor

## Overview
An end-to-end data analytics and machine learning project analyzing 
Netflix's content library of 8,807 titles. The project explores content 
trends and builds a model to predict audience rating categories 
(Kids / Teen / Adult) from content metadata.

## Dataset
Netflix Titles — Kaggle  
8,807 titles | 14 features after cleaning and engineering

## Project Structure
- `01_EDA.ipynb` — Exploratory Data Analysis & Visualizations
- `02_feature_engineering.ipynb` — Feature Engineering & Preprocessing  
- `03_ml_model.ipynb` — ML Model Training & Evaluation

## Key Insights
- 70%+ of Netflix content targets teens or adults (TV-MA dominates)
- USA and India are the top two content-producing countries
- Kids content is the most accurately predicted category by the model
- Teen content is hardest to classify — it sits between Kids and Adult

## Models Trained
| Model | Accuracy |
|---|---|
| Logistic Regression | 67% |
| Random Forest | 66% |
| XGBoost | 69% |

## Tech Stack
Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn

## How to Run
1. Clone this repository
2. Upload CSVs to a `data/` folder in your environment
3. Run notebooks in order: 01 → 02 → 03
