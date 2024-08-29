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
