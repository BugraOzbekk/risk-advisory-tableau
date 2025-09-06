# Risk Analysis of 1000 Companies

## Project Overview
This project focuses on analyzing 1,000 simulated companies to identify financially vulnerable firms.  
The dataset was originally sourced from Kaggle and enriched with synthetic company names and IDs (using the Faker library).  
New financial metrics were engineered to allow deeper analysis.  
The final dashboard highlights companies with high expenses but low profitability, which may indicate potential risk.

---

## Data Preparation
- Added **ID** and synthetic **Company Name** fields using Python (Faker library).  
- Exported the dataset to CSV and Excel for use in Tableau.  
- Created new financial metrics:  
  - **Total Expenses** = R&D Spend + Administration + Marketing Spend  
  - **Profitability Ratio** = Profit / Total Expenses  
- The final dataset is stored in: `data/1000_companies_final.xlsx`

---

## Tableau Dashboard
A Tableau dashboard was developed to visualize company risk levels.

### Key Features
- **Scatter Plot (Expenses vs. Profit):** Companies positioned by their expenses and profit.  
- **Dynamic Parameters:**  
  - Expenses Cutoff  
  - Profit Cutoff  
  - Worst Profit Ratios  
- **Sets and Filters:** Highlight high-expense and low-profit companies.  
- **Risk Quadrant:** Companies falling into both categories (high expenses, low profit) are highlighted as high-risk.  
- **Worst Profit Ratio List:** A dynamic table on the right shows the companies with the lowest profitability ratios.  
- **Reference Lines & Drop Lines:** Cutoff thresholds are clearly marked to guide analysis.  
- **Interactivity:** Users can adjust cutoffs and ratios dynamically to explore different risk scenarios.  

---

## Insights
- Companies with **high expenses and low profits** are visualized in the risk quadrant.  
- The **Worst Profit Ratio list** provides a ranked view of the weakest performers.  
- **Red points** in the scatter plot represent companies that appear in **both sets** (high expenses + low profit ratio), identifying them as the most vulnerable firms.  
