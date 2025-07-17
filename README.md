🕵️‍♂️ Credit Card Fraud Detection
Detect fraudulent credit card transactions using machine learning models on a real-world dataset. The pipeline includes data preprocessing, handling class imbalance, training classification models, and evaluating model performance using standard metrics.

📂 Dataset
Source: Kaggle - Credit Card Fraud Detection Dataset

Description: Contains transactions made by European cardholders in September 2013.

Total Records: 284,807

Fraudulent Transactions: 492 (highly imbalanced)

📊 Features
Time, Amount: Raw features

V1 to V28: Principal components obtained with PCA

Class: Target variable (0 for legit, 1 for fraud)

⚙️ Project Workflow
Data Loading

Upload and unzip dataset if needed.

Exploratory Data Analysis

Class imbalance visualization.

Preprocessing

Feature scaling on Time and Amount.

Imbalance Handling

Under-sampling using RandomUnderSampler.

Model Training

Logistic Regression

Random Forest

Support Vector Machine (SVM)

Evaluation

Classification Report (Precision, Recall, F1-score)

Confusion Matrix

ROC-AUC Score & ROC Curve plot

🧪 Libraries Used
text
Copy
Edit
numpy
pandas
matplotlib
seaborn
scikit-learn
imbalanced-learn
🚀 How to Run (on Google Colab)
Open the notebook in Google Colab

Upload creditcard.csv or creditcardfraud.zip

Run all cells sequentially

📈 Output Example
Model performance metrics

ROC-AUC comparison between classifiers

Visual plots of ROC curves and confusion matrices

📁 File Structure
scss
Copy
Edit
.
├── creditcard.csv (or ZIP)
├── credit_card_fraud_detection.ipynb
└── README.md
🧑‍💻 Author
Anshumaan Singh
anshuls2105@gmail.com
