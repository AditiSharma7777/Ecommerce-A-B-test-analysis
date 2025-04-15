# Ecommerce-A-B-test-analysis
This project focuses on analyzing A/B test results for an e-commerce website to determine whether a new webpage design improves conversion rates compared to the old one.

##  Objective

To assess whether the new landing page design leads to a higher conversion rate than the existing page using statistical testing methods.

## Dataset

The dataset `ab_data.csv` contains the following columns:
- `user_id`
- `timestamp`
- `group` (control or treatment)
- `landing_page` (old_page or new_page)
- `converted` (1 if the user converted, 0 otherwise)

## Key Steps

1. **Data Cleaning:**  
   - Removed duplicate and inconsistent rows.
   - Ensured proper alignment between `group` and `landing_page`.

2. **Exploratory Data Analysis (EDA):**  
   - Analyzed overall conversion rates.
   - Visualized differences between control and treatment groups.

3. **Hypothesis Testing:**  
   - Null Hypothesis (H₀): Conversion rate of new page ≤ old page  
   - Alternate Hypothesis (H₁): Conversion rate of new page > old page  
   - Used z-test to test statistical significance.

4. **Confidence Interval Calculation:**  
   - Estimated the range within which the true difference lies.

5. **Logistic Regression:**  
   - Built a logistic model to predict conversion based on page and user characteristics.

6. **Power Analysis:**  
   - Checked whether the sample size was sufficient to detect a meaningful difference.

## Conclusion

The statistical tests did not show a significant improvement in the new page’s conversion rate. Hence, we **fail to reject the null hypothesis**.



