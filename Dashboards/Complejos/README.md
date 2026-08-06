# Dashboards: Wine Quality and California Housing Predictions

This project showcases interactive dashboards and predictive modeling applied to two datasets:  
1. **Wine Quality (UCI dataset)** – classification of wine quality using Random Forest.  
2. **California Housing (Scikit-learn dataset)** – regression analysis of housing prices using Random Forest.  

The focus is on building **predictive models** and integrating them with **interactive visualizations** for exploratory data analysis.

---

## Wine Quality Prediction

### Objective
Classify wine samples into **good vs. bad quality** based on physicochemical attributes, using a Random Forest Classifier.

### Libraries Used
- pandas, numpy  
- scikit-learn (RandomForestClassifier, train_test_split, accuracy_score)  
- plotly (express, graph_objects)  
- ipywidgets (interact, display)  
- warnings  

### Dataset
Red wine quality dataset from UCI Machine Learning Repository:  
`winequality-red.csv`  

Target variable: **quality > 6 → Good (1), else Bad (0)**

### Main Results
- Dataset size: **1,599 records**  
- Random Forest Classifier trained with 100 estimators.  
- Achieved accuracy: **~72%** on test set.  
- Interactive dashboard built with Plotly and ipywidgets for dynamic exploration of features and predictions.  

---

## California Housing Prediction

### Objective
Predict median house values in California using a Random Forest Regressor, with interactive visualizations for feature exploration.

### Libraries Used
- pandas, numpy  
- scikit-learn (fetch_california_housing, RandomForestRegressor, train_test_split, r2_score)  
- plotly (express, graph_objects, io)  
- ipywidgets (widgets, display)  

### Dataset
California Housing dataset from scikit-learn (`fetch_california_housing`).  
Features include median income, house age, average rooms, population, and location-based attributes.

### Main Results
- Random Forest Regressor trained on housing features.  
- Achieved **R² score ~0.80**, indicating strong predictive performance.  
- Interactive dashboard built with Plotly and ipywidgets for visualizing predictions and feature importance.  

---

## Key Takeaways
- **Random Forest models** provide robust performance for both classification and regression tasks.  
- Integration of **interactive dashboards** enhances interpretability and user engagement.  
- These projects demonstrate practical skills in **data preprocessing, predictive modeling, and visualization** applied to real-world datasets.  
