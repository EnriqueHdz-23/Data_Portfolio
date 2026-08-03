# Sentiment Analysis with Gemini API

This project demonstrates the use of **Google Gemini API** to classify survey responses into sentiment categories. The workflow integrates API calls, error handling, and incremental saving of results, showcasing practical experience in applied Natural Language Processing (NLP) with cloud-based AI services.

---

## script_EHG

### Objective
Implementation of a script to **automatically classify text responses** into three sentiment categories: Positive, Negative, and Neutral. The goal is to leverage Gemini’s generative models to process survey data efficiently while respecting API usage limits.

### Libraries Used
- **csv** – reading and writing survey data  
- **os** – file and environment variable handling  
- **time** – managing pauses between API calls  
- **getpass** – secure input for API keys  
- **google.generativeai** – Gemini API client  

### Dataset
Survey responses stored in a CSV file (`respuestas_encuesta.csv`).  
Each record contains an **ID** and a **response text** to be classified.  
The output is saved in `resultados_sentimiento.csv` with sentiment labels.

### Main Results
- Successfully connected to **Gemini API** using secure API key management.  
- Implemented robust error handling and retry logic for API rate limits and timeouts.  
- Classified responses into **Positive, Negative, Neutral** categories.  
- Generated summary statistics of sentiment distribution across the dataset.  
- Results stored incrementally to avoid data loss during execution.  

---

## Key Takeaways
- Demonstrates integration of **cloud-based AI services** into data science workflows.  
- Highlights practical skills in **API management, error handling, and automation**.  
- Provides a scalable approach to sentiment analysis for survey or customer feedback data.  
- Reinforces ability to combine **Python scripting, NLP, and cloud AI models** for real-world applications.  
