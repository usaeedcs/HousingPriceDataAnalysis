# Housing Price Data Analysis and Feature Engineering using Python

The main purpose of this project is to understand the relationships within the data and to build a predictive model for the `SalePrice` variable, which represents the sale price of a house. The project uses a dataset named `DF_AH.csv`.

## Project Purpose and Findings

The primary goal of this project is to conduct exploratory data analysis on the provided dataset, clean and preprocess the data, and finally, build predictive models. The target variable for our models is `SalePrice`, a numerical value representing the sale price of a house.

During the exploratory data analysis, we found that some variables have missing values that needed to be handled. We used a greedy approach for imputation, where we found all columns having numeric data type and imputed them by mean, and similarly, we found all categorical data and imputed it by the most common one.

We also found that some variables are highly skewed and some variables have a strong correlation with each other. We used feature scaling to standardize the range of independent variables or features of data.

The predictive modeling part of the project includes Multiple Linear Regression, Ridge Regression, Lasso Regression, and Backward Elimination. After comparing these models, we found that the Lasso Regression model performed slightly better with an R-squared value of 0.85, indicating that 85% of the variance in the SalePrice can be predicted from the input features.

The results of the analysis provided valuable insights into the factors that influence the sale price of a house. For instance, the size and quality of the house, the neighborhood, and the year of construction were among the most significant factors.

## Libraries Used

The project uses several Python libraries, including:

- `numpy` and `pandas` for data manipulation
- `matplotlib` and `seaborn` for data visualization
- `sklearn` for machine learning and data preprocessing
- `statsmodels` for statistical models

## Project Structure

The project is structured as follows:

1. **Data Loading**: The dataset is loaded using pandas' `read_csv` function.
2. **Exploratory Data Analysis**: The data is explored using various statistical and visualization techniques.
3. **Data Cleaning**: The data is cleaned by handling missing values and encoding categorical variables.
4. **Feature Selection**: Important features are selected using various techniques like correlation matrix and SelectKBest.
5. **Model Building**: Several models are built and evaluated, including Multiple Linear Regression, Ridge Regression, Lasso Regression, and Backward Elimination.

## How to Run

To run this project, follow these steps:

1. Clone the repository to your local machine.
2. Make sure you have all the necessary Python libraries installed. You can install them using pip:
