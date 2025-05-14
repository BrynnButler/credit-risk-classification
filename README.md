# credit-risk-classification
module 20

# Overview 

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

# The Results

- **Accuracy Score:** 0.93  
- **Precision Score:**  
  - Healthy loans (0): 0.96  
  - High-risk loans (1): 0.68  
- **Recall Score:**  
  - Healthy loans (0): 0.97  
  - High-risk loans (1): 0.59  

# Questions and Answers:

**Question:** How well does the logistic regression model predict both the `0` (healthy loan) and `1` (high-risk loan) labels?

**Answer:** The model does a solid job predicting healthy loans (0) — it’s pretty accurate and catches most of them. But when it comes to high-risk loans (1), it struggles. The precision and recall are both low, which means it's missing a lot of risky borrowers and not predicting that class very confidently.

It seems like the model leans heavily toward predicting loans as healthy, which could be because the dataset has way more healthy loans than risky ones. So while it’s useful for spotting safe bets, I wouldn’t fully trust it to flag high-risk loans without making some improvements.

# Summary

Overall, the logistic regression model performs well at identifying healthy loans, but it’s less reliable at spotting high-risk loans. This is likely due to class imbalance in the dataset. Because of this, I wouldn't recommend using the model as-is for making critical decisions around risky borrowers. It could be improved by balancing the dataset or trying other models better suited for imbalanced data.
