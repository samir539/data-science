# Support Vector Machines (SVM)

## Section 1: Data Preparation of the Breast Cancer Wisconsin Dataset

The Breast Cancer Wisconsin (Diagnostic) Dataset is a popular dataset for classification tasks using SVM. Before applying SVM, we need to prepare the data:

1. Load the dataset: Load the Breast Cancer Wisconsin dataset using libraries like pandas.
2. Data Cleaning: Check for missing values and handle them appropriately (e.g., imputation or removal).
3. Feature Selection: Select relevant features and remove unnecessary ones to reduce dimensionality.
4. Data Splitting: Split the dataset into training and testing sets to evaluate the SVM model.

## Section 2: Linear SVM Formulation

SVM is a supervised learning algorithm used for classification tasks. For linearly separable data, the SVM formulation aims to find the best hyperplane that separates the data into distinct classes. The objective is to maximize the margin between the classes while minimizing classification errors.

The formulation of a linear SVM can be represented as follows:

Minimize: 1/2 * ||w||^2

Subject to: y_i * (w * x_i + b) >= 1 for all data points (x_i, y_i)

Where:
- w is the weight vector that defines the hyperplane.
- x_i is a data point.
- y_i is the class label of x_i (-1 or 1).
- b is the bias term.

## Section 3: SVM Optimization using SGD (Stochastic Gradient Descent)

Stochastic Gradient Descent (SGD) is an optimization algorithm commonly used to train SVM models. It aims to find the optimal parameters (w and b) that minimize the SVM objective function.

The steps for SVM optimization using SGD are as follows:

1. Initialize w and b with random values.
2. Select a random data point from the training set.
3. Calculate the gradient of the objective function with respect to w and b for the selected data point.
4. Update w and b using the gradient and a learning rate.
5. Repeat steps 2-4 until convergence or a fixed number of iterations.

SGD is computationally efficient and works well for large datasets.

## Section 4: Model Evaluation by T-fold Cross-Validation

To evaluate the performance of the SVM model, we use T-fold cross-validation. Cross-validation helps assess the model's generalization capabilities by dividing the dataset into T subsets (folds). The model is trained and tested T times, with each fold acting as the test set once while the remaining folds are used for training.

The steps for T-fold cross-validation are as follows:

1. Split the dataset into T subsets (folds).
2. For each fold, use it as the test set and the remaining folds for training.
3. Train the SVM model on the training set and evaluate it on the test set.
4. Repeat steps 2-3 for all T folds and record the evaluation metrics (e.g., accuracy, precision, recall).
5. Calculate the average performance metrics to assess the overall model performance.

T-fold cross-validation helps provide a more robust evaluation of the SVM model and reduces the risk of overfitting.

