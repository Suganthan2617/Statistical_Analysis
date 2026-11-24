# Statistical Analysis: Airbnb Nightly Prices in Seattle

## 1. Research Question

Is there a statistically significant difference in average nightly prices between entire-home listings and private-room listings in Seattle?

## 2. Hypotheses

- **Null Hypothesis (H₀):** There is no difference in average nightly prices between entire-home and private-room listings.
- **Alternative Hypothesis (H₁):** There is a difference in average nightly prices between the two groups.

Significance level: α = 0.05.

## 3. Dataset Description

The analysis uses the Inside Airbnb Seattle listings dataset.

- Original observations: 7,657
- Original columns: 19
- Entire-home listings analyzed: 5,267
- Private-room listings analyzed: 1,191
- Missing prices in the two selected room types excluded: 1,124

Hotel-room and shared-room listings were excluded because the research question focuses on two specific groups. Listings with missing prices were also excluded.

## 4. Statistical Method

Welch's independent two-sample t-test was selected because nightly price is a continuous variable and we are comparing the means of two independent groups.

Welch's test is appropriate when the two groups have unequal variances.

## 5. Assumption Checking

**Equal variance assumption:**

Levene's test:
- Test statistic: 9.1363
- P-value: 0.00252

Since the p-value is below 0.05, the equal variance assumption was rejected.

**Distribution and normality:**

- Entire-home price skewness: 17.68
- Private-room price skewness: 7.58

Both groups are strongly right-skewed and contain extreme price outliers.

The large sample sizes support using the Central Limit Theorem for inference about means. However, the extreme skewness and outliers remain limitations.

## 6. Descriptive Statistics

| Measurement | Entire Home | Private Room |
|---|---:|---:|
| Sample size | 5,267 | 1,191 |
| Average nightly price | $298.41 | $170.28 |

Observed average price difference: $128.13.

## 7. Hypothesis Test Results

Welch's independent two-sample t-test produced:

- T-statistic: 15.0066
- Degrees of freedom: 2311.00
- P-value: 1.2055 × 10⁻⁴⁸
- Significance level: 0.05
- 95% confidence interval: $111.39 to $144.87

Since the p-value is much smaller than 0.05, the null hypothesis is rejected.

There is strong statistical evidence of a difference in average nightly prices between the two listing types.

## 8. Practical Significance

The average nightly price difference was $128.13.

Entire-home listings were approximately 75.25% more expensive than private-room listings in this sample.

This is a substantial observed difference and may be meaningful to people comparing accommodation options. However, extreme prices can influence averages.

## 9. Conclusion

The statistical analysis found a significant difference in average nightly prices between entire-home and private-room Airbnb listings in Seattle.

Entire-home listings had an average nightly price of $298.41, compared with $170.28 for private rooms.

The Welch's t-test returned a t-statistic of 15.0066 and a p-value of approximately 1.21 × 10⁻⁴⁸. Since this p-value is below the 0.05 significance level, the null hypothesis was rejected.

The 95% confidence interval suggests that the average price difference lies between $111.39 and $144.87.

In simple terms, entire-home listings were considerably more expensive than private rooms in the analyzed dataset.

This analysis demonstrates a statistical difference, not a causal relationship. The findings are also subject to limitations from extreme price outliers and skewed distributions.