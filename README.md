# Phishing URL Detection Project 

## Objective
My goal with this project is to develop a machine learning model for detecting phishing URLs based on various URL-based features. The goal is to enhance cybersecurity defenses by accurately distinguishing malicious links from legitimate ones using a dataset of labeled URLs. I will be exploring feature engineering, model selection, and evaluation techniques to build a robust classification system.


### Skills Learned

- Data preprocessing and feature engineering for cybersecurity datasets.
- Applying machine learning models for phishing URL detection.
- Model evaluation techniques including precision, recall, and ROC-AUC.
- Handling class imbalance and improving generalization using cross-validation.
- Building and deploying a simple model-based detection system.

### Tools Used

- Python (pandas, scikit-learn, XGBoost, RandomForest) - Data processing, model training, and evaluation.
- Google Colab/Jupyter Notebook - Model development and experimentation.
- Streamlit - Deployment of an interactive web app for URL classification.
- Flask - API-based deployment for real-world integration.

## Steps

# Step 1: Problem Definition & Objectives | Data Preprocessing 
Phishing is one of the most common forms of cyberattacks, and having a system that can automatically detect malicious URLs can help users reduce the risk of compromise at the endpoint and network levels.

For this first step, I wanted to:

- Understand the structure and contents of my dataset.
- Define the classification problem clearly (binary: phishing vs. legitimate).
- Get a feel for the data: what features exist, what cleaning/preprocessing may be needed, and how to begin modeling.

To begin, I loaded and explored my dataset using Google Colab, using pandas to get a basic shape and preview of the data:

![Step 1](https://i.imgur.com/NnSWAnh.png)

Missing data can often break ML models, skew results and cause errors during preprocessing, so I wanted to check for missing values to avoid any complications once we start training our model:

![Step 1](https://i.imgur.com/vN0e2T8.png)

Checking for all the data types in the dataset was also very important, as the wrong data types could cause errors during training:

![Step 1](https://i.imgur.com/vj76HzG.png)
Both of these steps are basically like checking our ingredients before cooking, we wouldn't want spoiled milk or mislabeled spices in the mix.

