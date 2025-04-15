Handling Class Imbalance
This project explores different techniques to handle class imbalance in credit card fraud detection,.

Resampling Techniques Implemented
1. Oversampling
RandomOverSampler: Duplicates random minority class (fraud) instances to balance the dataset

SMOTE (Synthetic Minority Oversampling Technique): Creates synthetic fraud cases by interpolating between existing ones

2. Undersampling
RandomUnderSampler: Randomly reduces majority class (normal transactions) instances

NearMiss: Intelligent undersampling that keeps strategically selected normal transactions (versions 1-3 implemented)

3. Combined Approach (SMOTEENN)
SMOTE + ENN: Hybrid method that:

Oversamples minority class using SMOTE

Cleans data using Edited Nearest Neighbors (removes ambiguous samples from both classes)

Key Features
Comprehensive comparison of resampling strategies

StandardScaler integration for distance-based methods

Pipeline implementation for reproducible workflows

Detailed class distribution visualization

Model evaluation with appropriate metrics (precision, recall, F1-score)

Technical Stack
Python 3.x

Scikit-learn, imbalanced-learn

Pandas, NumPy for data handling

Matplotlib, Seaborn for visualization

Usage
Clone repository

Install requirements: pip install -r requirements.txt

Run Jupyter notebook: fraud_detection_resampling.ipynb

Note: Dataset expected in data/creditcard.csv
