# 🧠 Medicine Recommendation System

## 🔗 Dataset
https://docs.google.com/spreadsheets/d/1dQrY8D94yewQ0BbchliSYsGjv1Pw6y_IvFEGpm1kjbE/edit?usp=sharing

---

## 📌 Project Overview
This project develops a **medicine recommendation system** using patient review data. The system suggests relevant drugs based on a user’s input health condition by analyzing patterns in historical medical reviews.

It combines **Natural Language Processing (NLP)** and **similarity-based machine learning** to provide intelligent recommendations.

---

## 📊 Dataset Description
The dataset contains real-world patient reviews of medicines with the following attributes:

- **uniqueID** – Unique identifier for each review  
- **drugName** – Name of the drug  
- **condition** – Medical condition treated  
- **review** – Patient’s textual feedback  
- **rating** – Drug rating (1–10)  
- **date** – Review date  
- **usefulCount** – Number of users who found the review helpful  

- Total Records: **53,766**
- Data Type: Structured + Unstructured (text)

---

## ⚙️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 🔍 Exploratory Data Analysis
The following analyses were performed:

- Distribution of drug ratings  
- Most frequently reviewed drugs  
- Most common medical conditions  
- Relationship between rating and usefulness  

---

##  Model Description

### 🔹 Approach
A **content-based filtering system** is used.

### 🔹 Steps:
1. Text data (conditions) is converted into numerical vectors using **TF-IDF**
2. User input condition is vectorized
3. **Cosine similarity** is computed between input and dataset
4. Drugs associated with most similar conditions are recommended

---

## 🧪 Example Workflow

```python
user_condition = input("Enter your health condition: ")
