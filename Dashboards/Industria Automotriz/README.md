# Automotive Industry Dashboards

This project showcases interactive dashboards and predictive modeling applied to the automotive sector.  
The focus is on leveraging **public APIs, machine learning models, and synthetic datasets** to explore recalls, resale price predictions, and the global transition to electric vehicles (EVs).  
These dashboards highlight practical applications of **data visualization, predictive analytics, and industry insights**.

---

## Vehicle Recalls Explorer (NHTSA API)

### Objective
Develop an interactive dashboard to explore **vehicle recalls** using the official NHTSA API, enabling users to filter by brand and model.

### Libraries Used
- pandas  
- requests  
- plotly (express, io)  
- ipywidgets (widgets, display)  

### Dataset
Data retrieved dynamically from the **NHTSA Vehicle API** and **NHTSA Recalls API**.  
Curated list of popular automotive brands included for efficient querying.

### Main Results
- Interactive dashboard displaying recall information by brand and model.  
- API integration with error handling and optimized queries.  
- Enhanced usability with curated brand selection.  

---

## Motorcycle Resale Price Predictor

### Objective
Predict motorcycle resale prices using a **Random Forest Regressor**, integrating live currency conversion from INR to MXN.

### Libraries Used
- pandas, numpy  
- requests, io  
- scikit-learn (RandomForestRegressor, train_test_split, ColumnTransformer, OneHotEncoder, Pipeline, mean_absolute_error)  
- plotly (graph_objects, express, io)  
- ipywidgets (widgets, display)  

### Dataset
Public dataset of motorcycle prices (`Bike Prices.csv`) retrieved via URL.  
Currency conversion performed using the **Frankfurter API** (INR → MXN).

### Main Results
- Cleaned dataset with imputation of missing values.  
- Currency conversion applied to all price variables.  
- Random Forest Regressor trained for resale price prediction.  
- Achieved strong predictive performance with evaluation metrics (MAE, R²).  
- Interactive dashboard for exploring predictions by brand and features.  

---

## Global Automotive Electric Transition (2015–2024)

### Objective
Visualize the **global transition to electric vehicles (EVs)** using synthetic but realistic datasets inspired by public industry trends.

### Libraries Used
- pandas, numpy  
- plotly (graph_objects, make_subplots, io)  
- ipywidgets (widgets, display)  

### Dataset
Synthetic dataset simulating EV adoption, CO₂ emissions, and specifications by brand and country (2015–2024).  
Values are simulated for demonstration purposes but inspired by real-world industry patterns.

### Main Results
- Three synchronized visualizations controlled by widgets:  
  1. 🌍 Choropleth map – EV adoption by country.  
  2. 🧊 3D scatter plot – Weight vs. Power vs. Price, colored by CO₂ emissions.  
  3. 🔥 Heatmap + trend – CO₂ emissions by brand over time.  
- Interactive controls update all visualizations simultaneously.  
- Demonstrates industry-wide trends in EV adoption and emissions reduction.  

---

## Key Takeaways
- Integration of **APIs, machine learning, and synthetic datasets** enables robust automotive dashboards.  
- Dashboards provide insights into **vehicle recalls, resale price predictions, and EV adoption trends**.  
- These projects highlight practical skills in **data engineering, predictive modeling, and interactive visualization** applied to the automotive industry.  

