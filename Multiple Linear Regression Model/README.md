# Automatidata- Multiple linear regression model

## Project Description

In this project, we aim to build a multiple linear regression model to estimate the linear relationship between the fare amount of New York City taxi trips and various independent variables. Multiple linear regression allows us to consider multiple factors when predicting the fare amount, making it a valuable tool for data professionals in various domains.

The primary objectives of this project are:

1. Perform exploratory data analysis (EDA) to understand the dataset and check model assumptions.
2. Build a multiple linear regression model to predict the fare amount.
3. Evaluate the model's performance and interpret the results.
4. Demonstrate knowledge of EDA and multiple linear regression.

## Project Structure

The project is divided into three main parts, following the PACE framework (Plan, Analyze, Construct, Execute):

### Part 1: EDA & Checking Model Assumptions (Plan)

- Discuss the purposes of EDA before constructing a multiple linear regression model.
- Identify and address outliers and extreme data values.
- Handle missing data.
- Check for multicollinearity between predictor variables.

### Part 2: Model Building and Evaluation (Analyze)

- Discuss the resources used during this stage.
- Perform EDA to analyze and discover data, looking for correlations, missing data, outliers, and duplicates.
- Convert date columns to datetime format.
- Handle outliers and extreme values.
- Examine and impute zero values in trip_distance and address fare_amount outliers.
- Engineer new features (e.g., mean_distance) based on the dataset.

### Part 3: Interpreting Model Results (Construct, Execute)

- Build a multiple linear regression model using the selected features.
- Standardize the data and fit the model to the training dataset.
- Evaluate the model's performance on both the training and test data.
- Present key takeaways from the project.
- Discuss the results and findings.


## Results 
### Data Leakage and Imputing Fare Amounts

In the course of our data preprocessing and modeling workflow, there were instances where data leakage and imputing fare amounts occurred. It's important to understand these issues and the rationale behind the steps we took in our process.

### Data Leakage

Data leakage is a critical concern in machine learning projects. It happens when information from the training dataset contaminates the test dataset, potentially leading to overly optimistic model performance. In our case, data leakage occurred when computing the `mean_distance` and `mean_duration` columns. These means were calculated from the entire dataset, including both the training and test sets. Consequently, the same columns were then used to train a model and predict on the test set.

Surprisingly, in this particular scenario, the data leakage improved the R2 score by approximately 0.03. While this may seem beneficial in our case, it's important to recognize that this is not a recommended practice. 

### Imputing Fare Amounts

Another notable step in our workflow was the imputation of fare amounts for `RatecodeID` 2. This imputation occurred after training the model on the available data. A more best-practice approach would involve separating the rides with `RatecodeID` other than 2 and training a model specifically for that subset. Afterward, we could incorporate the `RatecodeID` 2 data and its imputed fares. This would prevent training the model on data for which a separate model isn't necessary and potentially lead to an even better final model.

While we combined these steps for simplicity and ease of explanation, it's important to emphasize that when deploying models in real-world applications, data cleaning, imputations, data splits, and predictions should be performed within modeling pipelines. This results in a streamlined and automated process, with no need for manual intervention at each step.



## Dependencies

The project uses the following Python libraries and packages:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn (for linear regression)

##

