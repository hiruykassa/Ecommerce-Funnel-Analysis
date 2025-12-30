# Data Directory

## Structure
```
data/
├── raw/              # Original, unmodified dataset
└── processed/        # Cleaned and transformed data
```

## Dataset Information

### Online Retail Dataset
**Source:** UCI Machine Learning Repository

**Download Instructions:**
1. Visit: https://archive.ics.uci.edu/ml/datasets/online+retail
2. Download the file: `Online Retail.xlsx`
3. Place it in the `data/raw/` folder
4. Do NOT commit this file to GitHub (it's in .gitignore)

### Dataset Description
This is a transnational dataset containing all transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based online retail company.

**Columns:**
- `InvoiceNo`: Invoice number (6-digit integral number uniquely assigned to each transaction)
- `StockCode`: Product code (5-digit integral number uniquely assigned to each distinct product)
- `Description`: Product name
- `Quantity`: Quantities of each product per transaction
- `InvoiceDate`: Invoice date and time
- `UnitPrice`: Unit price in sterling (£)
- `CustomerID`: Customer number (5-digit integral number uniquely assigned to each customer)
- `Country`: Country name where customer resides

**Size:** ~540,000 records

### Data Quality Notes
- Some transactions have missing CustomerIDs
- Negative quantities indicate returns/cancellations
- Need to handle missing values and outliers
- Dates need to be parsed correctly

## Usage
Do not commit large data files to GitHub. Use the `.gitignore` file to exclude:
- `data/raw/*.xlsx`
- `data/processed/*.csv`

Instead, document where to download the data and how to reproduce the processed datasets.