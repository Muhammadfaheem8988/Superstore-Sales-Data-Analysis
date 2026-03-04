# Superstore Sales Data Analysis

A hands-on exploratory data analysis project built around the popular Superstore retail dataset. The goal here is pretty straightforward — dig into the sales and profit numbers, figure out what's actually working (and what isn't), and pull out insights that could help a business make better decisions.

Everything is done in Python using Pandas, NumPy, Matplotlib, and Seaborn.

## What This Project Covers

The analysis is organized around seven specific questions:

1. Which products are selling the most?
2. Which region brings in the highest sales?
3. What are the top cities driving revenue?
4. Are there products that are consistently losing money?
5. How do sales change month over month and year over year — any seasonal patterns?
6. Which products generate the most profit?
7. Which products keep showing up as loss-makers?

## Dataset Overview

The dataset (`Sample - Superstore.csv`) contains **9,994 order records** with **21 columns**, including:

| Column | Description |
|--------|-------------|
| Order ID / Order Date / Ship Date | Order tracking and timing |
| Ship Mode | Shipping method used |
| Customer ID / Customer Name / Segment | Customer details (Consumer, Corporate, Home Office) |
| Country / City / State / Region | Geographic info (United States) |
| Product ID / Category / Sub-Category / Product Name | Product details across Furniture, Office Supplies, and Technology |
| Sales / Quantity / Discount / Profit | The key numbers we're analyzing |

The data is clean — no missing values at all — so the notebook jumps straight into exploration after a quick sanity check.

## How the Analysis Works

The notebook walks through things step by step:

1. **Encoding detection** — Uses `chardet` to figure out the file encoding (turns out it's ISO-8859-1)
2. **Loading and inspecting the data** — Basic checks with `.head()`, `.info()`, `.describe()` to get a feel for the dataset
3. **Null value checks** — Confirms there are zero missing values across all columns and rows
4. **Exploratory analysis and visualizations** — The main part: bar charts, trend lines, and breakdowns by category, region, time period, and customer segment

## Key Findings

- **Technology and Office Supplies** are the profit drivers. Furniture, on the other hand, has noticeably thinner margins.
- The **West and East regions** tend to outperform the South and Central regions when it comes to profit.
- There are clear **seasonal spikes** in sales — certain months (especially toward year-end) see a big jump.
- The **Consumer segment** pulls in the most profit compared to Corporate and Home Office.
- Some products are **consistently unprofitable**

## Project Structure

```
├── Superstore_sales_data_Analysis.ipynb   # Main analysis notebook
├── Sample - Superstore.csv                # The dataset
├── Requirnments.txt                       # Python dependencies
└── README.md                              # You're reading it
```

## Installation & Requirements
1. Clone this repository.
2. Ensure Python 3.7+ is installed.  
3. Install required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`.  
4. Download the dataset (`superstore.csv`) from the repository.  
5. Open `analysis_notebook.ipynb` in Jupyter or Google Colab and run all cells.

## Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/Muhammadfaheem8988/Superstore-Sales-Data-Analysis.git
   ```
2. Make sure you have **Python 3.7+** installed.
3. Install the dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn chardet
   ```
4. Open `Superstore_sales_data_Analysis.ipynb` in Jupyter Notebook or Google Colab and run the cells top to bottom.
 


## Future Work

- Build a predictive model to forecast future sales and profit trends.
- Add interactive dashboards (maybe with Plotly or Streamlit).
- Take a deeper look at how discounts affect profitability — the data hints at a strong connection there.

---

**Author:** Muhammad Faheem
