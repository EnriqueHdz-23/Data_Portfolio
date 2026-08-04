# Machine Learning and Pandas Experiments

This project explores the integration of **Machine Learning models** with **pandas data structures** and demonstrates attribute methods for series. The focus is on applying classification algorithms, handling datasets, and performing exploratory analysis with Python.

---

## Example: Machine Learning and Pandas

### Objective
Implementation of a **Decision Tree Classifier** using scikit-learn, combined with pandas for dataset handling and preprocessing.

### Libraries Used
- pandas  
- sklearn (DecisionTreeClassifier, train_test_split, preprocessing, tree)  
- matplotlib  
- yfinance  
- os  

### Dataset
Iris dataset (`iris.csv`) loaded with pandas.  
Demonstrates preprocessing and classification tasks.

### Main Results
- Verified scikit-learn installation and version.  
- Applied Decision Tree Classifier to the Iris dataset.  
- Visualized classification results with matplotlib.  

---

## Series Index Example

### Objective
Demonstration that **series indices do not need to be unique**, using pandas and visualization.

### Libraries Used
- pandas  
- numpy  
- sklearn (DecisionTreeClassifier, train_test_split, tree, datasets)  
- matplotlib  
- yfinance  
- os  

### Dataset
Iris dataset imported with `read_csv()` and other methods.  
Additional examples with financial data using yfinance.

### Main Results
- Plotted Apple stock closing prices (`apple_s['Close'].plot()`).  
- Illustrated handling of non-unique indices in pandas series.  

---

## Lambda Function Example

### Objective
Application of **lambda functions and reduce** for mathematical operations, combined with pandas for dataset handling.

### Libraries Used
- pandas  
- functools.reduce  

### Dataset
Custom dataset (`jamesbond_e.csv`) loaded with pandas.  

### Main Results
- Implemented a lambda function to cube integers in a list.  
- Demonstrated factorial calculation using user input.  

---

## Key Takeaways
- Integration of **pandas** with machine learning models facilitates efficient data preprocessing and analysis.  
- Attribute methods in pandas series provide flexibility in handling non-unique indices and custom operations.  
- Combining **lambda functions** with pandas enables concise mathematical transformations.  
- These experiments highlight practical skills in **data manipulation, machine learning, and exploratory analysis**.  
