# IS6813-Portfolio
Tommaso Pascucci
IS 6813 Portfolio

# Swire Coca Cola Capstone 
## Business problem summary
The Home Credit Default Risk project aims to predict the likelihood of a client defaulting on a loan. Financial institutions face significant challenges in assessing the creditworthiness of applicants, especially when traditional tools like credit scores are unavailable. Incomplete or inaccurate information about an applicant's financial background can lead to poor decision-making, resulting in loan defaults. Defaulting loans not only cause financial loss to the company but also increase operational costs and can harm the institution's reputation. The objective of this project is to develop a predictive model to determine whether a client will default on a loan, empowering lenders to make better-informed decisions

## Project objective
The primary goal of this project is to build a robust machine-learning model that can accurately classify clients as potential defaulters or non-defaulters. By leveraging data from the Kaggle competition, the project aims to:

* Reduce the financial risk for Home Credit.
* Streamline the loan approval process by identifying low-risk customers.
* Enable better financial inclusion by extending credit to applicants who are responsible but lack traditional credit profiles.

## [Solution to a business problem](https://github.com/CSJoyce/HomeCreditProject/blob/main/practiceProjectModeling2.Rmd)
The solution involves a multi-step process:

Exploratory Data Analysis (EDA): Understand the data, identify patterns, and determine variable importance.
Data Cleaning: Handle missing values, remove outliers, and preprocess data for model training.
Feature Engineering: Create new features to enhance predictive power.
Model Development: Test various machine learning algorithms, including Logistic Regression and XGBoost, to find the most effective model.
Evaluation: Assess models using metrics such as accuracy, precision, recall, F1-score, and AUC to select the best-performing solution.  <br />

With the overall recommendation being to use the the forest model for overall predictions though it is strongly recommended to compare these results with the other models as they showed strengths in different areas depending on whether false positives or false negatives are more or less acceptable.

## My contribution
I helped with some of the data cleaning and as a group decided how we wanted to handle missing values so that we all worked on the same cleaned data set when creating the models. I focused on creating the logistic regression and XGBoost models. The XGboost was the one that achieved our best Kaggle score of 0.69889.


### Logistic Regression
* 91.93% Accuracy
* 2.09% F1
* 50% Recall
* 1.07% Precision
* 
### XGBoost model
* 91.98% Accuracy
* 95.81% / 4.34% F1
* 99.86% / 2.26% Recall
* 92.08% / 58.03% Precision  <br />
![](/images/matrix.png)
![](/images/AUC.png)

### [EDA](https://github.com/TommasoPascucci/Portfolio/blob/main/EDA.Rmd)
Exploration included understanding feature importance and data distribution, as well as visualizing critical variables. For example, we observed age-related trends in loan default probabilities:
![](/images/Age.png)

### [Modeling](https://github.com/TommasoPascucci/Portfolio/blob/main/practiceProjectModeling2.Rmd)
The modeling process involved testing multiple algorithms, with XGBoost emerging as the most effective solution. Key steps included hyperparameter tuning, managing class imbalance, and optimizing thresholds.

## Business value of the solution
The predictive model developed through this project offers significant business value:

* Enhanced Risk Management: Improved loan approval decisions, reducing the likelihood of defaults.
* Increased Profitability: By identifying responsible borrowers, Home Credit can extend more loans with reduced risk.
* Operational Efficiency: Automated predictions streamline the approval process, reducing time and costs.
* Financial Inclusion: Offers opportunities for credit to individuals who may lack traditional credit histories.

## Difficulties
The project encountered several challenges, including:

* Data Cleaning: Handling a large dataset with missing values and outliers required careful preprocessing.
* Class Imbalance: The dataset was highly imbalanced, with far fewer default cases compared to non-defaults.
* Feature Importance: Identifying which features had the most predictive value was crucial for model performance.

## Learnings
This project reinforced the importance of:

* Spending significant time upfront on data cleaning and preprocessing, which simplifies downstream modeling efforts.
* Exploring and engineering features to maximize model performance.
* Allocating sufficient time for hyperparameter tuning to achieve the best results.
