# Cafe-Customer-Analytics

I used this project to practice working with customer transaction data in Python.

The main thing I wanted to understand was why revenue was falling over the year. At first, I thought customers might simply be spending less per order. After comparing revenue, order volume, active customers, and average order value, I found that customer activity seemed to be the bigger issue.

From there, I looked at customer behavior in more detail. I used K-Means clustering to separate customers with different activity patterns and then built a churn model to estimate which customers were less likely to return.

## Main results

- Revenue decreased by 20.6% from January to December.
- Order volume decreased by 19.4%.
- Active customers decreased by 12.6%.
- Average order value changed by only -1.4%.
- The top 20% of customers generated 34.8% of total revenue.
- Recency was the strongest feature in the churn model.
- Logistic Regression reached a test ROC-AUC of 0.959.
- I created a priority list of 600 customers for possible retention action.

## What I used

I worked mainly with Python, pandas, matplotlib, and scikit-learn.

The analysis included:
- data cleaning
- customer behavior analysis
- Pareto analysis
- K-Means clustering
- PCA
- Logistic Regression
- Random Forest
- Decision Tree
- cross-validation
- permutation importance
- retention prioritization
- coupon analysis

## What I learned

One part I found useful was seeing that the most complex model was not automatically the best choice. Logistic Regression performed well and was also easier to explain.

I also learned that a prediction model is more useful when the result can be connected to an action. Instead of stopping at churn probability, I used customer value and churn risk together to create a retention priority list.

## Files

- `Cafe_Customer_Analytics.ipynb` — analysis and code
- `Cafe_Customer_Analytics_Portfolio.pdf` — project summary

## Limitations

This project uses a course-provided educational dataset.

The coupon analysis should be treated as descriptive because I did not independently confirm random assignment. In a real project, I would also want profit margin data and an A/B test before making a final business decision.
