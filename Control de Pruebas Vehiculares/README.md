# Vehicle Testing Control Center & Dashboard

This project simulates a **vehicle testing control center** with synthetic data acquisition and dashboard visualization for automotive validation.  
The focus is on generating reproducible test runs, storing results in relational databases, and exposing interactive dashboards for **braking performance, fuel economy, and CAN bus data analysis**.

---

## Vehicle Testing Control Center

### Objective
Generate **four distinct test runs** (`Test_ID`) with different seeds, ambient conditions, and test objectives, simulating a real-world validation campaign on track.  
The dashboard integrates braking and fuel economy metrics, providing automated alerts when thresholds exceed engineering safety or efficiency limits.

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
- Three emergency braking events (100 → 0 km/h in 3.5 s).  
- Two gentle braking events.  
- Variables: speed, deceleration, brake pressure, ABS activation, disc temperature, engine RPM, throttle, load, coolant temperature, battery voltage, fuel flow, and fuel level.  

### Main Results
- Braking performance analysis: hydraulic pressure, ABS activation, disc temperature, stopping distance.  
- Fuel economy analysis: instantaneous fuel flow, average consumption in mixed cycles, driver behavior impact.  
- Interactive dashboard with Plotly and ipywidgets for real-time exploration.  
- Automated rule-based alerts for safety and efficiency thresholds.  

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
- Highlights practical skills in **data generation, anomaly detection, and visualization** applied to the automotive industry.  
