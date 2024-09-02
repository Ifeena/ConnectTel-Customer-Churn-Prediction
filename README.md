# ConnectTel-Customer-Churn-Prediction

# Project Overview
- The ConnectTel Customer Churn Prediction project aimed to develop a predictive model capable of accurately identifying customers at risk of churning. This project involved multiple stages, including Data Cleaning and Preparation, Exploratory Data Analysis (EDA), Feature Engineering, Model Selection, Training and Validation, and Model Evaluation. The goal was to optimize the model's performance to help ConnectTel enhance its customer retention strategies by reducing false negatives and improving the identification of customers likely to churn.

# Steps Taken:
### 1. Problem Definition
- ConnectTel needed a solution to predict customer churn effectively to maintain its customer base.
- Develop a machine learning model that accurately identifies customers likely to churn, focusing on reducing false negatives.
### 2. Data Cleaning and Preparation
- I handled missing values using median value of the affected feature to replace the missing values, and ensured that features were well-prepared for analysis.
-  The dataset was clean and ready for in-depth analysis and modeling.
### 3. Exploratory Data Analysis (EDA)
- Conducted Univariate, Bivariate, and Multivariate Analysis on key features, visualizing relationships and exploring correlations.
- Insights were gained into feature distributions and their relationships with the target variable (churn), guiding subsequent feature engineering and model selection.
### 4. Feature Engineering
- Encoded categorical variables using LabelEncoder, created new features where necessary, and ensured the numerical nature of features was preserved.
- The features were well-engineered, allowing the models to learn from the data effectively.
### 5. Model Selection, Training, and Validation
- I trained and tested several models, including Logistic Regression, XGBoost, RandomForestClassifier, and DecisionTreeClassifier. The process included:
  - Initial Model Training: Established a baseline for performance.
  - Feature Scaling: Applied standard scaling to improve model performance.
  - Addressing Class Imbalance: Used techniques like class weight to handle class imbalance, focusing on improving recall for the positive class (churn).
  - Hyperparameter Tuning: Fine-tuned models to achieve better balance between precision and recall.
- XGBoost emerged as the top-performing model with an F1 score of 0.65 for the positive class and an overall accuracy of 78%.
### 6. Model Evaluation
- Evaluated the models using confusion matrices, precision, recall, and F1 score (mean CV F1-score), focusing on reducing false negatives.
- The XGBoost model was particularly effective in identifying churn cases, aligning well with ConnectTel’s objectives.
### 7. Submission
- Published the Jupyter Notebook to GitHub, documented the process, and provided recommendations for future work.
- The project was successfully completed and submitted.

# Challenges I Faced and Overcoming Them
- Throughout the project, I encountered several challenges, including:
### 1. Struggling with Multivariate Analysis of Categorical Features
  - Uncertainty about whether to perform a multivariate analysis of categorical features.
  - Decide the best approach to gain meaningful insights.
  - After research and consultation with facilitators, I chose to proceed with insights I got from the Univariate and Bivariate Analysis of the categorical features.
  - This decision provided deeper insights into the relationships between features and the target variable and to streamline the process and focus on feature engineering, preparing the data for the next steps in modeling.
### 2. Data Splitting Dilemma
  - Uncertainty about the appropriate data split ratio.
  - Choose a split that balances training and testing needs.
  - After considering the dataset size and reviewing best practices as well as consulting with faciltators, I opted for an 80-20 split.
  - The chosen split ensured sufficient data for training and reliable testing results.
### 3. Feature Engineering Uncertainty
  - Difficulty in deciding which new features to create.
  - Enhance the dataset with meaningful features.
  - I referenced the WMDI and class recordings and industry practices to guide my decisions.
  - The features created improved model performance, particularly in capturing patterns related to churn.
### 4. Order of Model Training and Evaluation
  - Uncertainty about the sequence of model training steps.
  - Determine the most effective order for model training, evaluation, and validation.
  - I followed a structured approach: initial training, scaling, addressing class imbalance, and hyperparameter tuning.
  - This systematic approach led to steady improvements in model performance.
### 5. Metric Selection for Model Evaluation
  - Difficulty in identifying the most relevant evaluation metrics.
  - Choose metrics that align with business objectives, focusing on reducing false negatives.
  - After reviewing project goals and consulting with facilitators, I prioritized precision, recall, and F1 score.
  - This focus allowed me to align model evaluation with ConnectTel’s customer retention goals.
### 6. Deciding When to Stop Model Training
  - Uncertainty about whether to continue improving the model.
  - Balance the need for further improvements with diminishing returns.
  - After analyzing incremental improvements and consulting with peers, I decided to finalize the model at a point where XGBoost achieved satisfactory performance.
  - The decision to stop at this point provided a robust model without overfitting.

# Key Achievements
- XGBoost Performance: After hyperparameter tuning, XGBoost emerged as the top-performing model, with an F1 score of 0.65 and an accuracy of 78%, effectively reducing false negatives.
- Enhanced Recall: By addressing class imbalance, the recall for the positive class was significantly improved, aligning with the project’s goal of minimizing false negatives.

# Recommendations for Future Work
- Further Model Refinement: Explore advanced techniques to capture more complex patterns in the data.
- Data Augmentation: Incorporate additional features for deeper insights into churn behavior.
- Real-time Monitoring: Implement a real-time monitoring system to continuously assess and mitigate churn risk.

# Conclusion
- This project successfully identified a robust model for predicting customer churn. While challenges were encountered, the solutions applied provided valuable learning experiences and laid a strong foundation for ConnectTel’s future customer retention strategies.
