# Task 4: Data Storytelling & Statistical Validation

## ApexPlanet Data Analytics Internship

## Project Objective

This project completes **Task 4: Data Storytelling & Statistical Validation** of the ApexPlanet Data Analytics Internship. It brings together the work completed in Tasks 1-3 into a business-focused presentation and uses statistical testing to validate a key finding.

## Business Objective

The objective was to analyse sales performance, customer behaviour, and revenue opportunities, then convert the findings into practical business recommendations supported by data.

## Project Journey

| Task | Focus | Output Used in This Project |
|---|---|---|
| Task 1 | Data Immersion & Wrangling | Cleaned and analysis-ready sales dataset |
| Task 2 | EDA & Business Intelligence | Sales trends, category, product, and city insights |
| Task 3 | Deep-Dive Analysis & Dashboarding | Customer segmentation and interactive Power BI dashboard |
| Task 4 | Data Storytelling & Statistical Validation | Presentation, hypothesis test, conclusions, and recommendations |

## Dataset Overview

- **Records:** 1,000 sales transactions
- **Key fields:** Order Date, Customer ID, Gender, City, Product, Category, Quantity, Unit Price, and Total Sales
- **Source:** Cleaned dataset prepared in Task 1

## Key Business Insights

- Total revenue was **₹139.40M** across 1,000 sales transactions.
- Electronics generated the highest category revenue at approximately **₹50.78M**
- Patna was the highest-revenue city at approximately **₹19.29M**.
- High-value customers generated approximately **₹77.05M**, representing the largest revenue contribution among customer segments.
- Customer value and purchase behaviour provide a stronger basis for targeting than gender alone.

## Hypothesis Testing

### Business Question

Do male and female customers have significantly different average total sales?

### Hypotheses

- **H0 (Null Hypothesis):** There is no statistically significant difference in average total sales between male and female customers.
- **H1 (Alternative Hypothesis):** There is a statistically significant difference in average total sales between male and female customers.

### Test Used

**Welch Independent Samples T-Test** was used because the two gender groups are independent and the test does not assume equal variance.

### Test Results

| Metric | Result |
|---|---:|
| Male average sales | ₹141,807.34 |
| Female average sales | ₹136,883.21 |
| Male sample size | 511 |
| Female sample size | 489 |
| T-statistic | 0.6826 |
| P-value | 0.4950 |
| Significance level | 0.05 |

### Interpretation

Since the p-value (**0.4950**) is greater than the significance level (**0.05**), the null hypothesis cannot be rejected.

**Conclusion:** There is no statistically significant difference in average sales between male and female customers. Therefore, gender alone should not be used as the primary basis for sales targeting.
## Business Recommendations

1. Retain high-value customers through personalised offers, loyalty benefits, and proactive support.
2. Use cross-sell and upsell campaigns to grow medium-value customers.
3. Prioritise electronics, high-performing products, and high-revenue cities in sales planning.
4. Use customer segment, city, category, and purchase behaviour for targeted campaigns.
5. Avoid gender-only targeting because the statistical test did not identify a significant difference in average sales.

## Deliverables

```text
ApexPlanet-Task4-Data-Storytelling-Statistical-Validation/
|
|-- README.md
|-- Task4_Data_Storytelling_Statistical_Validation.pptx
|-- Task4_Hypothesis_Testing.ipynb
```

## Tools Used

- Power BI Desktop
- Python
- Pandas
- SciPy
- Google Colab
- Microsoft PowerPoint

## Skills Demonstrated

- Data storytelling
- Business presentation design
- Exploratory Data Analysis (EDA)
- Customer segmentation
- Statistical hypothesis testing
- Welch Independent Samples T-Test
- P-value interpretation
- Business insight generation

## How to Run the Hypothesis Test

1. Open `Task4_Hypothesis_Testing.ipynb` in Google Colab or Jupyter Notebook.
2. Upload `Task1_Cleaned_Dataset.xlsx`.
3. Run all cells in sequence.
4. Review the male/female mean sales, t-statistic, p-value, and decision.
