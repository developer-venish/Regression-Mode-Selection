# Regression-Mode-Selection
ML Python Project

![](https://github.com/developer-venish/Regression-Mode-Selection/blob/main/predict.png)

---------------------------------------------------------------------------------------

Note :- All the code in this project has been tested and run successfully in Google Colab. I encourage you to try running it in Colab for the best experience and to ensure smooth execution. Happy coding!

---------------------------------------------------------------------------------------

This code performs multiple regression tasks using different regression models and evaluates their accuracy using the R-squared metric.

Let's break down the code step-by-step:

1. Data Loading:
   - The code first imports necessary libraries, including pandas, numpy, matplotlib, and Google Colab's files module.
   - It then reads a CSV file named 'Data.csv' using the `pd.read_csv` function and stores the data in the 'dataset' DataFrame.

2. Data Preprocessing:
   - The features (X) and the target variable (y) are extracted from the dataset.
   - The target variable (y) is reshaped using `y.reshape(len(y), 1)` to convert it from a 1D array to a 2D array.

3. Data Splitting:
   - The data is split into training and testing sets using the `train_test_split` function from scikit-learn. Two sets of data are created: one for linear regression (`X_train`, `X_test`, `y_train`, `y_test`) and one for the support vector regression (`X_trainsvm`, `X_testsvm`, `y_trainsvm`, `y_testsvm`).

4. Model Initialization:
   - The code initializes five regression models: `modelLR` (Linear Regression), `modelPLR` (Polynomial Regression), `modelRFR` (Random Forest Regression), `modelDTR` (Decision Tree Regression), and `modelSVR` (Support Vector Regression).

5. Feature Scaling:
   - The code uses `StandardScaler` to scale the training data (`X_train`) for the Random Forest Regression model (`modelRFR`) to make it suitable for the algorithm.

6. Model Training:
   - Each regression model is trained using the corresponding training data.

7. Making Predictions:
   - The code makes predictions using each model for the test data.

8. Model Evaluation:
   - The R-squared scores are calculated for each model using the `r2_score` function from scikit-learn.
   - The R-squared score measures how well the model fits the data, with values closer to 1 indicating a better fit.

9. Printing the Results:
   - The code prints the R-squared scores for each regression model, which represent the accuracy of the model's predictions.

Overall, the code demonstrates how to perform multiple regression tasks using different regression models and evaluates their performance using the R-squared metric. It also includes data preprocessing steps like feature scaling and data splitting to ensure the models are trained and tested properly.

---------------------------------------------------------------------------------------
