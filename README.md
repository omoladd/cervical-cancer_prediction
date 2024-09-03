# Cervical Cancer Prediction
The dataset is multivariate, with  features that cover demographic information, habits, and historical medical records of 858 patients with 36 Features obtained from the  [UCI Machine Learning Repository.](https://archive.ics.uci.edu/dataset/383/cervical+cancer+risk+factors)

# Key Features

- **Demographic Information:** Age, number of sexual partners, etc.
- **Behavioral Habits:** Smoking, use of contraceptives, etc.
- **Medical History:** Number of pregnancies, history of STDs, etc.

# Target Variable

- **Biopsy:** A binary variable indicating the result of a biopsy (1 for positive, 0 for negative).

# Methodology

 1. Data Understanding and Exploration

- **Load and Explore Data:** Import the dataset and understand its structure.
- **Data Cleaning:** Handle missing values using appropriate strategies.
- **Exploratory Data Analysis (EDA):** Visualize data distributions, identify patterns, and understand relationships between features and the target variable.

2. Data Preprocessing

- **Feature Engineering:** Transforming existing features to enhance model performance.
- **Normalization/Standardization:** Scale features to ensure they are on the same scale.
- **Feature Selection:** Identify and select significant features through correlation analysis and model-based techniques (Random Forest)

3. Model Building

- **Model Selection:** Training various machine learning models such as Logistic Regression, Decision Trees, Random Forest, and SVM.

4. Model Evaluation

- **Cross-Validation:** Implement cross-validation to evaluate model performance.
- **Performance Metrics:** Using accuracy, precision, recall, and F1-score to assess model performance.

# Performance Metrics Evaluation
To assess the performance of the models, several metrics were considered:

**Accuracy:** Measures the proportion of correctly predicted instances out of the total instances. While accuracy gives a general idea of the model’s performance, it can be misleading in the case of imbalanced datasets, where one class significantly outweighs the other.

**Precision:** Indicates how many of the predicted positive instances are actually positive. In medical diagnosis, this metric is crucial as it reflects the model’s ability to avoid false positives (misdiagnosing a healthy person as sick).

**Recall (Sensitivity):** This parameter reflects the model’s ability to correctly identify actual positives (patients with the disease). High recall is critical in medical applications because it minimizes the chances of missing a positive case (false negative).

**F1-Score:** The harmonic mean of precision and recall, offering a balance between the two. It is particularly useful when the class distribution is imbalanced.

**Confusion Matrix:** This matrix summarizes the prediction results, detailing the true positive, false positive, true negative, and false negative predictions. It helps one understand the types of errors the model is making.

# Results
The evaluation results of the best-performing model (Voting Classifier) are as follows:

**Accuracy:** 97.92%
The model correctly predicted 97.92% of the cases, indicating a strong overall performance. However, accuracy alone isn't the most reliable metric in medical diagnosis due to the potential for imbalanced data.

**Recall:** 100%
The model identified all actual positive cases of cervical cancer (no false negatives). This is a critical outcome, as it means no potential cases were missed, which is vital in a medical setting.

**Confusion Matrix:**

True Negatives (90): The model correctly identified 90 patients as not having cervical cancer.
False Positives (2): The model incorrectly identified 2 patients as having cervical cancer when they did not.
False Negatives (0): The model correctly identified all cases of cervical cancer.
True Positives (4): The model correctly identified 4 patients as having cervical cancer.

# Interpretation:
The model’s high recall (100%) is particularly important in medical applications, where failing to diagnose a patient who actually has the disease could have severe consequences. The two false positives (patients wrongly diagnosed with the disease) can be further examined with additional medical tests, making this a manageable issue. Overall, the model’s performance is highly acceptable for medical diagnosis, prioritizing the identification of all potential cases of cervical cancer.
