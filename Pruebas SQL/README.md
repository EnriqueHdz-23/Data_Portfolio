# SQL Integration and Probability Modeling in Python

This project demonstrates the integration of **SQL queries within Python notebooks** using pandas and SQLite, combined with probability modeling through statistical distributions. The focus is on handling relational datasets, querying them efficiently, and applying statistical analysis to real-world scenarios.

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

