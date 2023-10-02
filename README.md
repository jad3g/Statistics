# Statistics
time constraint paper
# README

## Table of Contents
1. [Question 1](#question-1)
2. [Question 2](#question-2)
3. [Question 3](#question-3)

---

## Question 1
### (A) Margin of Error for Population Mean Life of Light Bulbs
To find the margin of error for the population mean life of compact fluorescent light bulbs at a 95% confidence level, follow these steps:

1. Calculate the sample size (n) = 81, which is greater than or equal to 30, making it suitable for this analysis.
2. Use the formula for the margin of error (e):
   ```
   e = Z_(α/2) * σ / (√n)
   ```
   where:
   - e = margin of error
   - Z = Z-value
   - α = level of significance (0.05 for 95% confidence)
   - 𝜎 = population standard deviation
   - n = sample size

3. Calculate Z_(α/2) by looking up the Z-table:
   ```
   P(-Z_(α/2) < Z < Z_(α/2)) = 1 – α
   P(-Z_(0.05/2) < Z < Z_(0.05/2)) = 0.95
   P(-Z_0.025 < Z < Z_0.025) = 0.95
   P(Z < Z_0.025) = 0.975
   ```
   Therefore, Z_0.025 ≈ 1.96.

4. Calculate the margin of error (e):
   ```
   e = 1.96 * 1000 / (√81)
   e ≈ 217.78 hours
   ```

### (B) Confidence Interval
The 95% confidence interval estimate for the population mean life of compact fluorescent light bulbs is:
```
P(x̄ - e < μ < x̄ + e) = 0.95
```
Where:
- x̄ = sample mean (7600)
- e = margin of error (217.78)
- μ = population mean

So, the confidence interval is:
```
P(7382.22 < μ < 7817.78) = 0.95
```
Therefore, the population mean life of compact fluorescent light bulbs is estimated to be between 7382.22 hours and 7817.78 hours with 95% confidence.

### (C) Normal Distribution Assumption
It can be assumed that the population compact fluorescent light bulb life is normally distributed due to a sufficiently large sample size (n ≥ 30) and the application of the Central Limit Theorem, which states that as the sample size increases, the sample mean approaches the population mean.

### (D) Revised Margin of Error and Confidence Interval
Repeat the same calculations with a different population standard deviation (σ = 800) to find the revised margin of error and confidence interval. The result is:
- Margin of error (e) ≈ 174.22 hours
- Confidence interval: P(7425.78 < μ < 7774.22) = 0.95

The manufacturer still has NO right to state that the compact fluorescent light bulbs have a mean life of 8,000 hours based on the revised analysis.

---

## Question 2
### (A) Hypotheses
Hypotheses for the average hourly wage of men and women:
- Null Hypothesis (H0): There is no difference (difference = 0) between the average hourly wage of men and women.
- Alternative Hypothesis (H1): There is a difference (difference ≠ 0) between the average hourly wage of men and women.

### (B) Test Results
- The t-value for the regression test is -4.95.
- It's a right-tailed test.
- Calculate the critical value (CV) at a 5% level of significance (α = 0.05). CV ≈ 1.64.
- Since the t-value (-4.95) is further away from the critical value (1.64), we fail to reject the null hypothesis. This means that at the 5% level of significance, we cannot conclude that the average hourly wage of men is significantly higher than that of women.

### (C) Multiple Regression Analysis
- Including the "degree" variable affects the regression model as it can predict changes in the coefficients of other variables.
- The model with both "gender" and "degree" variables is more realistic and has a slightly higher R-squared (R2) value, indicating a better fit.
- R2 measures the proportion of variation in hourly wage explained by the variables. Adding more variables can further improve the model's goodness of fit.

### (D) Regression Model Interpretation
The regression model is as follows:
```
rwage = 12.84 + 3.22 * male + 5.77 * degree + u
```
Interpretation of coefficients:
1. If male = 0 and degree = 0, the predicted wage rate is £12.84 per hour.
2. Holding other variables constant, being male increases wages by £3.22 per hour on average.
3. Holding other variables constant, having a degree increases wages by £5.77 per hour on average.
- Both "male" and "degree" variables are statistically significant in the model.
- The model suggests a gender pay gap.

### (E) Further Analysis
Consider adding more variables like years of experience, employment status, age, etc., to improve the model's R2 and better explain wage variations.

---

## Question 3
### (A) Regression Model
The regression model is as follows:
```
rlnwage = 2.24 + 0.16 * Degree + 0.058 * Experience - 0.001 * SquaredExperience - 0.024 * Worktraining + u
```

### (B) R-squared (R2)
R2 is 0.1206, indicating that 12.06% of the variation in the log of hourly wage is explained by the included variables (Degree, Experience, SquaredExperience, and Worktraining). The model needs additional variables to explain the remaining variation.

### (C) Interpretation of Coefficients
Interpretation of coefficients:
1. Holding all other variables constant, the predicted log of hourly wage is £2.24 per hour.
2. Holding other variables constant, having a degree increases hourly wages by 0.16% on average.
3. Holding other variables constant, each additional year of experience increases hourly pay by 0.058% on average.
4. Holding other variables constant, each additional unit of squared years of experience decreases hourly wages by 0.001% on average.
5. Holding other variables constant, receiving on-the-job training decreases hourly pay by 0.024% on average. However, this variable is not statistically significant.

The model's overall p-value is significant, but R2 is low, suggesting the need for additional explanatory variables.

### (D) Removing the "Worktraining" Variable
The "Worktraining" variable has a negative coefficient and is not statistically significant. Removing it may improve the model's validity and increase R2.

### (E) Estimating Mean Log of Hourly

 Wage
Using the model, the estimated mean log of hourly wage is approximately 2.83. However, this estimate falls outside the 95% confidence interval, indicating that the model underestimates the return to having a degree. To improve the model, consider adding more variables to explain the unaccounted variation in log hourly wage.

---

This README provides a summary of the analysis for the questions in the attached Word document. For a detailed understanding, please refer to the corresponding sections above.
