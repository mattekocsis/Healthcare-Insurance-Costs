# Healthcare Insurance Costs
Medical Insurance Cost Analysis and Premium Pricing Dashboard using PowerBI

Purpose: Build a dashboard for underwriting / actuarial team to identify which individual factors most influence medical insurance costs, and analyze which customer segments are systematically under or overpriced relative to their risk factors.

Data Source: Medical Cost Personal Dataset - https://www.kaggle.com/datasets/mirichoi0218/insurance

Data size: 7 columns, 1338 rows

Tools used:
- PowerBI Desktop (ETL/PowerQuery, data modeling, dahsboarding)
- VSCode (preview .csv file of dataset, write markdown of ETL notes)

ETL Process:
- Import Dataset and use Power Query to perform ETL process.
- Verify Data Types
- Ensure columns:
    - Age and Children are Whole Number;
    - BMI and Charges are Decimal Number;
    - Sex, Smoker and Region are Text.

- Check for Nulls / Duplicates by ensuring the Column Quality and Column Distribution are turned on.
- Ensure 0% missing values in dataset.

- Standardize categories with Text using Trim / Clean to remove leading or trailing whitespace.
- Create Conditional Column "BMI Category" for ease of visualization and comparison.
- Create Conditional Column "Age Band" for ease of visualization and conmparison.
- Rename columns:
    - Capitalize columns;
    - Change "children" to "# of Children" and "charges" to "Annual Premium (USD)" for ease of readability.

- Double check to ensure all column data types are correct:
    - Change "BMI Category" and "Age Band" to text type.

Close & Apply

Data Model: Dataset and Measures Table
<img width="760" height="510" alt="image" src="https://github.com/user-attachments/assets/de122a93-feb1-44a0-a21f-6cdabae14265" />

Dashboard Screenshots:

Executive Overview:
<img width="781" height="452" alt="DashboardTab1" src="https://github.com/user-attachments/assets/239fd766-4dbf-42d5-abaf-90057d3de18b" />
Underwriting Deep-Dive:
<img width="781" height="452" alt="DashboardTab2" src="https://github.com/user-attachments/assets/3e62372a-a5d4-4776-b1b7-8da7ced2c8c9" />

Key Findings:
  - Smoking Status is the single largest driver of annual premium charges, with smokers paying 3.8 times more on average than non-smokers.
  - The effect of BMI on annual charges was strongly conditional to smoking status, with smokers with a higher BMI beinmg associated with a much steeper cost increase.
  - Age showed a linear relationship independent of other factors.
  - Region accounted for minimal variation in charges relative to smoking status and BMI

Business Recommendation: Based in the findings, the insurer's pricing model should consider smoking status and the BMI to smoking status interaction more heavily than other factors as these explain most of the variance in claims costs.

Limitations: The dataset is a single cross-sectional snapshot with a sample size of 1338 individuals and does not include information regarding occupation, pre-existing health conditions or past claims history, all of which are considered as factors in a real underwriting model.
