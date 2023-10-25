
# Project： Detecting the difficulty level of French texts
# DMML2022_Ouchy
---

## Table of Contents
0. Team participant
1. Description
2. Approach
3. Results
4. Video
---

## 0. Team participant
Jingmin Wang

---

## 1. Description
To improve one's foreign language level, reading text suit for the reader's level is an efficient way. This project built a model for English speakers that predicts the difficulty of a French written text. This can be used in a recommendation system to recommend texts for readers.

---

## 2. Approach
To find the best model for French level detection, I followed these steps:

1. **Text Preparation**. During text preparation, French sentences were tokenized. Data cleaning was also conducted in this step.
2. **Text Representation**.  During this step, text data was represented numerically for further process. I tryed Bag of Words, tf-idf, and Doc2Vec. I choose Tf-idf based on the performance and convenience.
3. **Text Classification**. There are different models for text classification. The commonly used ones include: Logistic regression, KNN, Decision Tree, Random Forest, and LinearSVC. In the code, I compared the performance of these models and found the results below.

---

## 3. Results table

Results without Data Cleaning
| Classifier      | Accuracy | Precision     | Recall | F1_Score |
| :---        |    :----:   |    ---: |    :----:   |    ---: |
| Logistic Regression      | 0.4740      | 0.4670   |  0.4740  | 0.4671      | 
| KNN   | 0.3531      | 0.3825      |   0.3531   |  0.3268    |
| Decision Tree   |    0.3396      | 0.3360      |   0.3396    |  0.3366  |
| Random Forest   |   0.4000  | 0.3924      |   0.4000  |   0.3867  |
| LinearSVC      | 0.6729      | 0.6680   |   0.6729  |  0.6667  ||

Results with Data Cleaning
| Classifier      | Accuracy | Precision     | Recall | F1_Score |
| :---        |    :----:   |    ---: |    :----:   |    ---: |
| Logistic Regression      | 0.4333      | 0.4268   |  0.4333  | 0.4280      | 
| KNN   | N/A      | N/A      |   N/A   |  N/A    |
| Decision Tree   |    0.3177      | 0.3166      |   0.3177    |  0.3095  |
| Random Forest   |   0.3781  | 0.3975      |   0.3781  |   0.3629  |
| LinearSVC      | 0.6521      | 0.6506   |   0.6521  |  0.6420  ||
---

## 4. Explainatory video link
https://youtu.be/ixKY8vbWjoE
