# Recipe-Traffic-Classifier

#### This project was a component of my examination process for obtaining DataCamp's Professional Data Scientist Certificate.

## Introduction
This project focuses on analyzing and predicting the traffic (high or low) of recipes in a superstore. The goal is to develop a predictive model that accurately classifies recipes based on their potential traffic, which can assist in optimizing inventory, marketing strategies, and resource allocation.

## Data Validation
### Validation and Cleaning Steps
- Numerical Columns: Checked for missing values and filled them with the median of the respective category and servings.
- Categorical Columns: Transformed category and high_traffic columns into categorical data types.
- Servings Column: Converted to integer type.
- Null Values: Dealt with null values by filling with the median of the same category.
- Duplicate Rows: Ensured no duplicate rows were present.
### Exploratory Analysis
#### Single Variable Graphics
- Category Distribution: Displayed the frequency of each recipe category using a count plot.
- High Traffic Frequency: Presented the proportion of high and low traffic recipes using a pie chart.
- Traffic in Each Category: Visualized the frequency of high and low traffic recipes within each category using a stacked bar chart.
#### Relationship Between Features
- Distribution of Numerical Data: Plotted histograms to illustrate the distribution of calories, carbohydrate, sugar, and protein.
- Box Plots: Displayed box plots to highlight the distribution and identify outliers in numerical columns.
- Effect of Numerical Features on Calories: Utilized scatter plots to observe the relationship between numerical features and calories.
- Mean of Numerical Features in Each Category: Presented bar plots showcasing the mean of numerical features in each recipe category.
## Model Development
### Preprocessing
- Encoded the category column using one-hot encoding.
- Removed irrelevant columns such as servings and recipe.
- Standardized numerical features using Standard Scaler.
### Model Selection
- Selected models: Logistic Regression, Linear Discriminant Analysis, and Ridge Classifier.
- Reasoning: These models are suitable for binary classification tasks and provide interpretable results.
### Model Evaluation
- Evaluated models' accuracy, precision, recall, and F1-score.
- Conducted a grid search to optimize hyperparameters.
- Assessed models' performance using confusion matrices and classification reports.
## Business Metrics
- Achieved a general accuracy of 76% in predicting recipe traffic.
- Precision of 83% indicates a low false positive rate, reducing the risk of misclassifying low traffic as high traffic.
## Recommendations
- Decrease the number of chicken recipes and increase meat recipes.
- Increase the variety of vegetable and potato recipes.
- Consider reducing the number of beverage recipes.
## Conclusion
This project provides valuable insights into recipe traffic patterns and offers recommendations to optimize recipe assortment and improve overall store performance. By implementing the suggested changes, the superstore can enhance customer satisfaction and profitability.
