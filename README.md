# (Prosper Loan Dataset Exploration)
## by (Joshua Enam Semanyoh)


## Prosper Loan Dataset


>This data set contains 113,937 loans with 81 variables on each loan; including loan amount, borrower rate (or interest rate), current loan status, borrower income, employment status, listing category, loan term, prosper rating (alpha) and many other variables.

>Data was downloaded from https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv and you can find the data dictionary to understand the variables here https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554486256024000.

>Data wrangling was done to further assess the dataframe and clean the data. 
>> In these steps, uninsightful columns were dropped, rows with null values were dropped, duplicates were checked summarized descriptive statistics assessed, index was reset, datatypes were corrected and categorical data such as Prosper rating (alpha) was converted to categorical datatype.


## Summary of Findings
 
> 1. One main finding from the exploratory visualization is that borrower APR is affected by the loan amount; it is seen that as loan amount increases the borrower APR range becomes smaller.

> 2. Prosper Rating has a strong effect on Borrower APR; with improving Prosper rating there is lower Borrower APR. Even as the loan amount increases, this general trend is still evident. However, when borrower with the best two Prosper ratings are taking very high loans, their APR is slightly increased. This may be to deter highly rated borrowers from taking higher loans since other plots also showed that borrowers with the best ratings generally take higher loans. It may also be that Prosper (lending company) wants to make profit since a slight increase in APR on a high loan is still very substantial.

> 3. Another finding is that for very highly rated borrowers, their APR increases when they choose a longer loan term. However, for borrowers with ratings from HR to C, their APR reduces if they choose a longer term.

> 4. Another finding is that borrowers taking a short term loan (12-month) must have a baseline monthly income of 5000 dollars if they are rated D to HR whereas this doesn't apply to longer terms.

> 5. Short term (12-month) loans are capped below 6000 dollars regardless of Prosper rating of the borrower.


## Key Insights for Presentation

> My presentation focuses on features/variables that affect the borrower APR, which are original loan amount, Prosper rating and term.

The key insights in this presentation are:

> 1. A distribution of borrower APR.

> 2. A distribution of original loan amount.

> 3. A plot showing the relationship between borrower APR and loan amount. 

> 4. A plot showing the relationship between APR and Prosper rating.

> 5. Faceted plots showing the effect of term on the relationship between APR and loan amount.

> 6. Faceted plots showing the effect of prosper rating on relationship between borrower APR and loan amount.

> 7. A plot exploring the relationship between borrower APR, prosper rating and term.


## References

1. https://classrom.udacity.com

2. https://www.prosper.com/invest/how-to-invest/prosper-ratings/?mod=article_inline#:~:text=The%20Prosper%20Rating%20is%20our,average%20annualized%20loss%20rate%20range.

3. https://seaborn.pydata.org/generated/seaborn.color_palette.html

4. https://machinelearningmastery.com/data-visualization-in-python-with-matplotlib-seaborn-and-bokeh/
