# A/B Test Analysis for the Mobile Game "Cookie Cats"
## 1.Project Overview & Business Problem
The developer of the mobile game "Cookie Cats" conducted an A/B test to evaluate how changing the position of a "gate" from level 30 to level 40 affects player retention. The goal of this analysis is to determine the test's outcome and provide a data-driven recommendation on whether to implement this change for all players.
## 2. Tech Stack
* ### Python
* ### Pandas
* ### SciPy
* ### Matplotlib / Seaborn
* ### Jupyter Notebook
## 3. Analysis Steps
### 1. **Data Loading and Cleaning:** Load the dataset and check for any inconsistencies or missing values.
### 2. **Exploratory Data Analysis (EDA):** Perform an initial investigation of the data to understand the distribution of players and their overall behavior.
### 3. **Hypothesis Formulation:** Define the Null (H₀) and Alternative (H₁) hypotheses for the A/B test.
### 4. **Metric Calculation:** Calculate 1-day and 7-day retention rates for both the control and test groups.
### 5. **Statistical Testing:** Conduct a Chi-squared test to determine if the observed difference is statistically significant.
### 6. **Result Visualization:** Create a pointplot to visually compare the retention rates of the two groups.
## 4. Key Findings & Results
The statistical analysis and visualization provided a clear and mixed outcome:
* ### For 1-Day Retention:
    * ***gate_30*** rate: ~44.8%
    * ***gate_40*** rate: ~44.2%
    * **P-value**: 0.075
    * Conclusion: Since the p-value (0.075) is greater than our significance level (0.05), we fail to reject the null hypothesis. There is no statistically significant difference in 1-day retention.
* ### For 7-Day Retention:
    * ***gate_30*** rate: ~19.0%
    * ***gate_40*** rate: ~18.2%
    * **P-value**: 0.0016
    * Conclusion: Since the p-value (0.0016) is much smaller than our significance level (0.05), we reject the null hypothesis. There is a statistically significant difference in 7-day retention.
## 5. Business Recommendation
### **Recommendation: Do Not Implement the Change.**
### The analysis shows that moving the gate from level 30 to level 40 has no significant short-term benefit but results in a statistically significant decrease in 7-day player retention.

### This indicates that the earlier gate at level 30 is more effective at keeping players engaged in the long run. Therefore, the business should keep the gate at level 30 to maintain higher long-term player retention.