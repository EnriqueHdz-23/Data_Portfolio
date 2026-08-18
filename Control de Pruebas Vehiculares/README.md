# Automotive Testing Control Center & Analytical Dashboards

This project simulates a **vehicle testing control center** and extends it with analytical dashboards for automotive industry validation.  
The focus is on generating reproducible synthetic datasets, integrating them into relational databases, and exposing interactive dashboards for **braking performance, fuel economy, quality analytics, and real-time production monitoring**. It also includes a **Statistical Process Control (SPC) dashboard for automotive paint booths**, applying control charts and quality metrics to ensure compliance with OEM tolerances.  

---

## Vehicle Testing Control Center

### Objective
Simulate multiple vehicle test runs under varying conditions to evaluate **braking performance** and **fuel economy**.  
The system integrates CAN bus–like data into a relational database and provides interactive dashboards for engineering validation.

### Libraries Used
- numpy, pandas  
- plotly (graph_objects, make_subplots, io)  
- ipywidgets (interact, display)  
- sqlite3  
- datetime, os, json  
- scipy.integrate (cumtrapz, cumulative_trapezoid)  

### Dataset
Synthetic dataset simulating **600 seconds of driving cycles at 10 Hz**, including:  
- Mixed driving profile (city + highway).  
- Emergency and gentle braking events.  
- Variables: speed, deceleration, brake pressure, ABS activation, disc temperature, engine RPM, throttle, load, coolant temperature, battery voltage, fuel flow, and fuel level.  

### Main Results
- Braking performance analysis with hydraulic pressure, ABS activation, disc temperature, and stopping distance.  
- Fuel economy analysis with instantaneous fuel flow and average consumption in mixed cycles.  
- Interactive dashboard with automated alerts when thresholds exceed safety or efficiency limits.  

---

## Quality Analytics Warehouse — Cutting Emulsions & Burrs

### Objective
Build an **analytical warehouse** using DuckDB and machine learning to monitor quality metrics in automotive manufacturing processes.  

### Libraries Used
- pandas, numpy  
- duckdb  
- plotly (express, graph_objects, io)  
- ipywidgets (interactive_output, widgets, layouts)  
- scikit-learn (Ridge, StandardScaler, mean_absolute_error)  
- requests, io, warnings  

### Dataset
Public dataset of vehicle specifications (`mtcars.csv`) reinterpreted as component archetypes for populating dimension tables.  
Synthetic historical plant data generated to simulate production quality metrics.  

### Main Results
- Ingested external CSV data and transformed it into dimensional models.  
- Applied SQL queries with DuckDB for feature engineering and aggregations.  
- Built dashboards with corporate color palettes for monitoring quality KPIs.  
- Ridge regression applied to predict quality outcomes with evaluation metrics (MAE, R²).  

---

## Real-Time Production Monitor — Welding Robotics / Paint Booth

### Objective
Simulate a **real-time production monitoring dashboard** for automotive manufacturing, integrating robotic welding and paint booth operations.  

### Libraries Used
- pandas, numpy  
- plotly (graph_objects, io)  
- ipywidgets (VBox, HBox, Layout, display)  
- threading, time, collections  
- requests, datetime, warnings  

### Dataset
Demonstrative integration with **NHTSA recalls API** for external data, combined with synthetic streaming data for production monitoring.  

### Main Results
- Real-time dashboard simulating welding and paint booth operations.  
- Streaming data visualizations with alerts for anomalies.  
- External API integration (NHTSA recalls) for enriched context.  
- Offline fallback ensures robustness of the monitoring system.  

---

# Statistical Process Control (SPC) — Automotive Paint Booth

This project implements a **Statistical Process Control (SPC) dashboard** for monitoring electrostatic paint booth operations in automotive assembly plants.  
The focus is on ensuring color and finish quality under OEM tolerances (BMW, VW) by applying SPC methodologies to spectrophotometric measurements.

## Objective
Develop a dashboard that applies SPC techniques to monitor and control the paint booth process by:  
1. Establishing **control limits (±3σ)** based on warm-up phase measurements.  
2. Detecting special causes and systematic drifts using **Western Electric rules**.  
3. Measuring short-term variability with **Moving Range (MR) charts**.  
4. Calculating **First Time Through (FTT)** to evaluate production efficiency.  

## Libraries Used
- numpy, pandas  
- plotly (graph_objects, make_subplots, io)  
- ipywidgets (interactive controls, display)  
- sqlite3  
- datetime, json  

## Dataset
Synthetic dataset simulating spectrophotometric measurements of **CIE-Lab L\*** values during automotive paint booth operations.  
Data includes warm-up phase readings, production measurements, and tolerance thresholds defined by OEM standards.  

## Main Results
- Implemented **Individuals-Moving Range (I-MR) charts** for monitoring process stability.  
- Applied **Western Electric rules** to detect systematic drifts before out-of-control conditions occur.  
- Calculated **FTT metric** for the last hour of production, measuring compliance with OEM tolerances.  
- Interactive dashboard for real-time visualization of control charts and quality indicators.  
- Provided actionable alerts when deviations exceed control limits or drift patterns are detected.  

## Key Takeaways
- Demonstrates how **SPC dashboards** can ensure paint booth quality and prevent costly rework.  
- Combines **statistical process control, SQL integration, and visualization** for automotive manufacturing.  
- Highlights practical skills in **quality analytics, anomaly detection, and dashboard design** applied to the automotive industry.  

---

## Vehicle Testing Dashboard — CAN Bus Data Analysis

### Objective
Simulate **CAN bus time series data** for vehicle test runs, enabling anomaly detection and dashboard visualization.  

### Libraries Used
- numpy, pandas  
- plotly (graph_objects, make_subplots, io)  
- ipywidgets (widgets, display)  
- sqlite3  
- datetime, warnings, os  

### Dataset
Synthetic dataset generated for each test run, including:  
- Speed profile (acceleration, cruise, braking cycles).  
- Engine RPM, coolant temperature, battery voltage.  
- Brake pressure and 3-axis acceleration (X, Y, Z).  
- Gear selection derived from speed.  
- Injected anomalies: coolant temperature spikes and battery voltage drops.  

### Main Results
- Generated reproducible CAN bus datasets with realistic sensor noise.  
- Detected anomalies in coolant temperature and battery voltage.  
- Interactive dashboard for visualizing speed, RPM, braking, and acceleration data.  
- Demonstrated integration of synthetic CAN bus data with relational databases and dashboards.  

---

## Key Takeaways
- Demonstrates how **synthetic DAQ and CAN bus systems** can replicate real-world vehicle testing scenarios.  
- Combines **SQL integration, simulation, and interactive dashboards** for automotive engineering validation.  
- Highlights practical skills in **data generation, anomaly detection, predictive modeling, and visualization** applied to the automotive industry.  
