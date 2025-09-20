**Objective:** Predict passenger survival (Survived = 0 or 1) using Logistic Regression on the Titanic dataset.  
- **Dataset:** Titanic-Dataset.csv containing passenger details such as Pclass, Sex, Age, SibSp, Parch, Fare, and Embarked.  
- **Preprocessing:**
  - Filled missing numeric values (Age, SibSp, Parch, Fare) with median.  
  - Filled missing categorical values (Sex, Embarked) with mode.  
  - Applied one-hot encoding to categorical features.  
  - Standardized numerical features using z-score normalization.  
- **Model:** Logistic Regression (scikit-learn, solver = lbfgs, max_iter = 1000).  
- **Train/Test Split:** 80% training, 20% testing with stratification.  
- **Results:**
  - Accuracy: ~80% on the test set.  
  - Confusion Matrix (counts):  
    ```
    [[98 12]
     [23 46]]
    ```
  - Higher recall for "Not Survived", lower recall for "Survived" due to class imbalance.  
- **Visualizations:** Histograms and boxplots for feature distributions, Confusion Matrix for performance evaluation.  
- **Report:** LaTeX report (`report.tex`) included, covering dataset, preprocessing, logistic regression theory, and results.  
- **Future Work:**
  - Add feature engineering (family size, titles).  
  - Handle class imbalance (oversampling, class weights).  
  - Compare with advanced models (Decision Trees, Random Forests, Neural Networks).  
