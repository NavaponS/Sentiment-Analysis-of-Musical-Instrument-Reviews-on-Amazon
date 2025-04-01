# Sentiment-Analysis-of-Musical-Instrument-Reviews-on-Amazon
NLP using Python (Logistic Regression, K-NN) 

This study analyzes customer sentiment in the Musical Instruments category on Amazon, classifying reviews into three categories Neutral, Negative, and Positive. The dataset, Amazon Musical Instruments Reviews from Kaggle, contains 10,261 reviews collected between 2004 and 2014. The study compares the performance of K-Nearest Neighbors (K-NN) and Logistic Regression models. After optimizing parameters, **K-NN achieved accuracy 65.38%**, while Logistic Regression achieved 95%. Additionally, Logistic Regression outperformed K-NN in other metrics, with precision of 95% and recall of 94.66%, compared to K-NN's Precision of 77.44% and recall of 66.76%. These results demonstrate that Logistic Regression is more accurate and efficient in classifying customer reviews.

![image](https://github.com/user-attachments/assets/6e9abd5b-1bc4-48d1-b04e-c56fdb52a718)

# Cleaning and Preparing Data
- mix reviewText and summary column together
- drop column that unnassesary
- drop rows with missing values
- transform score into sentiments
  - 1-2 : negative
  - 3 : neutral
  - 4-5 : positive
- Preprocessing
  - remove number
  - remove punctuation
  - remove extra white spaces
  - remove nonEng
  - remove stopwords
  - lemmatization
- label encoder
  - 2 - positive, 1 - negative, 0 - neutral
- SMOTE
- tfidf_vectorizer
- split data by using hold-out method train 75% test 25%

# 🎵 Sentiment Analysis of Musical Instrument Reviews on Amazon  
**NLP using Python (Logistic Regression, K-NN)**  

## 📌 Overview  
This study analyzes **customer sentiment** in the **Musical Instruments** category on Amazon, classifying reviews into three categories:  
✅ **Positive**  
➖ **Neutral**  
❌ **Negative**  

The dataset, **Amazon Musical Instruments Reviews** from Kaggle, contains **10,261 reviews** collected between 2004 and 2014. The study compares the performance of **K-Nearest Neighbors (K-NN)** and **Logistic Regression** models.  

🔹 **Model Performance:**  
- **K-NN**: **Accuracy 65.38%**  
- **Logistic Regression**: **Accuracy 95%** 🎯  

Logistic Regression outperformed K-NN in all metrics:  
| Model | Accuracy | Precision | Recall |
|--------|----------|-----------|--------|
| Logistic Regression | 95% | 95% | 94.66% |
| K-NN | 65.38% | 77.44% | 66.76% |

These results indicate that **Logistic Regression is more accurate and efficient** in classifying customer reviews.  

---

## 🛠️ **Data Cleaning & Preparation**  
✔ **Combining** `reviewText` and `summary` columns  
✔ **Dropping unnecessary columns**  
✔ **Removing rows** with missing values  
✔ **Transforming review scores** into sentiment labels:  
  - `1-2` → ❌ Negative  
  - `3` → ➖ Neutral  
  - `4-5` → ✅ Positive  

---

## 🔄 **Preprocessing Steps**  
✔ **Text Cleaning:**  
   - Remove numbers, punctuation, and extra white spaces  
   - Remove non-English words  
   - Remove stopwords  
   - Apply **lemmatization**  

✔ **Encoding Labels:**  
   - `2` → ✅ Positive  
   - `1` → ❌ Negative  
   - `0` → ➖ Neutral  

✔ **Handling Imbalanced Data:**  
   - Applied **SMOTE (Synthetic Minority Over-sampling Technique)**  

✔ **Feature Engineering:**  
   - Used **TF-IDF Vectorization** for text representation  

✔ **Splitting Data:**  
   - **Hold-out method** → **Train 75% / Test 25%**  

