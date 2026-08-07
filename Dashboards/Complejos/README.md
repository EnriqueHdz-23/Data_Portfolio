# Dashboards: Predictive Maintenance, Wine Quality and California Housing Predictions

This project showcases interactive dashboards and predictive modeling applied to two datasets:  
1. **Predictive Maintenance (AI4I 2020 Predictive Maintenance Dataset)** - estimating real-time machine failure probability based on operational conditions 
2. **Wine Quality (UCI dataset)** – classification of wine quality using Random Forest.  
3. **California Housing (Scikit-learn dataset)** – regression analysis of housing prices using Random Forest.  

The focus is on building **predictive models** and integrating them with **interactive visualizations** for exploratory data analysis.

---

## Predictive Maintenance Dashboard — Rotating Machinery

### Objective
Develop an interactive dashboard for **industrial predictive maintenance**, estimating real-time machine failure probability based on operational conditions (temperature, rotational speed, torque, and tool wear).

### Libraries Used
- pandas, numpy  
- scikit-learn (RandomForestClassifier, train_test_split, LabelEncoder, accuracy_score)  
- plotly (express, graph_objects, io)  
- ipywidgets (interact, display, widgets)  
- warnings  

### Dataset
**AI4I 2020 Predictive Maintenance Dataset** — 10,000 synthetic records simulating manufacturing processes, including process variables (air temperature, process temperature, rotational speed, torque, tool wear) and associated failure events.

### Main Results
- Random Forest Classifier trained to predict machine failure events.  
- Achieved reliable accuracy for binary classification (failure vs. no failure).  
- Interactive dashboard built with Plotly and ipywidgets, allowing users to adjust operational parameters via sliders and instantly view predicted failure probability.  
- Demonstrates practical application of **predictive maintenance** in industrial contexts.  

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
