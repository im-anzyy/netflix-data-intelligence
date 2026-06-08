# Netflix Content Intelligence & Rating Predictor

## Overview

An end-to-end Data Analytics and Machine Learning project analyzing Netflix's content library of 8,807 titles. This project explores global content trends, audience-targeting patterns, and builds predictive models to classify Netflix content into audience rating categories: **Kids**, **Teen**, and **Adult**.

The project follows a complete machine learning workflow, including data cleaning, exploratory data analysis (EDA), feature engineering, model training, and performance evaluation.

---

## Research Question

Can content metadata such as content type, genre, release year, duration, and country of origin be used to accurately predict the target audience category of Netflix content?

---

## Dataset

**Source:** Netflix Titles Dataset (Kaggle)

**Dataset Size:** 8,807 Netflix titles

The dataset contains metadata describing movies and TV shows available on Netflix, including:

- Title
- Content Type (Movie / TV Show)
- Country
- Date Added
- Release Year
- Rating
- Duration
- Genre Categories

After preprocessing and feature engineering, the dataset was transformed into a machine-learning-ready format for classification.

---

## Project Structure

```text
01_EDA.ipynb
│
├── Exploratory Data Analysis
├── Trend Analysis
└── Data Visualization

02_feature_engineering.ipynb
│
├── Data Cleaning
├── Feature Engineering
├── Data Transformation
└── Dataset Preparation

03_ml_model.ipynb
│
├── Model Training
├── Model Evaluation
└── Performance Comparison
```

## Exploratory Data Analysis (EDA)

The EDA phase focused on understanding Netflix's content distribution and identifying trends within the platform.

Areas explored include:

- Distribution of Movies vs TV Shows
- Content growth over time
- Country-wise content production
- Rating distribution
- Genre popularity
- Audience category trends

---

## Key Insights

- More than 70% of Netflix content targets Teen or Adult audiences.
- TV-MA is the most common rating category across the platform.
- The United States and India are the two largest content-producing countries in the dataset.
- Teen content is the most difficult category to classify due to overlap with both Kids and Adult content.
- Kids content is the most distinguishable audience category and is classified more accurately by machine learning models.

---

## Feature Engineering

To prepare the dataset for machine learning:

- Missing and inconsistent values were handled.
- Relevant metadata fields were cleaned and transformed.
- Categorical features were encoded for model compatibility.
- Features were prepared for supervised classification.

---

## Machine Learning Models

Three classification models were trained and compared:

| Model | Accuracy |
|---------|---------|
| Logistic Regression | 67% |
| Random Forest | 66% |
| XGBoost | 69% |

---

## Evaluation

Models were evaluated using classification accuracy and comparative performance analysis.

### Results

- XGBoost achieved the highest overall accuracy (**69%**).
- Logistic Regression delivered competitive performance despite its simpler architecture.
- Random Forest provided a strong baseline model for comparison.
- XGBoost demonstrated the best predictive capability among the evaluated approaches.

---

## Tech Stack

### Programming & Data Science
- Python
- Pandas
- NumPy

### Visualization
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn
- XGBoost

### Development Environment
- Jupyter Notebook

---

## Future Improvements

Potential extensions to this project include:

- Incorporating NLP-based analysis of content descriptions.
- Experimenting with deep learning models.
- Improving classification performance for Teen-rated content.
- Using additional metadata sources for richer feature representation.
- Exploring recommendation-system applications using content intelligence insights.

---

## How to Run

1. Clone this repository.

```bash
git clone https://github.com/im-anzyy/netflix-data-intelligence.git
```

2. Create a `data/` folder and place the Netflix dataset CSV file inside it.

3. Run the notebooks in the following order:

```text
01_EDA.ipynb
↓
02_feature_engineering.ipynb
↓
03_ml_model.ipynb
```

---

## Project Highlights

- End-to-end Machine Learning workflow
- Analysis of 8,807 Netflix titles
- Exploratory Data Analysis and visualization
- Feature engineering and preprocessing pipeline
- Comparative evaluation of multiple classification models
- Best model accuracy: **69% using XGBoost**
