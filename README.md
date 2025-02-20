# Diabetes-Prediction-using-Artificial-Neural-Network-ANN-with-PC
This project implements an Artificial Neural Network (ANN) using the MLPClassifier from scikit-learn to predict diabetes based on the Pima Indians Diabetes dataset. The dataset includes 8 features such as glucose level, blood pressure, BMI, and age, with a binary target variable indicating the presence or absence of diabetes.


Key Steps:
Data Preprocessing:

The dataset is loaded and normalized using StandardScaler.

The data is split into training (80%) and testing (20%) sets.

Model Training:

A simple ANN with one hidden layer (64 neurons) is trained using MLPClassifier.

The model is evaluated on both training and test sets.

Dimensionality Reduction with PCA:

The dataset is reduced from 8 features to 3 principal components using PCA.

The model is retrained and evaluated on the reduced dataset.

Results:

Without PCA: Training accuracy ~80%, Test accuracy ~77%.

With PCA: Training accuracy ~74%, Test accuracy ~73%.

Precision and Recall are also calculated to evaluate the model's performance on imbalanced classes.

Challenges:
The model shows a ConvergenceWarning, indicating it may need more iterations or hyperparameter tuning.

The dataset is imbalanced, leading to lower precision (~49%) despite good recall (~82%).

Suggestions for Improvement:
Increase max_iter or adjust the learning rate.

Use techniques like SMOTE to handle class imbalance.

Experiment with different ANN architectures and hyperparameters.
