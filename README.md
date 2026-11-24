# Airbnb Statistical Analysis

## Project Overview

This project performs statistical hypothesis testing on the Inside Airbnb Seattle listings dataset to determine whether average nightly prices differ significantly between entire-home listings and private-room listings.

## Research Question

Is there a statistically significant difference in average nightly prices between entire-home and private-room Airbnb listings in Seattle?

## Hypotheses

- **Null Hypothesis (H₀):** There is no difference in average nightly prices between the two groups.
- **Alternative Hypothesis (H₁):** There is a difference in average nightly prices between the two groups.

Significance level: 0.05.

## Tools and Technologies

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Statistical Methods

- Descriptive statistics
- Boxplot visualization
- Levene's test for equality of variances
- Welch's independent two-sample t-test
- 95% confidence interval

## Key Findings

| Measurement | Entire Home | Private Room |
|---|---:|---:|
| Sample size | 5,267 | 1,191 |
| Average price | $298.41 | $170.28 |

**Hypothesis test results:**

- T-statistic: 15.0066
- P-value: 1.2055 × 10⁻⁴⁸
- 95% confidence interval: $111.39 to $144.87
- Decision: Reject the null hypothesis.

Entire-home listings had an average nightly price approximately 75.25% higher than private-room listings in the analyzed sample.

## Project Files

- `Statistical_Analysis.ipynb` - Complete Python statistical analysis.
- `Statistical_Analysis_Report.md` - Written findings report.
- `raw_dataset.csv` - Original dataset (download separately).
- `.gitignore` - Files excluded from Git.

## How to Run

1. Clone this repository.
2. Download the Seattle listings dataset from [Inside Airbnb](https://insideairbnb.com/get-the-data/).
3. Place the downloaded file in the project folder and name it `raw_dataset.csv`.
4. Install the required libraries:

   `pip install pandas numpy matplotlib seaborn scipy jupyter ipykernel`

5. Open `Statistical_Analysis.ipynb` in Jupyter Notebook or VS Code.
6. Run all cells.

## Conclusion

The analysis found strong statistical evidence that average nightly prices differ between entire-home and private-room Airbnb listings in Seattle.

The results should be interpreted with caution because both price distributions contain extreme outliers and are strongly right-skewed.