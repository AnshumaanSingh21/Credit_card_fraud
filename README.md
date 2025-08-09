# 🕵️‍♂️ Credit Card Fraud Detection

Detect fraudulent credit card transactions using machine learning models on a real-world dataset. This project implements a complete ML pipeline, including data preprocessing, handling class imbalance, model training, and evaluation using standard metrics.

---

## 📂 Dataset

- **Source:** [Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Description:** Contains transactions made by European cardholders in September 2013. Features are PCA-transformed (V1 to V28) for privacy.
- **Total Records:** 284,807  
- **Fraudulent Transactions:** 492 (highly imbalanced dataset)

---

## 📊 Features

- `Time`, `Amount`: Original features (scaled)
- `V1` to `V28`: Principal components
- `Class`: Target variable (0 = Legit, 1 = Fraud)

---

## ⚙️ Project Workflow

1. **Data Loading**
   - Upload the dataset manually or from a zip file
2. **Exploratory Data Analysis**
   - Class distribution visualization
3. **Preprocessing**
   - Scaling `Amount` and `Time` features
4. **Imbalance Handling**
   - Using `RandomUnderSampler` to balance classes
5. **Model Training**
   - Logistic Regression
   - Random Forest
   - Support Vector Machine (SVM)
6. **Evaluation**
   - Classification Report (Precision, Recall, F1-score)
   - Confusion Matrix
   - ROC-AUC Score
   - ROC Curve Visualization

---

## 🧪 Libraries Used

```bash
numpy
pandas
matplotlib
seaborn
scikit-learn
imbalanced-learn
```

## Install missing libraries in Colab using:

python
Copy
Edit
!pip install imbalanced-learn
🚀 How to Run
On Google Colab
Open the Jupyter Notebook in Google Colab

## Upload the dataset (creditcard.csv or zipped version)

## Run each cell in order to preprocess data, train models, and evaluate results

## 📈 Outputs
- Classification reports for each model

- Confusion matrices

- ROC-AUC scores and ROC curve plots

## Performance comparison of Logistic Regression, Random Forest, and SVM classifiers

- 📁 File Structure
- python
- Copy
- Edit
.
- ├── creditcard.csv (or creditcardfraud.zip)
- ├── credit_card_fraud_detection.ipynb
- └── README.md

## Actionable Recommendations & Business Insights

**Based on the model analyses above, the following recommendations are made for financial fraud detection:**

1. **Model Choice:** All three models (Logistic Regression, Random Forest, SVM) perform well. Logistic Regression gives slightly better recall, which is important to reduce missed fraud cases (false negatives).  
   _Recommendation: Use Logistic Regression for initial deployment, but monitor Random Forest performance as well._

2. **Threshold Selection:** By adjusting the decision threshold (see Precision-Recall plot above), recall can be increased to over 95% at the cost of some precision.  
   _Recommendation: Set threshold to 0.55 to maximize fraud detection, and periodically review based on business impact._

3. **Class Imbalance Handling:** Undersampling was used for balance; for larger datasets or in production, consider advanced techniques such as SMOTE or ensemble methods for further improvement.

4. **Operational Safeguards:**  
   - Regularly retrain the model with new data to adapt to evolving fraud patterns.
   - Integrate the model into transaction monitoring systems for real-time alerts.
   - Implement a human-in-the-loop review process for flagged transactions to minimize customer disruption.

5. **Next Steps:**  
   - Test the model on additional datasets from other environments or institutions to ensure robustness and scalability.
   - Monitor key metrics (recall, precision, false positive rate) post-deployment and adjust thresholds as necessary.

**Conclusion:**  
The deployed solution can significantly reduce risk exposure and financial loss by catching more fraudulent transactions, with actionable thresholds tailored to operational needs.

## ✍️ Author
- Anshumaan Singh
- anshuls2105@gmail.com
