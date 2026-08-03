# MapReduce Text Analysis

This project demonstrates the use of **MapReduce functions** to process and analyze text data efficiently. The focus is on leveraging distributed computing with Apache Spark to handle large-scale datasets and extract meaningful insights.

---

## mapReduce_EHG

### Objective
Implementation of a **MapReduce workflow** for text analysis. The goal is to tokenize, transform, and aggregate textual information to identify patterns, frequencies, and relevant metrics in unstructured data.

### Libraries Used
- **findspark** – Spark initialization within Python  
- **SparkConf** – Spark configuration setup  
- **SQLContext** – Structured data handling with Spark SQL  
- **StringType** – Schema definition for text fields  

### Dataset
The dataset is based on **textual input files** (unstructured text). While the specific dataset is not detailed, the workflow is designed to be adaptable to any large text corpus such as logs, survey responses, or documents.

### Main Results
- Successful implementation of a **MapReduce pipeline** using PySpark.  
- Text preprocessing included tokenization and schema definition with `StringType`.  
- Aggregation of word frequencies and identification of key terms across the dataset.  
- Demonstrated scalability and efficiency of Spark for distributed text analysis.  

---

## Key Takeaways
- MapReduce provides a **scalable approach** to text analytics, enabling efficient processing of large datasets.  
- Integration with Spark allows for **flexible schema handling** and structured queries via SQLContext.  
- This project highlights the ability to combine **data engineering techniques** with **data science workflows**, making it relevant for real-world applications in big data environments.  
