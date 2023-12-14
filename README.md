# final-project

### 1 Explain what you do in your project
Created three different classifiers(ExtraTreesClassifier, KNeighborsClassifier, RidgeClassifier)\n
Created VotingClassifier that allow to combine different machine learning models and use a majority vote or a weighted vote to make predictions.\n
Trained the Voting Classifier and made prediction

### 2 Explain the training dataset
X_train, X_test, y_train, y_test = sklearn.model_selection.train_test_split(X, y, test_size=0.3, random_state=0)\n
30% of the data used as the testing set, and the remaining 70% used for training.\n
Sets a random seed for reproducibility. When the same seed is used, the data split will be the same each time the code is executed.\n

### 3 Explain the algorithm you choose
ExtraTreesClassifier: Ensemble method based on decision trees. It builds multiple decision trees and merges their predictions, providing robustness and avoiding overfitting.\n
KNeighborsClassifier: A simple instance-based learning algorithm based on the k-nearest neighbors.\n
RidgeClassifier: A linear classifier that uses Ridge regression to handle multicollinearity in the input features.\n

### 4 Explain hyper-parameter of the function
ExtraTreesClassifier: n_estimators - Number of trees in the forest = 100.\n
  max_depth - Maximum depth of the trees = 1.\n
  max_features - Maximum number of features to consider for the best split = 1.\n
  min_samples_split - Minimum number of samples required to split an internal node = 3.\n
  n_jobs - Number of jobs to run in parallel for fitting and predicting = -1.\n
  random_state - Seed for random number generation for reproducibility = 1774.\n
KNeighborsClassifier: n_neighbors - Number of algorithm consider the nerest neighbor = 1.\n
RidgeClassifier: alpha - Regularization strength, controlling the amount of shrinkage applied = 0.32.
