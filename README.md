## Lab Activity 4.3 — Analyzing Student Performance Using T-Tests and Z-Tests
Objective
To determine whether there are statistically significant differences in student performance based on gender and study time using T-Tests and Z-Tests.

Dataset
Student Performance Dataset from UCI Machine Learning Repository:
🔗 UCI Dataset Link

Requirements

Computer with Python and Jupyter Notebook installed
Python Libraries: pandas, numpy, matplotlib, seaborn, scipy, statsmodels


Prerequisites

Basic Python programming knowledge
Understanding of statistics, especially hypothesis testing
Familiarity with pandas for data manipulation
Understanding of data visualization using matplotlib and seaborn


Problem Statement
This activity analyzes the impact of gender and study time on student academic performance using statistical hypothesis testing. By applying T-Tests and Z-Tests, the goal is to determine if score differences are statistically significant and provide insights for data-driven educational decisions.

Steps
StepTask1Import required libraries2Load dataset (student_performance.csv, semicolon-separated)3Check for missing values, display df.info() and df.describe()4EDA — visualize grade distribution by gender and study time (boxplots)5Perform Welch's T-Test to compare male vs female final grades (G3)6Perform Z-Test to compare low study time (≤2) vs high study time (>2) groups7Interpret results using significance level α = 0.05

Hypothesis
T-Test (Gender-based)
HypothesisStatementH₀No significant difference in performance based on genderH₁A significant difference exists between male and female scores
Z-Test (Study Time-based)
HypothesisStatementH₀No significant difference in performance based on study timeH₁Study time significantly affects student performance

Decision Rule
ResultConclusionp-value < 0.05Reject H₀ — significant difference existsp-value ≥ 0.05Fail to reject H₀ — no significant difference

When to Use Which Test
TestUsed ForT-Test (Welch's)Comparing two groups with potentially unequal variances (e.g., male vs female)Z-TestComparing two groups when sample size is large (e.g., low vs high study time)

Visualizations

Boxplot — Final grades (G3) distribution by gender
Boxplot — Final grades (G3) distribution by study time groups


Tech Stack
LibraryUsagepandasData loading and manipulationnumpyNumerical operationsmatplotlibPlottingseabornBoxplot visualizationsscipyT-Test (ttest_ind)statsmodelsZ-Test (ztest)

File Structure
Lab4_3/
├── Lab4_3.ipynb                  # Main notebook
├── student_performance.csv       # Dataset (semicolon-separated)
└── README.md                     # This file

Conclusion
The T-Test and Z-Test results reveal whether gender and study time have a measurable impact on student academic performance. A p-value below 0.05 confirms a significant difference, helping educators identify key factors that influence learning outcomes and make informed decisions to improve student success.
