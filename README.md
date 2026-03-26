This project focuses on performing Exploratory Data Analysis (EDA) using MySQL to uncover insights and trends from a global layoffs dataset. The analysis aims to identify which industries, countries, and funding stages were most impacted by workforce reductions, as well as tracking the progression of layoffs over time.

Dataset Description
The dataset used is layoff_staging2, which contains cleaned data regarding company layoffs. Key columns include:
Company: Name of the organization.
Location: HQ of the company.
Industry: Sector (e.g., Tech, Finance, Retail).
Total_laid_off: Number of employees let go.
Percentage_laid_off: Fraction of the company's workforce affected.
Date: Date of the layoff event.
Stage: Funding stage (e.g., Series B, Post-IPO).
Funds_raised_millions: Total capital raised by the company.
https://github.com/KanakSharma0308/SQL-Exploratory-Data-Analysis-Layoffs/blob/main/layoffs.csv

Key Business Questions Answered
The SQL scripts in this repository answer several critical questions:
Which companies had the highest number of layoffs in a single event?
Which industries and countries faced the most significant workforce reductions?
How did layoffs progress month-over-month (Rolling Total analysis)?
Who were the "Top 5" companies with the most layoffs for each specific year?

SQL Techniques Applied
I utilized several advanced SQL features to perform this analysis:
Common Table Expressions (CTEs): Used to create modular and readable queries, especially for ranking and rolling totals.
Window Functions: Applied SUM() OVER() for rolling totals and DENSE_RANK() to categorize company rankings.
Aggregations: Extensive use of SUM, MAX, MIN, and GROUP BY to summarize data.
String & Date Manipulation: Used SUBSTRING and YEAR() functions to format dates for time-series analysis.


