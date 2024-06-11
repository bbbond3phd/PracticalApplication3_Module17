# Overview
In this third practical application assignment, your goal is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) you encountered in this section of the program.

## Business Understanding: CRISP-DM Step 1
The data is from a Portuguese banking institution and is a collection of the results of multiple marketing campaigns. The objective is to compare model performance against coupon acceptance for predicting if the client will subscribe (yes/no) a term deposit (variable y).

## Data Understanding: CRISP-DM Step 2
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.
The four datasets are as follows: 
1) bank-additional-full.csv with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010)
2) bank-additional.csv with 10% of the examples (4119), randomly selected from 1), and 20 inputs
3) bank-full.csv with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs)
4) bank.csv with 10% of the examples and 17 inputs, randomly selected from 3 (older version of this dataset with less inputs)
For the purposes of this analysis the third dataset was used for model building and comparing.

## Data Preparation: CRISP-DM Step 3
### Data preparation after our initial exploration

<img width="969" alt="Bank_Pairplot" src="https://github.com/bbbond3phd/PracticalApplication3_Module17/assets/161508171/dbe4ed2c-041f-4bb2-8f22-cac544ae10b6">

Visual investigation found and outlier in the 'previous' feature.
In this instance once occurrence was found with the maximum value for 'previous' is: 275
The decision was to leave the record.

## Modeling: CRISP-DM Step 4
In total four models were run against the data in attempts to predict the target variable ('conversion', after renaming the feature)
1. k Nearest Neighbor
2. Decision Tree
3. Logistic regression
4. Support vector machine

## Evaluation: CRISP-DM Step 5
Findings:
1. kNN: Moderate performance with an accuracy of: 0.8923621350634031
2. Decision Tree: Strong performance with an accuracy of: 0.8731200235918608
3. Logistic Regression: Consistent performance with an accuracy of: 0.891108817457977
4. SVM: High performance with an accuracy of: 0.8975228546151578 

<img width="863" alt="Accuracies" src="https://github.com/bbbond3phd/PracticalApplication3_Module17/assets/161508171/43eadd99-920a-4165-b854-cd01f6ac4046">

### Conclusion
The analysis shows that Decision Trees and SVM classifiers provide the best performance for predicting conversion. With proper tuning and potential feature engineering, these models can be further improved to achieve better predictive accuracy. The visualizations and metrics provided clear insights into the data and model performances, making them actionable for business decisions.
