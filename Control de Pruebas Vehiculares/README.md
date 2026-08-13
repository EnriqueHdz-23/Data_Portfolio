# Vehicle Testing Control Center

This project simulates a **vehicle testing control center** with synthetic data acquisition for braking performance and fuel economy analysis.  
The focus is on generating reproducible test runs, storing results in relational databases, and exposing interactive dashboards for engineering validation in the automotive industry.

---

## Objective
Generate **four distinct test runs** (`Test_ID`) with different seeds, ambient conditions, and test objectives, simulating a real-world validation campaign on track.  
The dashboard integrates braking and fuel economy metrics, providing automated alerts when thresholds exceed engineering safety or efficiency limits.

---

## Libraries Used
- numpy, pandas  
- plotly (graph_objects, make_subplots, io)  
- ipywidgets (interact, display)  
- sqlite3  
- datetime, os, json  
- scipy.integrate (cumtrapz, cumulative_trapezoid)  

---

## Dataset
Synthetic dataset generated via simulation of **600 seconds of driving cycles at 10 Hz**, combining:  
- Mixed driving profile (city + highway).  
- Three emergency braking events (100 → 0 km/h in 3.5 s).  
- Two gentle braking events.  

The dataset includes chassis, braking, engine, and fuel system variables such as:  
- Vehicle speed, deceleration, brake pressure, ABS activation, disc temperature.  
- Engine RPM, throttle position, load, coolant temperature, battery voltage.  
- Instant fuel flow and cumulative fuel level.  

---

## Main Results
- Generated reproducible datasets with **sensor-like noise** for realistic simulation.  
- Braking performance analysis: hydraulic pressure, ABS activation, disc temperature, stopping distance.  
- Fuel economy analysis: instantaneous fuel flow, average consumption in mixed cycles, driver behavior impact.  
- Interactive dashboard with Plotly and ipywidgets for real-time exploration.  
- Automated rule-based alerts for safety and efficiency thresholds.  

---

## Key Takeaways
- Demonstrates how **synthetic DAQ systems** can replicate real-world vehicle testing scenarios.  
- Combines **SQL integration, simulation, and interactive dashboards** for automotive engineering validation.  
- Highlights practical skills in **data generation, feature engineering, and visualization** applied to the automotive industry.  

