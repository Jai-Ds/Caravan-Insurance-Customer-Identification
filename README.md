# Caravan-Insurance-Customer-Identification

Problem Statement: - 
Need to classify the potential customers in buying Caravan insurance. Target variable Caravan(Binary Classification).
Kaggle dataset :- https://www.kaggle.com/kathakaliseth/caravan-insurance-customer-identification/notebook

Data Analysis: -
The dataset contains 87 variables and 9823 observations. Please refer the Kaggle link for variable descriptions.
The dataset contains both train and test observations. Hence the dataset was divided into two data frames Train and Test using the ORIGIN variable. Then the variable was dropped.
Train’s shape (5822, 86)
Test’s shape (4000, 86)
•	Down sampling
Train test contains the imbalanced classification so we are going for down sampling.  The categories were down sampled from
0 -3762     1 – 238 (Value counts)

To
0 - 400   1- 348 (Value counts)

•	No Missing Values

•	Feature Selection

Applied chi-sq-Test for Categorical variables with p-value threshold limit 0.02 and neglected the insignificant variables. The dimensions was reduced from 87 to 26.

All were categorical variables with pre set type codes.

•	No outliers were carried out since all are categorical variables.

•	Model Development

Initially the model came out with 75% accuracy rates. When the p value of the chi-sq test was reduced to 0.02 the dimensions were further reduced and the model came up with 100% accuracy rates with no FP and FN.

Accuracy: 1.0
Confusion matrix: [[3762    0]
                                  [   0  238]]

