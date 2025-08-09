# Student Performance Analysis

## 1. Project Overview
This is an end-to-end machine learning project focused on analyzing and predicting student performance. By leveraging student demographics and academic data, the project aims to identify key indicators of success and support educational interventions.

## 2. Dataset
- **Source**: Include dataset origin (e.g., Kaggle, UCI Student Performance Data)
- **Size & Structure**: X records, Y features, and the target variable (e.g., Pass/Fail or Final Grade)
- **Features**:
  - Demographics (gender, age, parental education, etc.)
  - Academic metrics (attendance, previous grades, study hours)
  - Socioeconomic indicators (lunch type, access to resources)

## 3. Data Preprocessing
- Handled missing values via [e.g., mean/mode imputation]
- Categorical encoding: label encoding or one-hot for variables such as gender, meal type
- Numerical scaling: StandardScaler or MinMaxScaler for features like study hours
- Feature engineering: Created new variables such as "study_hours × previous_grade" to enhance model performance
- Train/Validation/Test split: e.g., 70% train, 15% validation, 15% test

## 4. Exploratory Data Analysis (EDA)
- Visualizations: histograms, boxplots, and heatmaps to understand distribution and relationships
- Insights: e.g., parental education and attendance showed strong correlation with performance

## 5. Modeling & Evaluation
- Algorithms experimented with:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost / CatBoost (if applicable, based on folder `catboost_info`)
- Model tuning with GridSearchCV / RandomizedSearchCV
- Evaluation metrics:
  - Classification: Accuracy, Precision, Recall, F1-score, ROC-AUC
  - Regression: RMSE, R² (if predicting continuous grade values)

## 6. Results & Key Insights
- Best model: e.g., Random Forest achieved 85% accuracy, 0.90 ROC-AUC
- Feature importance:
  - Top predictors were attendance, previous grades, and parental education
- Educational insight: Students with higher attendance and parental academic support tended to perform better

## 7. Application & Deployment
- **App files**: `app.py` and `appliccation.py`
- **Usage**:
  ```bash
  pip install -r requirements.txt
  python app.py
