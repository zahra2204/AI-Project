# Fraud Detection System

A machine learning-based fraud detection system that uses Random Forest Classifier to identify fraudulent transactions.

## Features

- Data preprocessing and feature scaling
- Handling of class imbalance using SMOTE
- Model training and evaluation
- Feature importance visualization
- Model persistence and loading
- Prediction capabilities
- Sample dataset generation

## Requirements

- Python 3.8+
- Required packages are listed in `requirements.txt`

## Installation

1. Clone this repository
2. Install the required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Generate sample dataset (optional):
```bash
python generate_sample_data.py
```
This will create a `creditcard.csv` file with 10,000 sample transactions (1% fraud rate).

2. Run the fraud detection system:
```bash
python fraud_detection.py
```

## Project Structure

- `fraud_detection.py`: Main script containing the fraud detection system
- `generate_sample_data.py`: Script to generate sample transaction data
- `requirements.txt`: List of required Python packages
- `feature_importance.png`: Generated visualization of feature importance
- `creditcard.csv`: Sample dataset (generated by generate_sample_data.py)

## Sample Dataset Details

The generated sample dataset includes:
- 28 anonymized features (V1-V28)
- Transaction amount
- Transaction time
- Class label (0 for legitimate, 1 for fraud)
- 10,000 total transactions
- 1% fraud rate
- Realistic patterns in fraudulent transactions

## Model Details

The system uses a Random Forest Classifier with the following features:
- 100 decision trees
- SMOTE for handling class imbalance
- StandardScaler for feature normalization
- Comprehensive evaluation metrics (classification report, confusion matrix, ROC AUC)

## Output

The system generates:
- Classification report
- Confusion matrix
- ROC AUC score
- Feature importance visualization
- Saved model file (fraud_detection_model.joblib)

## Contributing

Feel free to submit issues and enhancement requests. 