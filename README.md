# pima-indians-diabetes
Project Title: Exploratory Analysis and Classification of Pima Indians Diabetes Dataset

1. Introduction:

The project aims to explore the Pima Indians Diabetes dataset, understand its characteristics, preprocess the data, build classification models using the Perceptron algorithm, address class imbalance, and optimize model performance.
2. Dataset Overview:

The Pima Indians Diabetes dataset contains various health-related attributes of individuals, along with a binary target indicating the presence or absence of diabetes.
It consists of 768 instances and 9 attributes including features like pregnancy count, glucose concentration, blood pressure, skin thickness, insulin level, BMI, diabetes pedigree function, age, and the target variable class.
3. Data Preprocessing:

Checked for missing values (none found).
Split the data into features and target variables.
Applied Min-Max scaling to normalize the feature values between 0 and 1.
4. Data Splitting:

Split the data into training (60%), testing (20%), and validation (20%) sets.
5. Handling Class Imbalance:

Used the Synthetic Minority Over-sampling Technique (SMOTE) to address class imbalance in the training data.
Demonstrated the improvement in F1 scores for minority class after applying SMOTE.
6. Model Training and Evaluation:

Trained Perceptron models on both original and SMOTE-resampled data.
Evaluated model performance using F1-score on the test set.
Observed improvement in F1 scores for minority class post-SMOTE.
7. Feature Importance Analysis:

Identified and dropped the two least significant predictors based on Perceptron coefficients.
Created a new DataFrame with the dropped columns and retrained the model.
Evaluated model performance on the modified dataset.
8. Hyperparameter Tuning with Grid Search:

Utilized Grid Search with cross-validation to find optimal parameters for SMOTE.
Re-sampled the training data with optimal SMOTE parameters.
Trained a Perceptron model with the optimized parameters.
Evaluated model performance on the test set.
9. Conclusion:

The analysis demonstrates the effectiveness of preprocessing techniques like Min-Max scaling and handling class imbalance using SMOTE in improving the performance of classification models.
Feature importance analysis provides insights into the influential predictors affecting the model's decisions.
Hyperparameter tuning enhances model performance, leading to better classification accuracy and F1 scores.
10. Future Work:

Further exploration could involve trying different classification algorithms and ensemble methods.
Feature engineering or selection techniques could be employed to enhance model interpretability and performance.
Experimentation with more advanced techniques for handling class imbalance, such as adaptive synthetic sampling approaches.
