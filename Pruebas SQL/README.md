# SQL Dashboards and Probability Modeling in Python

This portfolio section demonstrates the integration of **SQL queries within Python notebooks** using both **SQLite** and **DuckDB**, combined with statistical modeling and machine learning.  
The focus is on handling relational datasets, performing analytical queries, and applying advanced techniques such as **predictive maintenance dashboards**, **exchange rate analysis**, and **probability modeling of customer arrivals**.  
These projects highlight versatile workflows that combine **SQL engines, Python, and data science methods** for real-world scenarios.
**SQL Integration (Automotive Examples)** – Analytical dashboards using SQLite and DuckDB applied to automotive scenarios.  
  Includes **Predictive Maintenance**, **Exchange Rate Analysis**, **Customer Arrival Modeling**, plus new examples for **Fleet Management & Spare Parts Logistics** and **Profitability by Model (Costs vs. Sale Price)**.  

# Automotive Industry SQL Dashboards

This project demonstrates the use of **SQL queries within Python notebooks** applied to automotive industry scenarios.  
The focus is on building synthetic but realistic datasets, executing analytical queries with **CTEs and window functions**, and integrating results into interactive dashboards with Plotly and ipywidgets.  
These examples highlight how SQL can be combined with Python to model **fleet management, spare parts logistics, and profitability analysis** in automotive contexts.

---

## Fleet Management and Spare Parts Logistics

### Objective
Model a network of dealerships with rental fleets, maintenance history, and spare parts inventory using **SQLite**.  
Perform analytical queries to evaluate monthly sales, maintenance events, and inventory risks.

### Libraries Used
- pandas, numpy  
- sqlite3  
- plotly (graph_objects, io)  
- ipywidgets (interact, widgets, display)  

### Dataset
Synthetic dataset generated with fixed seed (`np.random.seed(42)`), ensuring reproducibility.  
Tables include:  
- `concesionarios` – dealership catalog by region  
- `ventas_mensuales` – monthly rental income and units  
- `historial_mantenimiento` – maintenance events by model and dealership  
- `inventario_repuestos` – spare parts stock, lead time, and consumption  

### Main Results
- Built reproducible SQLite database with multiple tables.  
- Applied **CTEs and window functions** (`LAG`, `RANK`) for analytical queries.  
- Interactive dashboard for exploring fleet performance and spare parts logistics.  

---

## Profitability by Model (Costs vs. Sale Price)

### Objective
Analyze profitability by combining spare parts costs and sale prices through **SQL joins** and caching mechanisms.

### Libraries Used
- pandas, numpy  
- sqlite3  
- plotly (graph_objects, io)  
- ipywidgets (widgets, display)  
- functools.lru_cache  

### Dataset
Synthetic dataset modeling 5 brands × 5 models with quarterly costs and sale prices.  
Tables include:  
- `modelos` – brand/model catalog  
- `costos_repuestos` – component costs by model and period  
- `precios_venta` – list price and average discount by model, period, and region  

### Main Results
- Implemented parameterized queries with caching (`lru_cache`) to optimize performance.  
- Combined costs and prices via SQL joins to calculate margins.  
- Interactive dashboard with chained dropdowns (brand → model).  
- Demonstrated profitability analysis with SQL-driven workflows.  

---

## Key Takeaways
- **SQL integration with Python** enables efficient analytical queries on synthetic automotive datasets.  
- Dashboards provide insights into **fleet management, spare parts logistics, and profitability analysis**.  
- These projects showcase practical skills in **SQL feature engineering, interactive visualization, and industry-specific modeling**.  


---

## Predictive Maintenance Dashboard with Analytical SQL (DuckDB) + Machine Learning

### Objective
Develop an interactive dashboard for **predictive maintenance** using industrial sensor data, combining **DuckDB SQL feature engineering** with a Random Forest Classifier to estimate machine failure probability.

### Libraries Used
- pandas, numpy  
- duckdb (analytical SQL engine)  
- scikit-learn (RandomForestClassifier, train_test_split, LabelEncoder, accuracy_score)  
- plotly (express, graph_objects, io)  
- ipywidgets (widgets, display)  
- requests, io  
- warnings  

### Dataset
**AI4I 2020 Predictive Maintenance Dataset** — 10,000 synthetic records simulating manufacturing processes, including process variables (air temperature, process temperature, rotational speed, torque, tool wear) and associated failure events.

### Main Results
- Feature engineering performed entirely with **SQL queries in DuckDB** (derivative variables, aggregations, descriptive statistics).  
- Random Forest Classifier trained once and cached for real-time predictions.  
- Interactive dashboard with sliders to adjust operational parameters and view predicted failure probability.  
- Demonstrates modern workflows combining **SQL OLAP engines** with Python and ML.  

---

## Interactive SQL Dashboard for Exchange Rates

### Objective
Build an interactive dashboard to analyze **currency exchange rates** using SQL queries with SQLite, integrated into Jupyter Notebook.

### Libraries Used
- pandas, numpy  
- sqlite3 (SQL engine)  
- plotly (graph_objects, io)  
- ipywidgets (widgets, display)  
- requests  
- datetime (date, timedelta)  
- warnings  

### Dataset
Exchange rate data retrieved via **public API requests**, stored and queried with SQLite for analysis and visualization.

### Main Results
- Implemented SQL queries with **window functions** for time-based analysis of exchange rates.  
- Interactive dashboard with Plotly visualizations embedded in Jupyter Notebook.  
- Demonstrated integration of **SQL + Python** for financial data exploration.  
- Showcased practical use of SQLite for lightweight analytical tasks.  

---

## Customer Arrival Modeling

### Objective
Model customer arrivals at a service desk using the **exponential distribution** to estimate waiting times.  
The goal is to calculate probabilities of waiting less than a given time between arrivals.

### Libraries Used
- pandas – data manipulation  
- sqlite3 – database connection and queries  
- sqldf – SQL queries directly on pandas DataFrames  
- scipy.stats.expon – exponential distribution modeling  

### Dataset
Relational datasets imported via pandas:  
- `departments.csv`  
- `upd_empl_2.csv`  
- `regions.csv`  

These files simulate organizational data for SQL query testing.

### Main Results
- Defined arrival rate λ = 1/15 customers per minute (average arrival every 15 minutes).  
- Calculated probability of waiting less than 7 minutes between arrivals using exponential CDF.  
- Result:  Probability of waiting less than 7 minutes ≈ 0.36

- Demonstrated SQL queries on relational datasets using pandas and SQLite integration.  

---

## Key Takeaways
- Integration of **SQL with Python notebooks** enables efficient querying and analysis of relational data.  
- The **exponential distribution** is a practical tool for modeling inter-arrival times in queuing systems.  
- Combining SQL queries with statistical modeling provides a versatile workflow for **data engineering and analytics**.  

