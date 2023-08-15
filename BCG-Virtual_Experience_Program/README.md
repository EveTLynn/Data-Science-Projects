## This is a Project for BCG Data Science Virtual Experience Program on Forage.

[link to the program here!](https://www.theforage.com/virtual-internships/Tcz8gTtprzAS4xSoK?ref=dDsCRiLXErJmXtsZq)

[link to the certificate](https://forage-uploads-prod.s3.amazonaws.com/completion-certificates/BCG%20/Tcz8gTtprzAS4xSoK_BCG_dDsCRiLXErJmXtsZq_1691288193757_completion_certificate.pdf)

The program consists of 4 main tasks:
1. Business Understanding & Hypothesis Framing
2. Exploratory Data Analysis
3. Feature Engineering & Modelling
4. Findings & Recommendations

Tools/libraries used:
1. Programming Language: Python
2. Libraries: pandas, matplotlib, seaborn, scikit-learn
3. Algorithms: classification: Random Forest
4. Skills: EDA, Data Visualization, Machine Learning

*Disclaimer: I take ideas and code from the BCG sample solution (and from Google, of course :3) and put my own take on them.
This is still in process of refining and improving. It's messy but hey I'm learning and working on it.*

# Context of the project
The context involved a major gas and electricity utility that supplies to corporate, SME (Small & Medium Enterprise), and residential customers called PowerCo.
The power-liberalization of the energy market in Europe has led to significant customer churn, especially in the SME segment. 
They have partnered with BCG to help diagnose the source of churning SME customers. 
A fair hypothesis is that price changes affect customer churn. Therefore, it is helpful to know which customers are more (or less) likely to churn at their current price, 
for which a good predictive model could be useful. 
Moreover, for those customers that are at risk of churning, a discount might incentivize them to stay with our client. 
The head of the SME division is considering a 20% discount that is considered large enough to dissuade almost anyone from churning (especially those for whom price is the primary concern).

The client provide 2 data files:
- client_data.csv
- price_data.csv

The details of the data will be discussed in the EDA task.

# The tasks
## 1. Business Understanding & Hypothesis Framing

**The goal:** formulate the hypothesis as a data science problem and lay out the major steps needed to test this hypothesis.

**The hypothesis:** customer churn is driven by price sensitivity. 

In order to test the hypothesis, we will need to model churn probabilities of customers, and derive the effect of prices on churn rates. This will include the following steps:
- Define what is price sensitivity? In this case to my understand it is the churn due to the change in price, which means there will be some correlations between price related variables to customer churn
- Feature engineering and choose a classification model. I used Random Forest as the task requested
- Evaluate the model and dive deeper
- Size the business impact of the client’s proposed discounting strategy

## 2. Exploratoty Data Analysis

The dataset includes features of SME customers in January 2016 as well as the information about whether or not they have churned by March 2016. In addition to that we have received the prices from 2015 for these customers. 

Given that this is the first time the client is resorting to predictive modelling, it is beneficial to leverage descriptive statistics and visualization for extracting interesting insights from the provided data before diving into the model.

The client would like to have a view on whether the 20% discount offer to customers predicted is a good measure. Given that it is a steep discount – bringing their price lower than all competitors – we can assume for now that everyone who is offered the discount will accept it. According to regulations, PowerCo cannot raise the price of someone within a year if they accept the discount. Therefore, offering it excessively is going to hit revenues hard.

## 3. Feature Engineering and Modeling

### Feature Engineering

The steps include:
- Calculate the Difference between off-peak prices in December and preceding January and its variance:
  - Average price changes across perods
  - Max price changes across periods and months
- Transform datetime data into months
- Transform categorical data
- Transform numerical data
- Remove highly correlated features

### Modeling

This project use Random Forest algorithm to predict the churn customers. The steps include:
- Modeling
- Model Evaluation
- Calculate feature importances

### Discount Impact

This task includes:
- Calculate the baseline revenue
- Calculate the benefits and costs if applied discounts

*All the code for task 2 & 3 is in the \*.ipynb file*

## 4. Findings & Recommendations

Please read the *.pptx presentation file.

