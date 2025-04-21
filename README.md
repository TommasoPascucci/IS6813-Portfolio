# IS6813-Portfolio
Tommaso Pascucci
IS 6813 Portfolio

# Swire Coca Cola Capstone 
## Business problem summary
 The objective of this project is to develop a predictive/classification model to determine whether a customer will be high or low growth, specifically in identifying important attributes, empowering Swire to make better-informed decisions

## Project objective
The primary goal of this project is to build models that can assist in identifying high and low growth customers with 2 distinct groups, first is the full data set and the second being the local market partners with fountain only and no CO2. By leveraging data from the Swire team, the project aims to:

* Identify and retain high growth potential customers.
* Move low growth customers.
* Determine which variables have a high importance in predictions.

## [Solution to a business problem]([https://github.com/CSJoyce/HomeCreditProject/blob/main/practiceProjectModeling2.Rmd](https://github.com/TommasoPascucci/IS6813-Portfolio/blob/main/Capstone.ipynb))
The solution involves a multi-step process:

Exploratory Data Analysis (EDA): Understand the data, identify patterns, and determine variable importance.
Data Cleaning: Handle missing values, remove outliers, and preprocess data for model training.
Feature Engineering: Create new features to enhance predictive power.
Model Development: Test various machine learning algorithms, including Logistic Regression and XGBoost, to find the most effective model.
Evaluation: Assess models using metrics such as accuracy, precision, recall, F1-score, and AUC to select the best-performing solution.  <br />

With the overall recommendation being to use the the forest model for overall predictions though it is strongly recommended to compare these results with the other models as they showed strengths in different areas depending on whether false positives or false negatives are more or less acceptable.

## My contribution
I helped with some of the data cleaning and as a group decided how we wanted to handle missing values so that we all worked on the same cleaned data set when creating the models. I focused on creating the logistic regression and XGBoost models. The XGboost was the one that achieved our best Kaggle score of 0.69889.


### Clustering
* 66% Accuracy
* 77% F1
* 98% Recall
* 65% Precision
![](/images/AUC.png)
  
### XGBoost model (local market partners)
* 65.62% Accuracy
* 77% / 28% F1
* 95% / 18% Recall
* 65% / 68% Precision  <br />
![](Picture/XGboost.png)


### [EDA]([https://github.com/TommasoPascucci/Portfolio/blob/main/EDA.Rmd](https://github.com/TommasoPascucci/IS6813-Portfolio/blob/main/EDA.ipynb))
Exploration included understanding feature importance and data distribution, as well as visualizing critical variables. For example, we observed Specific trade channels such as Fast Casual Dining seem to be correlated more with high growth:
![](Picture/tradechannel.png)
We can also observe that there is a very large class imbalance between high and low growth as well as a big range in values between the 2 groups, which needs to be kept in mind when building models and interpreting outputs.
![](Picture/classimbance.png)

### [Modeling]([https://github.com/TommasoPascucci/Portfolio/blob/main/practiceProjectModeling2.Rmd](https://github.com/TommasoPascucci/IS6813-Portfolio/blob/main/Capstone.ipynb))
The modeling process involved testing multiple algorithms, with XGBoost emerging as the most effective solution. Key steps included hyperparameter tuning, managing class imbalance, and optimizing thresholds.

## Business value of the solution
The predictive model developed through this project offers significant business value:

* Enhanced Risk Management: Improved loan approval decisions, reducing the likelihood of defaults.
* Increased Profitability: By identifying responsible borrowers, Home Credit can extend more loans with reduced risk.
* Operational Efficiency: Automated predictions streamline the approval process, reducing time and costs.
* Financial Inclusion: Offers opportunities for credit to individuals who may lack traditional credit histories.

## Difficulties
The project encountered several challenges, including:

* Data Cleaning: Handling a large dataset with some missing values and outliers required careful preprocessing.
* Class Imbalance: The dataset was highly imbalanced, with far fewer default cases compared to non-defaults.
* Feature Importance: Identifying which features had the most predictive value was crucial for model performance.

## Learnings
This project reinforced the importance of:

* Spending significant time upfront on data cleaning and preprocessing, which simplifies downstream modeling efforts.
* Exploring and engineering features to maximize model performance.
* Allocating sufficient time for hyperparameter tuning to achieve the best results.
