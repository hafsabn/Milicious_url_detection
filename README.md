#  Malicious URL Detection using ML and Deep Learning

This project focuses on detecting and classifying **malicious URLs** into multiple categories using both Machine Learning and Deep Learning techniques. It's a cybersecurity-focused project aiming to help systems identify threats based on URL patterns.

##  Dataset

- **Source:** [Kaggle - Malicious URLs Dataset](https://www.kaggle.com/datasets/sid321axn/malicious-urls-dataset)
- **Classes:** The dataset includes **multiple URL types**, such as:
  - Benign
  - Defacement
  - Phishing
  - Malware


##  Approaches

### 1.  Machine Learning Approach

- **Preprocessing:** 
  - URL cleaning and normalization
  - Extracted key characteristics from each URL (e.g., URL length, number of digits/special characters, presence of IP address, etc.)

- **Algorithms Used:**
  - Decision Tree
  - Random Forest
  - K-Nearest Neighbors (KNN)
  - SGD Classifier
  - Naive Bayes

####  Handling Class Imbalance

The dataset was **imbalanced**, so I experimented with:
- **SMOTE** (Synthetic Minority Oversampling Technique)
- **Random Undersampling**

Each algorithm was tested on:
- The original unbalanced dataset
- The balanced versions using SMOTE and using undersampling also



### 2. Deep Learning Approach

- **Model Used:** LSTM (Long Short-Term Memory)
- **Preprocessing:** Tokenized URLs and padded sequences
- **Architecture:** Embedding layer + LSTM + Dense layers
- **Result:** LSTM achieved the **highest performance** with around **98% accuracy** in classifying URLs into multiple categories, and it gives a good results in confusion matrix.



##  What I Learned

- **Data balancing techniques like SMOTE** can significantly improve fairness and accuracy.
- **LSTM performs better on raw URL sequences**, as it learns structural patterns directly.
- **Cybersecurity meets AI**: This project showed how AI can effectively detect phishing, malware, and defacement threats based on URL patterns.
- **Model evaluation must go beyond accuracy** in multi-class settings — precision, recall, and confusion matrices are essential.


## ✅ Conclusion

This project helped me explore and compare different Machine Learning and Deep Learning techniques for **multi-class URL classification**. Through hands-on experimentation, I observed how feature-based ML models perform with traditional algorithms, and how sequence-based models like LSTM can capture deeper patterns in raw URLs. 
