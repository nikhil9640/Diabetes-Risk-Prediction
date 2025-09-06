# Diabetes-Risk-Prediction
Diabetes is one of the most common chronic diseases worldwide, often resulting from a combination of genetic, lifestyle, and clinical factors. Early detection of individuals at risk can help reduce complications through timely interventions such as lifestyle modification and medical treatment. 
Machine learning models can support risk assessment and decision-making by identifying patients at higher risk of developing diabetes.

**Objective**
The primary goal of this project is to predict the risk of diabetes based on patient data, including demographics, medical history, clinical features and lifestyle factors. 
We use logistic regression as the baseline classification model to estimate the probability of developing diabetes.

# Dataset Overview
The dataset, such as framingham.csv. It contains clinical and lifestyle records.
Target variable: diabetes (0 = no diabetes, 1 = diabetes).

**Features include:**
Demographics (age, sex, education)
Lifestyle (smoking status, cigarettes per day)
Medical history (hypertension, blood pressure, cholesterol, BMI, glucose, etc.)

**Methodology:**

Step 1: Data Exploration
Inspect dataset shape, columns, and missing values.
Visualize diabetes distribution (imbalanced dataset).

Step 2: Data Preprocessing
Handle missing values (median for numeric, mode for categorical).
Encode categorical features using One-Hot Encoding.
Normalize numerical features with StandardScaler.

Step 3: Model Training (Logistic Regression)
Train-test split (80/20, stratified).
Logistic Regression with class_weight="balanced" to handle imbalance.
Fit the model on training data.

Step 4: Evaluation
Metrics: Accuracy, Precision, Recall, F1-score.
Confusion Matrix for misclassification patterns.
ROC Curve & AUC, Precision-Recall Curve & Average Precision Score.

Step 5: Feature Importance (optional)
Interpret logistic regression coefficients.
Permutation importance to identify top predictors.

# Proposed Model
Logistic regression was selected as the baseline predictive model because:
It is interpretable (coefficients reflect feature importance).
It works well with binary classification tasks.
It handles imbalanced datasets when class weights are adjusted.

# Conclusion
Logistic regression provides a baseline predictive model for diabetes risk.
Despite class imbalance, the model achieves reasonable recall and ROC-AUC,making it is useful for screening high-risk individuals.

**Future improvements:**
Experiment with advanced models (Random Forest, XGBoost, Neural Networks).
Apply SMOTE or other resampling techniques to handle imbalance.
Use larger, more diverse datasets for better generalization.
