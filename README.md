# Kernel SVM with k-Fold Cross Validation

This project demonstrates the use of a **Kernel Support Vector Machine (SVM)** with **k-Fold Cross Validation** to classify social network ads based on user features such as age and estimated salary. The dataset `Social_Network_Ads.csv` is used for training and testing the model.

### Dataset
The dataset contains the following features:
- **Age**: Age of the user.
- **Estimated Salary**: Estimated salary of the user.
- **Purchased**: Binary target variable indicating if the user purchased the product (1) or not (0).

- ![image](https://github.com/user-attachments/assets/1732b371-2558-41a1-902e-ebc855677bc2)


The dataset is split into a training set (75%) and a test set (25%) to evaluate the performance of the model.

## Implementation Steps

### 1. Data Preprocessing
- **Splitting the dataset**: The data is split into training and test sets using the `train_test_split` function from `sklearn`.
- **Feature Scaling**: Features are scaled using `StandardScaler` to standardize the age and salary data for better performance of the SVM model.

### 2. Training the Kernel SVM Model
- A **Support Vector Machine** classifier with a **Radial Basis Function (RBF) kernel** is trained on the training set.

### 3. Model Evaluation
- The model is evaluated using a **confusion matrix** and **accuracy score**.
- **k-Fold Cross Validation** is applied to assess the model’s performance across 10 different folds.

### 4. Visualization of Results
- The decision boundaries for both the **Training Set** and **Test Set** are visualized using `matplotlib`.

## Results

- The confusion matrix shows the performance of the model on the test set.
- Accuracy from **k-Fold Cross Validation** is calculated, along with the standard deviation to measure the model’s reliability.c
