# Lending Club Case study
>In this assignment, we are trying to analyse the impact of various factors on loan repayment defaulting.
>We shall perform Exploratory data analysis and draw observations and provide suggestions to minimize risk and loss



## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Suggestions](#suggestions)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- We use EDA techniques like Univariate analysis, Bivariate analysis, Bayesian analysis and time series analysis
- In this case study, we will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.
- Our dataset contains the complete loan data for all loans issued through the time period 2007 t0 2011.


## Conclusions
### From univariate analysis
- Most of the lendings were successful
- Major purpose for applying for loan is debt_consolidation (almost 50%)
- Second major purpose is for credit_card
- Less than 1% of lendees have an education loan or renewable energy loan
- Most income sources have not been verified by LC
- CA has been the most active state where loans were give (about 18%)
- About half the lendees rent and alomst another half have mortgaed their homes.
- People with unmortgaged homes (7.5%) are least likely to apply for a loan
- More than 3/4th of lendees went for 36 months term
- More than 3/4th of lendees are graded C or above

### From baysian analysis of P(Fail|factor)
- OTHER type of home ownership is the riskiest albiet by a small margin
- Small businesses are the riskiest to lend to
- 60 month terms are significantly much riskier than 36 month terms
- The probabilty of defaulting seems to increase down the grades, A being the safest and G being the riskiest
- Although the loan grading technique seems to work reasonably well, the technique to sub-grade seems to be faulty, especially with the strong misbehaviors presented in the sub-gradings of E, G and especially F (F5 is disproportionately higher than any G)
- probability to default seems to increase with derogatory public records
- In general, chances of defaulting seem to increase with inquiries in last 6 months
- loan_amt shows up to have some impact on the default prbability: cases of fully paid are distribute around amounts greater than those in case of defaulting.
- The probability of defaulting seems to increase with revol_util, and int_rate
- The probability of defaulting seems to decrease with annual_inc

### Bivariate analysis
- median Small business, house related and credit/consolidation loans are higher than the rest
- median loan amount increases with decreasing grade
- median interest rate increases with decreasing grade
- Higher the grade (A is highest), lower the interest rate
- Higher the interest rate, higher the revolving utility
- annual_income is mildly postively correlated with loan/funded amounts

### Time series analysis
- Number of loans issue increased month by month, almost doubling each year
- Each year saw an increase with year average loan
- But annual incomes didn't change much over the years

## Suggestions
- Consider only cases with very few previous charge offs
- Reduce rate of interests. Interest rates might be higher for smaller grades, but the reason of defaulting could be high interest accumulation.
- Reduce loan amount sanctions for lower grade/more previous charge offs lendees to ensure minimal losses.


## Technologies Used
- numpy - 1.23.1
- pandas - 1.4.3
- seaborn - 0.12.1



## Contact
Created by [@showman-sharma] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
