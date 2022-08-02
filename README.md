# (Data Visualization of Prosper's Loan Dataset)
## by (Obi-Okonkwo)


## Dataset

> The dataset I used was given to me by Udacity. It is a dataset of a lending comapny called Prosper that has over 100,000 loan data observations and many variables that directly or indirectly influence the outcome of each loan.

> For my data wrangling, 
I selected only useful columns which are:
ListingKey
CreditGrade
Term
LoanStatus
BorrowerRate
ProsperRating (Alpha)
EmploymentStatusDuration
CreditScoreRangeLower
CreditScoreRangeUpper
StatedMonthlyIncome
LoanOriginalAmount
MonthlyLoanPayment

>I merged a couple of columns together to create a new variable.
I did feauture engineering to get a new variable, the new variable was the mean of two of the original variables.
I changed the datatype of some variables to categorical variables.


## Summary of Findings

>Univariate Plots
Of the different loan statuses, people with current loans are the most frequent while those with cancelled loans have the least frequent counts. The distribution of the mean credit score was unimodal and was not skewed. Loans of 36 months was the most frequent and also credit grades of C was the most frequent. The distribution of monthly income, number of months employed and monthly loan payment was right skewed and the borrower rate was capped just below 40%.

>Bivariate Plots
>The company that provided the credit scores did a fairly decent job as the credit score gave an insight to whether the individual defaults or not. The observations with current loan status had the biggest value of money to be paid back. 
>Using a boxplot, I also saw the amount loaned as regards each loan status also had the Current loan status as the category that loaned the highest money.
>Delinquent, Defaulted and charged off loans had the highest borrower rate and it was because of their low credit scores.
>Percentage of defaulted loans increased with increasing loan risk.

>Multivariate plots
>With a facet grid plot, It means that as the credit grade tends to be riskier, credit score would be smaller and the probability for defaults are increased'.
>A scatter plot of borrower rate vs amount loaned at the left bottom of the plot, only green dots are there meaning that loans with low borrower rate and low loaned amount are generally completed.
>Used heatmap to get the correlation of all the numerical variables. Monthly loaned payment and amount borrowed have the strongest correlation.


## Key Insights for Presentation

>The last multivariate plot which is the scatter plot shows that defaulted loans rarely ever have a small interest rate and small loaned amount. The plot also shows that loans of 35% and greater than 30K dollars are raely defaulted because they are given to people with good credit scores.
>Therefore, having a good credit score would almost guarantee the individual a better borrower rate, then the loan would be a low risk loan and the individual would be eligible to a bigger loan if he/she desires.