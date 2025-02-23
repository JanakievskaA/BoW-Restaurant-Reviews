# **Sentiment Analysis using Bag of Words and Machine Learning**

This project performs **sentiment analysis** on restaurant reviews using **Natural Language Processing (NLP)** and the **Bag of Words (BoW)** model. The text is preprocessed, converted into numerical features, and classified using **Naive Bayes, K-Nearest Neighbors (KNN), and Logistic Regression**.

---

##  **Project Overview**
1. **Loading the Dataset**  
   - The dataset is in **TSV format** and is loaded using `pandas`.  
   - It contains **restaurant reviews** labeled as **positive (1)** or **negative (0)**.  
   
2. **Text Preprocessing**  
   - Removes **non-alphabetic characters**.  
   - Converts text to **lowercase**.  
   - Tokenizes and removes **stopwords**, except `"not"` to preserve sentiment.  
   - Applies **stemming** using `PorterStemmer`.  
   - Stores the cleaned reviews in a `corpus` list.  

3. **Feature Extraction (Bag of Words Model)**  
   - Uses `CountVectorizer` to transform text into a **numerical matrix**.  
   - Selects the **top 1000 most frequent words** as features.  

4. **Splitting Data**  
   - The dataset is split into **80% training** and **20% testing** using `train_test_split`.  

5. **Machine Learning Models**  
   - **Naive Bayes**  
   - **K-Nearest Neighbors (KNN)**  
   - **Logistic Regression**  

6. **Model Evaluation**  
   - Uses **confusion matrix** and **accuracy score** to evaluate performance.  

