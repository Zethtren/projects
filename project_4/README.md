# Project 4
#### Resources:
The Notebook: 
(Caution running these cells. I am using a 16GB RAM with GPU optimization on the XGBoost. I experienced many Kernel crashes while putting this notbook together)
https://git.generalassemb.ly/hbova/project_4/blob/master/ExploringLoanData.ipynb

The Data:
https://www.kaggle.com/wendykan/lending-club-loan-data#loan.csv

The Presentation:
https://docs.google.com/presentation/d/1wtbOwRK--AOGInoV7aIMq7XFDlodqQc25Gk-gFhcjjM/edit?usp=sharing

## The Question:

<font size=4>Can we predict The count of deliquincies a person has based on other metrics collected when applying for a loan. 
</font>
## Hypothesis:

<font size=4>I believe that there are features which will be able to significantly predict how many payment delinquincies someone has had. </font>
<font size=4>This information will be useful in determining whether or not someone is likely to miss payments. This is information that any lender would love to have available to them when providing a loan service.</font>

## The Data:

<font size=4>The data I will be using is from the Kaggle website:</font>
https://www.kaggle.com/wendykan/lending-club-loan-data#loan.csv

<font size=4>There is many variables that seemed irrelevant to the predicting process and many variables that were directly correlated. During EDA all of the features were removed. And missing Data was handled with various methods of dropping and imputing.  </font>

## Modeling:

<font size=4>The First model was used to determine how well the data can be used to predict my outcome. So first I fit a Generalized Linear Model from the statsmodel library. I passed a family class of Poisson. This allowed me to get a good fit to the data. Since the distribution was whole integers with many values at 0 decreasing as the value rises. </font>
<font size=4>After Analyzing the Coeficients and P values from the Statsmodels Summary I continued to try and build predictive models.</font>

## Analyzing Results:
<font size=4>With the methods I followed I was unable to build a model which generated accurate predicitons. I was however, able to identify some strong trends in the data. To me this indicates that it is possible to model against this data I would just need to adjust parameters in my models. </font>

## Conclusions:

<font size=4>Apart from being able to conclude that relationship between home ownership categories and purpose of loan againt number of delinquencies is significant. I am not able to conclude at this time wether or not that information can be used to build an effective model. Given how high some of the values were I do believe that an accurate model exists. I was limited greatly by computational resources and time during this project. Given more time I suspect an SVC model would fit very well.</font>

Project Time Limit was 6 hours
