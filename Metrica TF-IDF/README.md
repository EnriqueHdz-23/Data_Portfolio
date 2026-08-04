# TF-IDF Metric Example

This project demonstrates the use of **TF-IDF (Term Frequency–Inverse Document Frequency)** as a text representation technique for Natural Language Processing (NLP). The focus is on transforming raw text into numerical features that can be used in machine learning models.

---

## prueba-TF-IDF_EHG

### Objective
Implementation of a workflow to **vectorize text data using TF-IDF**, highlighting how term frequency and inverse document frequency combine to measure the importance of words in a corpus.  
Extended with a **Naive Bayes classifier** to show practical application in text categorization.

### Libraries Used
- **pandas** – data manipulation and preprocessing  
- **sklearn.feature_extraction.text.TfidfVectorizer** – TF-IDF transformation  
- **sklearn.naive_bayes.MultinomialNB** – text classification  
- **sklearn.model_selection.train_test_split** – dataset splitting  
- **sklearn.metrics.classification_report** – model evaluation  

### Dataset
Synthetic dataset of short text samples labeled as **positive, negative, or neutral**.  
Additional examples included for prediction on unseen text.

### Main Results
- Applied **TF-IDF vectorization** to sample text data.  
- Generated a sparse matrix representation of word importance.  
- Trained a **Naive Bayes classifier** on TF-IDF features.  
- Achieved classification with evaluation metrics (precision, recall, F1-score).  
- Example predictions:  
