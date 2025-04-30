# Vision-Health-Clinic
Capstone Project: Diabetes Prediction Model
Project Overview:
The goal of this project is to develop a solid diabetes prediction model that helps Vision Health Clinic identify patients at risk of developing diabetes. This will enable timely intervention and reduce healthcare costs.
The dataset used for this project is diabetes_prediction_dataset.csv, which contains patient data and relevant features that will help predict the likelihood of diabetes onset.

Steps to Complete the Task:
1. Data Collection
Dataset Used: diabetes_prediction_dataset.csv

The Diabetes Prediction Dataset used in this project is utilized to predict the likelihood of diabetes onset based on various health-related factors.

It contains features such as age, glucose levels, blood pressure, BMI, etc., along with a target variable indicating whether a person has diabetes or not.

2. Exploratory Data Analysis (EDA)
Handling Missing Values: Checked for missing data and there weren't any.

I began by performing an Exploratory Data Analysis (EDA) to understand the dataset and its structure. This step helped me identify patterns, trends, and issues in the data.

Key Analyses Performed:
Univariate Analysis: Analyzed individual features in the dataset.

Visualized the distribution of individual features like Blood Glucose Level, BMI, and Hemoglobin using boxplots.

Examined the spread and central tendency of continuous variables (mean, median, standard deviation).

Bivariate Analysis: Explored relationships between pairs of features.

Plotted column charts like column charts to identify relationships between variables such as Smoking history vs. Label(Diabetes), Age Group vs Label(Diabetes), Gender vs. Label(Diabetes).

Investigated the relationship between the target variable (diabetes outcome) and other features to check for dependencies.

Multivariate Analysis: Analyzed interactions between multiple variables.

Used heatmaps to study the interactions between more than two features and their relationship with the target variable.

Examined how combinations of features (e.g., Glucose, BMI, Age) impact diabetes prediction.

Tools/Packages Used:

Pandas, Matplotlib, Seaborn for data manipulation and visualization.

3. Data Preprocessing and Machine Learning
The dataset required several preprocessing steps before it could be used for machine learning models:

Feature Engineering:

Some features were normalized or scaled to bring them to the same scale e.g. outliers like Blood Glucose Level, BMI, and Hemoglobin

I also created new features if needed for better model performance.

Feature Selection: I removed highly correlated features or features that weren't contributing to the model’s performance.

Train-Test Split: The data was split into training and testing sets (80% for training, 20% for testing) using train_test_split from Scikit-learn.

4. Model Selection
I used multiple machine learning models to predict diabetes onset:

Logistic Regression: A baseline model to understand the relationship between the features and the target.

Random Forest Classifier: A powerful ensemble method that helps to capture non-linear relationships in the data.

XGBoost Classifier: A more advanced boosting algorithm known for its strong predictive performance.

K-Nearest Neighbors: A simpler yet effective model for classification.

Support Vector Classifier (SVC): A model for high-dimensional data with a non-linear decision boundary.

SGD Classifier: Used for large-scale machine learning tasks, leveraging stochastic gradient descent.

5. Model Evaluation
Metrics Used:

Accuracy: The proportion of correctly predicted instances.

Precision: The proportion of positive predictions that were actually correct.

Recall: The proportion of actual positives that were correctly predicted.

ROC-AUC: Measures the area under the ROC curve, providing an indication of model performance across all thresholds.

Confusion Matrix: Plotted confusion matrices for each model to visually assess their performance in terms of true positives, false positives, etc.

Cross-validation was also performed on the models to ensure that the performance is generalized and not overfitted.

6. Model Tuning and Optimization
I performed hyperparameter tuning using grid search and random search to optimize the models for better accuracy and performance.

For models like XGBoost and Random Forest, parameters such as max_depth, learning_rate, and n_estimators were tuned.

7. Final Model Selection
After comparing all models, XGBoost Classifier gave the best results in terms of accuracy, precision, recall, and ROC-AUC.

It was selected as the final model for diabetes prediction.

8. Conclusion
The selected XGBoost model achieved the best performance and was able to predict diabetes onset with high accuracy.

The model will help Stark Health Clinic identify individuals at risk of diabetes, enabling timely interventions and reducing healthcare costs.
