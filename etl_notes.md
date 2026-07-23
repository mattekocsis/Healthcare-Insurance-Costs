Create new PowerBI report and name it accordingly.

Import Dataset and use Power Query to perform ETL process.
Verify Data Types
    Ensure columns:
        Age and Children are Whole Number;
        BMI and Charges are Decimal Number;
        Sex, Smoker and Region are Text.

Check for Nulls / Duplicates by ensuring the Column Quality and Column Distribution are turned on.
Ensure 0% missing values in dataset.

Standardize categories with Text using Trim / Clean to remove leading or trailing whitespace.
Create Conditional Column "BMI Category" for ease of visualization and comparison.
Create Conditional Column "Age Band" for ease of visualization and conmparison.
Rename columns:
    Capitalize columns;
    Change "children" to "# of Children" and "charges" to "Annual Premium (USD)" for ease of readability.

Double check to ensure all column data types are correct:
    Change "BMI Category" and "Age Band" to text type.

Close & Apply

Create a measures table and add custom DAX measures for:
    Average Charge;
    Average Charge for Non-Smokers;
    Average Charge for Smokers;
    Charge per BMI Point;
    Smoker Premium Multiplier.

Create Executive Review Page
Add KPI Cards for:
    Average Charge;
    Average Charge Snmokers;
    Average Charge Non-Smokers;
    Smoker Premium Multiplier.
Add Clustered Bar Charts for:
    Average Charge by Age Band;
    Average Charge by Region;
    Average Charge by BMI Category and Smoker Status.
Add Slicers for:
    Smoker Status;
    Sex;
    Region.

Create Underwriting Deep-Dive Page
Add Scatter Plots for:
    Annual Premium by BMI, coloured by Smoker Status;
    Annual Premium by Age, coloured by Smoker Status.
        Scatter plots create a clear visual understanding of the data by producing distinct clusters between smokers and non-smokers.
Add Decomposition Tree to break down Annual Premium charge by Smoker Status, BMI Category and Age Band.
Add table with all attributes visible for underwriter review, sorted descending by Annual Premium.

Apply consistent theme and colour coding across the report pages.
