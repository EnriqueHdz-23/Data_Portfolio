# Automotive Industry Dashboards

This project showcases interactive dashboards and predictive modeling applied to the automotive sector.  
The focus is on leveraging **public APIs, machine learning models, and synthetic datasets** to explore recalls, resale price predictions, and the global transition to electric vehicles (EVs).  
It also includes advanced **predictive monitoring dashboards** for industrial assets such as conveyor belt networks, highlighting applications of **IoT analytics, health scoring, and maintenance forecasting**.  
Additionally, it features **inventory forecasting and demand management dashboards**, designed to anticipate shortages of critical components and optimize preventive actions.  
These dashboards demonstrate practical applications of **data visualization, predictive analytics, and industry insights**.   

---

# Predictive Monitoring Dashboard — Conveyor Belt Network

This project simulates a **predictive monitoring and diagnostic system** for conveyor belts in automotive assembly lines.  
The focus is on transforming raw IIoT sensor data into **actionable intelligence** for early fault detection, asset health scoring, and maintenance planning.

## Objective
Develop a dashboard that monitors conveyor belt performance and predicts failures by:  
1. Detecting early degradation (bearing wear, misalignment, jams).  
2. Quantifying asset health with a **Health Score (0–100%)**.  
3. Estimating **Remaining Useful Life (RUL)** and suggesting preventive maintenance schedules.  
4. Calculating **Overall Equipment Effectiveness (OEE)** to prioritize maintenance resources.

## Libraries Used
- numpy, pandas  
- plotly (graph_objects, make_subplots, io)  
- ipywidgets (interactive controls, display)  
- sqlite3  
- datetime, warnings, signal processing (rfft, signal)  

## Dataset
Synthetic dataset simulating an **8-hour production shift**, with sensor readings every **10 seconds** across four conveyor belts.  
Controlled faults are injected to validate detection capabilities:  

| Conveyor | Failure Time | Failure Type       | Expected Signature                          |
|----------|--------------|--------------------|---------------------------------------------|
| B        | Hour 4       | Mechanical jam     | Sharp sustained spike in `Motor_Current_A`  |
| D        | Hour 6       | Roller misalignment| Spike in `Vibration_Z_ms2` with degradation |

## Main Results
- Generated reproducible IIoT sensor datasets with realistic fault signatures.  
- Implemented **Health Score** and **RUL estimation** for each conveyor.  
- Calculated **OEE metrics** to evaluate overall system efficiency.  
- Interactive dashboard for real-time monitoring and predictive diagnostics.  
- Export capability for executive reports in HTML/PDF format.  

## Key Takeaways
- Demonstrates how **predictive dashboards** can prevent costly downtime in automotive assembly lines.  
- Combines **signal processing, SQL integration, and visualization** for industrial IoT analytics.  
- Highlights practical skills in **predictive maintenance, health scoring, and dashboard design** applied to the automotive industry.  

---

# Inventory Control Dashboard — Demand Forecasting & Critical Component Management

This project implements a **forecast-driven inventory planning system** tailored for the automotive industry.  
The focus is on transforming demand simulations into actionable insights, ensuring that critical components are available to prevent production line stoppages.

## Objective
Develop a dashboard that integrates forecasting models with inventory management to:  
1. Simulate realistic demand patterns with seasonality.  
2. Manage a master parts catalog in SQLite.  
3. Apply **Holt-Winters exponential smoothing** for demand forecasting.  
4. Project inventory levels against `Safety_Stock` and `Reorder_Point`.  
5. Trigger risk alerts with exact reorder quantities (simplified EOQ).  
6. Generate executive reports in JSON format.  

## Libraries Used
- numpy, pandas  
- sqlite3  
- plotly (graph_objects, io)  
- ipywidgets (interactive controls, display)  
- statsmodels (ExponentialSmoothing)  
- datetime, json, warnings  

## Dataset
Synthetic dataset simulating demand for critical automotive components.  
Data is structured in SQLite tables for parts management, demand history, and inventory projections.  

## Main Results
- Implemented **forecasting pipeline** with Holt-Winters exponential smoothing.  
- Generated inventory projections against safety stock and reorder points.  
- Designed a **traffic-light risk system** to highlight potential shortages.  
- Automated alerts with recommended reorder quantities (EOQ-based).  
- Produced executive reports in JSON for decision-making.  

## Key Takeaways
- Demonstrates how **forecast-driven dashboards** can prevent costly production line stoppages.  
- Combines **time series forecasting, SQL integration, and visualization** for inventory management.  
- Highlights practical skills in **predictive analytics, demand planning, and dashboard design** applied to the automotive industry.  

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

