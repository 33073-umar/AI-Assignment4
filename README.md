# Fraud Detection and Sentiment Analysis with Meta Ensemble Models

This repository contains three different datasets and the corresponding machine learning models developed to analyze them. Each dataset represents a distinct type of data: numerical, image, and text. For each dataset, various machine learning models were trained, and a meta ensemble model with hyperparameter tuning was employed to improve performance.

## Datasets and Models

### 1. Fraud Detection Dataset
This dataset contains transaction data with labeled fraud and non-fraud transactions. The following features are included:

- **step**: A unit of time where 1 step equals 1 hour
- **type**: Type of online transaction
- **amount**: The amount of the transaction
- **nameOrig**: Customer initiating the transaction
- **oldbalanceOrg**: Balance before the transaction
- **newbalanceOrig**: Balance after the transaction
- **nameDest**: Recipient of the transaction
- **oldbalanceDest**: Initial balance of recipient before the transaction
- **newbalanceDest**: New balance of recipient after the transaction
- **isFraud**: Indicator if the transaction is fraudulent

**Models Trained:**
- Artificial Neural Network (ANN)
- Decision Tree (DT)
- Meta Ensemble Model with Grid Search Hyperparameter Tuning

### 2. OCR Image Dataset
This dataset contains images of letters and numbers used for Optical Character Recognition (OCR).

**Models Trained:**
- Convolutional Neural Network (CNN)
- Support Vector Machine (SVM)
- Meta Ensemble Model with Grid Search Hyperparameter Tuning

### 3. Drug Review Dataset
This dataset includes patient reviews of medications, including the following features:

- **Drug Name**: The medication the review is about
- **Condition**: The medical condition the medication is intended to treat
- **User ID**: Anonymized identifier for the patient who left the review
- **Date**: The date the review was submitted
- **Rating**: A score (1-10) reflecting the patient's overall satisfaction with the medication
- **Content**: The patient's free-text review detailing their experience

For this dataset, only **Content** and **Rating** were used to perform sentiment analysis.

**Models Trained:**
- Naive Bayes (NB)
- Artificial Neural Network (ANN)
- Meta Ensemble Model with Grid Search Hyperparameter Tuning
