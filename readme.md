# Week 2 - Halfday 5

## Missions & Activities:

### Activity 1 – ~30 minutes
- **Peer Review and Validation of Data Analysis (Halfday 4)**: Work in pairs to review and compare your code and results. Exchange the outcome of the previous activity and discuss your approach. Write together 1-2 slides with a list of the key-differences concerning:
    - The result you had
    - The method you used to get to that results
- **Consolidation by the Professor**: After peer review, the professor will provide further clarification and consolidation of the concepts.

### Activity 2
- **Problem**:
  - **Goal**: Proper evaluation of a *regression* model.
  - **Idea**: Restart from scratch, this time, the goal is to predict the age of the passengers (instead of predicting if they survived or not). In other terms, change target variable `y` from `Survived` to `Age`).
- **Hint**: The preprocessing of the data is *almost* the same as before. Some passanger have missing values on the Age column. Be sure of not using them for training. For regression use [this model](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html).
- **Tools**: scikit-learn, Random Forest Regressor
- **New/Consolidation of ML Glossary**: Mean Squared Error, Root Mean Squared Error, Mean Absolute Error

### Activity 3 – ~1 hour
- **Weekly Evaluation**:
  - **Hints**: Review the questions and concepts covered throughout the week.
  - **Tools**: MCQ + open questions in Moodle

## Expected Outcomes:
- **Activity 2**: A new Jupyter notebook for regression. Provide direct answers to **all** the questions listed below (Section [Questions](#questions)).
- **Activity 3**: A grade for the students based on the weekly evaluation.

## Tasks – Regression (Random Forest)
1. **Implement RF Regression Using scikit-learn**:
   - Find the best hyperparameters for RF using grid search and k-fold cross-validation.
   - [Optional] Previously you probably imputed some missing ages. Now you used a full regression algorithm to predict them. Compare the imputation vs the prediction.  
2. **Evaluate the Performance**:
   - Calculate Mean Squared Error, Root Mean Squared Error, and Mean Absolute Error.
     - **Hint**: Here we talk about errors. The lower, the better!
   - Identify and print the most important features according to RF and compare them with your earlier correlation analysis.

## Questions:
- Do Random Forest Classifier and Random Forest Regressor have the same hyperparameters? What are the differences?
- Now that my target variable is a continue variable (float), should I rescale/standardize it? why?
- Quickly present the metrics you used for regression. In your research, did you find any other metrics in addition of the metrics mentioned above?
- You trained your Regressor. Now you need to predict the age of a new, unseen passenger. In your data preparation you probably normalized/rescaled the data. This means that an additional step is required when predicting new values (e.g., for `age`). What is it, and why is it necessary?

---

## Acquired Competences (Week 2)
- **Explore a dataset and properly implement and evaluate a simple classification or regression pipeline using Random Forest**:
  - Analyze a dataset to understand its characteristics, including features available, target variable, balance/unbalance, correlation analysis, missing values, outliers, etc.
  - Preprocess a dataset correctly for regression and classification analysis using supervised approaches.
  - Evaluate a machine learning model to provide a quantitative estimation of its performance using the most suitable metrics for the problem and the data.