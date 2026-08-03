# COVID-19 Data Analysis and Prediction – Mexico

This repository contains multiple experiments using **public COVID-19 datasets from Mexico**. The projects explore statistical tests, machine learning models, clustering, and deep learning approaches to analyze pandemic data and ultimately predict daily infections for the following 7 days at the national level.

---

## Chi-Cuadrado_EHG

### Objective
Application of the **Chi-Square test** to evaluate independence between categorical variables in COVID-19 data.

### Libraries Used
- pandas  
- numpy  
- chi2_contingency (scipy.stats)

### Dataset
COVID-19 open dataset (`datos_abiertos_covid19.csv`, 1,000 rows).

### Main Results
Exploratory statistical analysis of categorical relationships in patient records.

---

## Correlacion_EHG

### Objective
Correlation analysis of numerical variables to identify relationships in COVID-19 data.

### Libraries Used
- pandas  
- numpy  

### Dataset
COVID-19 open dataset (`datos_abiertos_covid19.csv`, 6,200 rows).

### Main Results
Correlation matrices highlighting associations between patient attributes and outcomes.

---

## cor_EHG

### Objective
Use of **PySpark** for distributed correlation analysis on COVID-19 data.

### Libraries Used
- findspark  
- SparkConf, SQLContext, StringType  
- pandas  
- numpy  

### Dataset
COVID-19 open dataset (`datos_abiertos_covid19.csv`, 6,200 rows).

### Main Results
Schema exploration and distributed data handling with Spark.

---

## Modules

### Objective
Deep learning experiments with **TensorFlow/Keras** to model COVID-19 data.

### Libraries Used
- pandas, numpy, csv, os  
- matplotlib (pyplot)  
- tensorflow, keras (Sequential, layers, RMSprop)  
- sklearn OrdinalEncoder  
- scipy (curve_fit)

### Dataset
COVID-19 dataset (`COVID-19.csv`).

### Main Results
Neural network models applied to encoded patient data for predictive tasks.

---

## k-means_EHG

### Objective
Clustering of patient attributes using **K-Means** to identify risk groups.

### Libraries Used
- pandas  
- numpy  
- matplotlib  
- sklearn.preprocessing, KMeans  

### Dataset
COVID-19 open dataset (`datos_abiertos_covid19.csv`, 1,000 rows).  
Selected features: smoking, obesity, cardiovascular conditions, and region.

### Main Results
Cluster visualization of municipalities and obesity prevalence.

---

## KNeighbors_EHG

### Objective
Classification of patient outcomes using **K-Nearest Neighbors (KNN)**.

### Libraries Used
- pandas  
- numpy  
- sklearn.neighbors.KNeighborsClassifier  
- sklearn.metrics.confusion_matrix  

### Dataset
COVID-19 open dataset (`datos_abiertos_covid19.csv`, 6,000 rows).

### Main Results
Confusion matrix analysis of intubation predictions.

---

## naiveBayes_EHG

### Objective
Classification using **Naive Bayes models** (Bernoulli, Gaussian, Multinomial).

### Libraries Used
- pandas  
- numpy  
- sklearn.naive_bayes  

### Dataset
COVID-19 open dataset (`datos_abiertos_covid19.csv`, 6,000 rows).

### Main Results
Evaluation of probabilistic models for patient outcome prediction.

---

## pandas_EHG

### Objective
Data exploration and preprocessing with **pandas**.

### Libraries Used
- pandas  

### Dataset
COVID-19 open dataset (`datos_abiertos_covid19.csv`, 1,000 rows).

### Main Results
Basic data cleaning and inspection.

---

## PronosticoCovid-19_EHG

### Objective
Forecasting daily infections using **deep learning models** (LSTM, Sequential, Keras).

### Libraries Used
- pandas, numpy, matplotlib  
- keras (Sequential, Dense, LSTM, Dropout, BatchNormalization, Callbacks)  
- sklearn.preprocessing.MinMaxScaler  

### Dataset
COVID-19 time series dataset (`diarios_baselimpia(arreglada).csv`).  
Variables: daily infections, cumulative infections, daily deaths, cumulative deaths.

### Main Results
- Time series forecasting of daily infections.  
- Neural network models trained to predict **7-day horizon of daily cases**.  
- Visualizations of predicted vs. actual infection trends.

---

## pySpark_1_EHG

### Objective
Exploration of COVID-19 data with **PySpark** for scalable processing.

### Libraries Used
- pandas  
- numpy  
- findspark, SparkConf, SQLContext, StringType  

### Dataset
COVID-19 open dataset (`datos_abiertos_covid19.csv`, 6,000 rows).

### Main Results
Schema inspection and distributed data handling.

---

## Regresion_lineal_EHG

### Objective
Application of **Linear Regression** to model COVID-19 infection trends.

### Libraries Used
- pandas  
- numpy  
- matplotlib  
- sklearn (datasets, linear_model, mean_squared_error, r2_score)

### Dataset
COVID-19 dataset (`Covid.csv`).  
Variables: daily infections, cumulative infections, normalized cases per 100k, deaths.

### Main Results
Linear regression models applied to time series features with evaluation metrics (MSE, R²).

---

## Key Takeaways
- Public COVID-19 datasets enable **rich statistical and machine learning experiments**.  
- Models range from **basic statistical tests** (Chi-Square, correlation) to **advanced deep learning** (LSTM forecasting).  
- Predictive modeling demonstrated the feasibility of forecasting **daily infections for 7 days ahead** at the national level.  
- This portfolio highlights skills in **data preprocessing, statistical analysis, machine learning, and deep learning applied to real-world public health data**.  
