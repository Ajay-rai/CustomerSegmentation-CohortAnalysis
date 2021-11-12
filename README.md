# Customer Segmentation/Cohort Analysis of customer data for Saas company
Businesses can gain valuable insights about their customers' behavior by converting their customer data into cohort analysis charts. The metrics used to do cohort analysis are: customer retention rate, net revenue retention, and customer lifetime revenue. The Jupyetr notebook includes data manipulation, cohort charts, a cohort layer cake chart, and insights.


## Code and Resources Used
* **Python Version:** 3.8.5
* **Packages:** pandas, numpy, matplotlib, seaborn


## Methodology
Following metrics are useful for a start-up ecosystem with subscription model to track their progress:
  * __Customer Retention Rate__: tracks the number/percent of cohort made purchases for the subsequent months
  * __Net Revenue Retention__: tells the % of total revenue for subsequent month with respect to the month of joining
  * __Customer Lifetime Revenue__: tells the amount of cumulative revenue we make per customer for subsequent months
  * __Customer Lifetime Value__: tells how much profit we make from each customer


Assumptions:
  * Assumed that the country of a customer is the country recorded in one of the transaction in “card_country” column. 
  * Consider that the first day of transaction for a customer in 2020 is the date of sign-up


## Data Cleaning 
Cleaned the raw data and made new columns with proper assignment of variables.
* Made a net revenue column using paid and refund
* Imputed missing countries using a dictionary made with customerid with their respective countries.
* Checked for ouliers

## EDA 
Plotted cohort analysis charts, some examples are shown below:

![alt text](https://github.com/Ajay-rai/CustomerSegmentation-CohortAnalysis/blob/main/images/US_Customer_Retention_Rate.svg)
![alt text](https://github.com/Ajay-rai/CustomerSegmentation-CohortAnalysis/blob/main/images/US_Net_Revenue_Retention.svg)
![alt text](https://github.com/Ajay-rai/CustomerSegmentation-CohortAnalysis/blob/main/images/US_Customer_Lifetime_Revenue.svg)
![alt text](https://github.com/Ajay-rai/CustomerSegmentation-CohortAnalysis/blob/main/images/cohort_layer_cake.svg)


## Results and Conclusion
* During the month of December, cohort retention rates were low in all three countries. To regain customers, one can analyze their behavior and offer them a deal.
* In a few cases, we noticed an unexpected increase in net revenue retention. It'd be interesting to learn about the behaviors of those cohorts and see what's going on.
* On average, the company made the revenue of 4000 dollars per customer per year.
* By the end of the year, the company's revenue had increased from 50k dollars to 200K dollars. We can also see how covid-19 might affect revenue from the cohort layer cake.
* Customer Lifetime Value can be analyzed if gross margin profit is given.
