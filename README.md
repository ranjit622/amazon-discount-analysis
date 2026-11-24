# Amazon India: Discount, Pricing & Product Quality Analysis

## 1. Business Problem
An e-commerce category team gives discounts across many product categories, but it is unclear **where discounts actually help** and where they only reduce margin. At the same time, some well-rated products get little visibility, and some poorly rated products sit in high-demand slots.

**Goal:** use product listing data to find where discounts, pricing and product quality need attention, and give clear, actionable recommendations.

## 2. Dataset
- **Source:** Amazon Sales Dataset (Kaggle) - https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset
- **Size:** 1,465 rows, 16 columns
- **Key columns:** `product_name`, `category`, `discounted_price`, `actual_price`, `discount_percentage`, `rating`, `rating_count`, `review_content`
- **Note:** This is product listing data, not transaction data. It has no orders, revenue or profit. `rating_count` is used as a **proxy for demand**.

## 3. Tools Used
Python (pandas, NumPy, Matplotlib, Seaborn), Jupyter Notebook

## 4. Approach
1. Loaded the data and checked data types
2. Cleaned the data: converted price, discount, rating and rating_count to numeric; handled missing values and duplicate products
3. Extracted the main category from the category path
4. Analysed five business problems (below)
5. Visualised the results and wrote recommendations

## 5. Business Questions & Findings

| # | Business Problem | Finding | Recommended Action |
|---|------------------|---------|--------------------|
| 1 | Is the discount strategy working? | [Add your finding, e.g. relationship between discount % and rating_count] | [Add action] |
| 2 | Which categories should the company focus on? | [Add your finding] | [Add action] |
| 3 | Which products have quality risk (low rating, high rating_count)? | [Add your finding] | [Add action] |
| 4 | Where is pricing out of line with the category? | [Add your finding] | [Add action] |
| 5 | Which well-rated products have low visibility (hidden gems)? | [Add your finding] | [Add action] |

## 6. Key Visuals
Add your charts here, for example:
- `category_demand.png` - category-wise demand proxy
- Discount bucket vs median rating_count
- Top 10 risk products / Top 10 hidden gems

## 7. Recommendations
1. [Recommendation 1 based on your findings]
2. [Recommendation 2]
3. [Recommendation 3]

## 8. Limitations
- The dataset is a **snapshot of listings**, so there is no time trend or seasonality.
- `rating_count` is a **proxy** for demand, not actual sales.
- Correlation does not prove causation. A link between discount and demand does not mean the discount caused it.
- Sales, revenue and profit data would make the analysis much stronger.

## 9. Project Structure
- `data/` - raw dataset
- `notebook.ipynb` - cleaning and analysis
- `images/` - saved charts
- `README.md` - this file

## 10. Author
Ranjit - aspiring Data Analyst
