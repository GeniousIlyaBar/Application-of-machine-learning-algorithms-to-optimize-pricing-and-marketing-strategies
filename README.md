# Notebooks
1. Pre-processing and data analysis
2. Encoding
3. Machine Learning

# Stages
## Pre-processing and data analysis
In this notebook, I have executed the essential pre-processing and EDA required on the dataset before modeling. This includes loading data, performing simple statistics using df.describe() that gives an insight into the nature of features and their distribution; removing obviously non-relevant features that would have no contribution toward model training and eliminating features where a high percent of values in the column have missing values because it will seriously affect the data quality. Next, further refinement in this dataset was done by the identification and removal of outliers to avoid skewed performance by the model. The data type was changed where necessary, and all numerical and categorical features were maintained alike. I further segregated numerical and categorical variables for better feature engineering. Finally, a correlation matrix is constructed to see relationships between the numerical features for multicollinearity. These preprocessing steps are literally the very foundation of efficient model training.

**Notebook:** [Pre-processing and data analysis.ipynb](https://github.com/GeniousIlyaBar/Application-of-machine-learning-algorithms-to-optimize-pricing-and-marketing-strategies/blob/main/Pre-processing%20and%20data%20analysis.ipynb)

**Result:** preprocessed_df.csv

## Encoding
The encoding of categorical features and the transformation of numerical data were done in this notebook to enhance the model's performance. First, I have used Label Encoding for ordinal categorical features and One-Hot Encoding for those features where there is no natural order. In that way, categorical variables were represented properly to machine learning models. Next, I standardized the numerical features using StandardScaler, scaling the variables to a common scale that usually helps in improving model convergence. In features of a datetime nature, I extracted the year, month, day, hour, minute, second, and week number to help the model get more patterns concerning time. These transformations optimized the dataset for training and enhanced feature interpretability.

**Notebook:** Encoding.ipynb

**Result:** encoded_scaled_df.csv
