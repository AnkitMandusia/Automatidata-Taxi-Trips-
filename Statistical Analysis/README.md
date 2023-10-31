# Statistical Analysis(A/B Test Analysis)
## Project Overview
This project aims to analyze whether there is a significant relationship between payment type (credit card or cash) and the fare amount paid by customers using taxi cab services. The goal is to provide insights that can help taxi cab drivers generate more revenue.

## Business Understanding
The key business insight that emerged from this A/B test is that encouraging customers to pay with credit cards can result in higher revenue for taxi cab drivers. By comparing the average fare amounts between customers who use credit cards and customers who use cash, we found that customers who pay with credit cards tend to pay a larger fare amount.

## Data Understanding
We used a dataset containing taxi trip data, including information on payment type (encoded as integers: 1 for credit card and 2 for cash) and fare amounts. The data was collected in 2017.

## Modeling and Evaluation
We conducted a two-sample t-test with a significance level of 5% to test the hypothesis:

- Null Hypothesis (H0): There is no difference in the average fare amount between customers who use credit cards and customers who use cash.
- Alternative Hypothesis (HA): There is a difference in the average fare amount between customers who use credit cards and customers who use cash.

The t-test resulted in a p-value of approximately 6.80e-12, which is significantly smaller than the chosen significance level. Therefore, we reject the null hypothesis, indicating a statistically significant difference in the average fare amount between the two payment types.

## Business Recommendations
Based on the results of this A/B test, we recommend the following for taxi cab drivers:

1. Encourage customers to use credit cards for payments to potentially increase revenue.
2. Consider offering incentives or promotions for customers who choose credit card payments to further encourage its use.

## Assumptions and Limitations
It's important to note that this A/B test is based on several assumptions:

1. We assume that the dataset represents a controlled experiment where customers are randomly assigned to either credit card or cash payments. In reality, passengers may choose their payment method based on various factors, and causation may not be established.

2. The dataset does not account for other likely explanations for payment type, such as riders' preferences or the nature of the trip. The correlation between fare amount and payment type might be driven by other factors.

## Conclusion
The A/B test suggests a link between payment type and fare amount, real-world conditions and customer behavior may lead to more complex relationships.

This analysis provides a starting point for further investigations and strategies to optimize revenue for taxi cab drivers.
