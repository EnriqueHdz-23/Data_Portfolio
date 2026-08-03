# Decision Trees Experiments

This repository contains exploratory projects applying **Decision Tree models** for both regression and classification tasks. The goal is to evaluate model performance, interpretability, and feature importance across different datasets.

---

## Arboles_EHG

### Objective
Implementation of **Decision Tree Regression** to predict continuous outcomes, with hyperparameter tuning and visualization of decision paths.

### Libraries Used
- pandas  
- numpy  
- matplotlib  
- scikit-learn (DecisionTreeRegressor, GridSearchCV, train_test_split, export_graphviz, export_text, plot_tree, mean_squared_error)  
- warnings  

### Dataset
Boston Housing dataset (`load_boston` from scikit-learn).  
Features include socioeconomic and housing attributes; the target variable is median house value.

### Main Results
- Decision Tree Regressor applied to predict housing prices.  
- GridSearchCV used for hyperparameter optimization.  
- Visualization of the tree structure and feature importance.  
- Model achieved reasonable predictive accuracy, with mean squared error as the evaluation metric.

---

## DecisionTreeClassifier_EHG

### Objective
Application of **Decision Tree Classification** to survey data, aiming to classify responses and evaluate model interpretability.

### Libraries Used
- pandas  
- numpy  
- matplotlib  
- scikit-learn (tree, RandomForestClassifier, RandomForestRegressor)  
- eli5  
- shap  

### Dataset
Survey dataset (`EncuestaFI.csv`).  
Data preprocessing included handling missing values and random sampling for train/test splits.

### Main Results
- Decision Tree Classifier applied to categorical survey responses.  
- Random Forest models used for comparison and feature importance analysis.  
- Visualizations generated with `tree` and `eli5` to interpret model decisions.  
- Results highlighted key survey questions as influential predictors.

---

## expVoluntaria_EHG

### Objective
Classification experiment using **Decision Trees and Random Forests** on encoded survey data to predict voluntary responses.

### Libraries Used
- pandas  
- numpy  
- matplotlib  
- scikit-learn (tree, RandomForestClassifier, RandomForestRegressor)  
- eli5  
- shap  

### Dataset
Encoded survey dataset (`encoded.csv`).  
Preprocessing included dropping missing values, shuffling, and splitting into training and test sets.

### Main Results
- Decision Tree and Random Forest models applied to encoded categorical data.  
- Feature importance analysis performed with SHAP and ELI5.  
- Results demonstrated the model’s ability to identify key predictors of voluntary responses.  
- Accuracy and interpretability balanced through tree visualization and feature importance plots.

---

## Key Takeaways
- Decision Trees provide **transparent and interpretable models**, useful for both regression and classification tasks.  
- Hyperparameter tuning and ensemble methods (Random Forests) improve performance while maintaining interpretability.  
- Feature importance analysis (SHAP, ELI5) adds value for stakeholders by highlighting the most relevant variables.  
