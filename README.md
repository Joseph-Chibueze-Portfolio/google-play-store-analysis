# Google Play Store Data Analysis Project 🚀

> Project Dashboard: [View Interactive Power BI Report](INSERT_YOUR_PUBLIC_LINK_HERE)

> Project Files: [Download .pbix Source File](INSERT_LINK_TO_YOUR_PBIX_FILE_IN_GITHUB)

---

## Project Overview
This project involved transforming a messy, raw dataset of 11,500+ Google Play Store entries into a clean, analytical-ready format. The goal was to uncover market trends, app performance metrics, and user preferences through data modeling and visualization in Power BI.

## Dashboard Preview
![Dashboard Overview](images/dashboard_screenshot.png)

---

## Data Cleaning & Transformation Pipeline
Data was processed entirely within Power BI's Power Query Editor to ensure an automated, repeatable pipeline:
*   Deduplication: Removed duplicate app listings to isolate 2,377 unique, high-quality records.
*   Missing Value Imputation: Applied a median imputation (4.1) to missing ratings, ensuring a statistically sound average without skewing the analysis.
*   Feature Engineering:
    *   Size Standardization: Built a conditional column to isolate numerical values from "M" suffixes, converting text to a decimal format for meaningful AVERAGE calculations.
    *   Version Structuring: Decomposed "Current Version" and "Android Version" strings into Major, Minor, and Patch segments, enabling chronological version analysis.
    *   Genre Mapping: Utilized delimiter-based splitting to separate complex genre strings into Primary Genre and Sub-Genre for granular filtering.

## Technical Highlights
*   DAX KPI Development: Created a 5-KPI dashboard (Total Apps, Average Rating, Total Reviews, Top Category, and Maximum Price) for immediate business context.
*   Dynamic DAX Measures:
    *   *Top Category:* Implemented TOPN combined with VALUES to dynamically identify the most prominent category.
    *   *Monetization Metrics:* Developed dedicated measures using CALCULATE(COUNTROWS(...)) to compare Free vs. Paid app distribution.
*   Visual Analysis: Enabled cross-functional insights by standardizing data types, allowing for correlation analysis between app size and user reception.

## Key Analytical Questions Solved
1.  Market Saturation: Which five genres have the highest number of apps available?
2.  Pricing Analysis: Which specific apps are the most expensive?
3.  Performance Correlation: Does app size (MB) impact the average user rating?
4.  Monetization Distribution: What is the ratio between free and paid apps in the ecosystem?

## Tools Used
*   Data Preparation: Power BI (Power Query)
*   Modeling & Visualization: Power BI
*   Analytical Language: DAX (Data Analysis Expressions)

## Data Attribution
The dataset utilized for this analysis is the public Google Play Store Dataset. This data was leveraged to simulate real-world app market analytics and demonstrate end-to-end data processing workflows.

---
*Author: Joseph Chibueze (JojoTechMan)*
