Superstore Sales Dashboard (Power BI)

An interactive three-page Power BI dashboard that analyses four years of retail orders (2014 to 2017). It shows how sales, profit and discounts move across time, customer segments and product categories, and pinpoints where the business loses money.

Tech Stack :
Data cleaning (ETL) - Power Query
Data modelling -  Star schema - 1 fact table aur 3 dimension tables, one-to-many relationships
DAX Calculations - Measures (SUM, DIVIDE, DISTINCTCOUNT, CALCULATE, SAMEPERIODLASTYEAR) aur Date table (CALENDAR)
Power BI Desktop	 - Cards, line chart, bar charts, matrix, table, slicers, Top N filters, conditional formatting

Data Source- The data comes from the Sample Superstore dataset on [Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final). It contains 9,994 order lines (21 columns) from a fictional US retailer, covering January 2014 to December 2017. After removing 1 duplicate row, 9,993 rows were used. This is a public sample dataset used for learning and portfolio purposes only.

Highlights :
  A retail store sells furniture, office supplies and technology products to three customer segments. Sales grew strongly in 2016 and 2017, but the profit margin is only 12.47%, and some sub-categories lose money even when they sell well.

The store does not clearly know:

- Where its profit is coming from, and where it is leaking
- Which products and sub-categories lose money
- Whether heavy discounting is the reason for those losses
- Which customer segment and which months matter most

This project builds a dashboard that answers these questions and turns the findings into simple recommendations.

The goal of this dashboard is to help a retail business understand how it is performing and where it is losing money. It tracks sales, profit and orders over time, and shows which customer segments, product categories and products drive profit or loss. The findings are turned into simple recommendations, such as where to review discounts.

Analysed 9,993 order lines ($2.30M sales, $286.41K profit, 12.47% margin)
- Cleaned the data in Power Query: fixed data types, removed 1 duplicate row and built a staging query
- Sales grew 29.47% in 2016 and 20.36% in 2017 after a small dip in 2015
- Found three loss-making sub-categories (Tables, Bookcases, Supplies), about $22.4K combined
- Showed that high discounts are linked to some losses (Tables 26%, Bookcases 21% vs 15.6% overall), but not all of them
