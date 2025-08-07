#💳 Fraud Detection Using XGBoost & Random Forest with SMOTE + Hyperparameter Tuning
This project builds and compares XGBoost and Random Forest classifiers for detecting fraudulent financial transactions in a highly imbalanced dataset. It integrates SMOTE for class balancing, and uses HalvingRandomSearchCV for efficient hyperparameter optimization. Built entirely in a Google Colab notebook, the project demonstrates an end-to-end ML pipeline including preprocessing, model training, evaluation, and tuning.

#🔍 Problem Statement
In financial datasets, fraudulent transactions are rare (typically <1%) and traditional classifiers struggle due to this imbalance. This project addresses the issue by combining oversampling and ensemble learning techniques to build robust fraud detection models.

#✅ Key Features
⚖️ SMOTE Oversampling: Generates synthetic samples for the minority fraud class to improve model learning.

🌲 Random Forest Classifier: A bagging-based ensemble model known for its robustness and interpretability.

⚡ XGBoost Classifier: A fast and accurate gradient boosting model tailored for structured data.

🔁 Pipeline Integration: Clean, modular imblearn pipeline using Pipeline to combine preprocessing, SMOTE, and classifier.

⚙️ HalvingRandomSearchCV: Efficient hyperparameter tuning algorithm that eliminates poor configurations early.

#📊 Evaluation Metrics: Includes ROC-AUC, average precision score, confusion matrix, and classification report.

#📊 Dataset Features
step: Hour of the transaction (from 1 to 744)

type: Transaction type (PAYMENT, TRANSFER, CASH_OUT, etc.)

amount: Transaction value

nameOrig, nameDest: Originator and destination identifiers (masked)

oldbalanceOrg, newbalanceOrig: Originator's balance before/after

oldbalanceDest, newbalanceDest: Destination's balance before/after

isFraud: Binary target (1 = fraud, 0 = normal)

