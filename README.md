<div align="justify">
  
# Incident Classifier with Machine Learning in Cybersecurity 🛡️ 
</div>

<div align="justify">
  
## Objective
Develop a machine learning model to accurately classify cybersecurity incidents into specific types, addressing class imbalance using techniques like SMOTE, and deploy the solution through a Streamlit app for real-time, accessible incident prediction and response support.  

## Dataset 

Contains features like source and destination IPs, protocols, timestamps, and other network attributes capturing incident patterns. <br>
Target: incident_category, with labels such as malware, phishing, and network attacks.

## Business Use Case
 Enhances SOC efficiency by enabling quick incident classification, uncovering attack trends for threat intelligence, and generating real-time automated reports.



##  Approach

### Data Preparation & Exploration

Performed thorough data cleaning to handle missing and inconsistent values, followed by exploratory data analysis (EDA) to uncover incident trends, attack patterns, and feature correlations through visualizations.

### Data Balancing

Addressed class imbalance using SMOTE and SMOTE-ENN, improving minority class representation and removing noise. Post-balancing, model accuracy improved from 0.60 to 0.68, and F1-scores across classes became more consistent.

### Feature Engineering

Selected key attributes such as `source_IP`, `destination_IP`, `protocol`, `timestamp`, and `severity`, and encoded categorical data for model compatibility.

### Model Training & Evaluation

Tested multiple algorithms — Random Forest, SVM, Logistic Regression, Decision Tree, XGBoost, and LightGBM — evaluated using accuracy, precision, recall, and macro-F1 score.

* 🏆 Best Model: Random Forest
* Accuracy: 0.70 Macro-F1: 0.67 Precision: 0.70 Recall: 0.66

### Deployment

Deployed the final Random Forest model using Streamlit, enabling real-time incident classification via an intuitive, web-based interface for SOC teams.

### Results Summary

| Model               | Macro-F1 | Precision | Recall |
| ------------------- | -------- | --------- | ------ |
| Random Forest       | 0.84     | 0.82      | 0.81   |
| SVM                 | 0.81     | 0.79      | 0.77   |
| Logistic Regression | 0.76     | 0.75      | 0.74   |


**🧾Note:** Go through the report in the files for a detailed explanation of the approach.  



## Conclusion

The Random Forest model proved most effective for cybersecurity incident classification, offering high accuracy and scalability for SOC teams. By automating incident categorization, it enables faster, more strategic responses and strengthens organizational resilience against evolving cyber threats. This solution provides a robust, adaptable framework to enhance proactive risk management in an ever-changing digital landscape.

## How to Use

Clone the repository:

```bash
git clone https://github.com/root-x-rohan/cyber-incident-classifier-ML.git
```

## Install dependencies:

```bash
pip install -r requirements.txt
```

### Run the app:

```bash
streamlit run app.py
```

## 🧾Note
Engage via Pull Requests 🔄

</div>
