# SmartSupply Insights
## Supply Chain Performance, Delivery Risk & Profitability Analytics

**AICTE | IBM SkillsBuild Data Analytics with AI — Academic Internship 2026**

**Submitted by:** Himani Mane

---

## Project Overview

SmartSupply Insights is a complete end-to-end data analytics project applied to the **DataCo SMART SUPPLY CHAIN FOR BIG DATA ANALYSIS** dataset. The project analyzes 180,519 supply-chain transactions spanning January 2015 to January 2018, covering profitability drivers, delivery risk patterns, customer performance, product performance, regional and market analysis, and shipping operations.

---

## Problem Statement

Supply-chain organisations face persistent challenges in understanding operational efficiency, delivery reliability, and profitability. This project addresses:

- Which product categories and markets drive revenue and profit?
- What factors are associated with late deliveries (54.8% rate)?
- Where are discounts eroding profitability (18.7% negative-profit orders)?
- Can delivery risk be predicted from pre-shipment data for proactive intervention?

---

## Objectives

1. Understand the supply-chain dataset structure and perform data quality assessment
2. Clean and preprocess data following professional standards
3. Engineer meaningful analytical features
4. Calculate key business KPIs
5. Perform comprehensive EDA across all business dimensions
6. Investigate late-delivery patterns by region, market, and shipping mode
7. Build and evaluate ML models for late-delivery risk prediction
8. Generate evidence-based business recommendations

---

## Dataset

**Dataset:** DataCo SMART SUPPLY CHAIN FOR BIG DATA ANALYSIS

| Attribute | Value |
|-----------|-------|
| Records | 180,519 |
| Features | 53 |
| Date Range | Jan 2015 – Jan 2018 |
| Markets | Africa, Europe, LATAM, Pacific Asia, USCA |

**Kaggle Source:**
https://www.kaggle.com/datasets/alinoranianesfahani/dataco-smart-supply-chain-for-big-data-analysis

**Original Source (Mendeley Data):**
https://data.mendeley.com/datasets/8gx2fvg2k6/5

**DOI:** 10.17632/8gx2fvg2k6.5

---

## Dataset Setup

> **Important:** The dataset is NOT included in this repository. You must download it separately.

1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/alinoranianesfahani/dataco-smart-supply-chain-for-big-data-analysis)
2. Extract the ZIP file
3. Place the following files inside the `data/` directory:
   - `DataCoSupplyChainDataset.csv`
   - `DescriptionDataCoSupplyChain.csv`
4. Open `HimaniMane_SmartSupply_Insights.ipynb`
5. Run all cells from top to bottom

The notebook uses relative paths (`data/DataCoSupplyChainDataset.csv`) and will work from any machine where the dataset is placed in the `data/` folder.

---

## Technologies Used

| Technology | Purpose |
|------------|---------|
| Python 3.x | Core language |
| Pandas | Data manipulation |
| NumPy | Numerical computing |
| Matplotlib | Visualisation |
| Seaborn | Statistical visualisation |
| Scikit-learn | Machine learning |
| Jupyter Notebook | Interactive analysis |
| Python-docx | Word report |

---

## Project Workflow

```
Dataset
   ↓
Data Loading & Understanding
   ↓
Data Quality Assessment
   ↓
Data Cleaning & Preprocessing
   ↓
Feature Engineering
   ↓
KPI Calculation
   ↓
Exploratory Data Analysis
   ↓
Business Analysis (Sales, Profit, Customers, Products, Regions, Markets, Shipping)
   ↓
Delivery Risk Analysis
   ↓
Machine Learning (Late Delivery Risk Prediction)
   ↓
Model Evaluation & Comparison
   ↓
Insights & Business Recommendations
   ↓
Professional Report Generation
```

---

## Main Code

The complete executable project code is contained in a single notebook:

**`HimaniMane_SmartSupply_Insights.ipynb`**

This notebook covers all 33 sections from Executive Summary through References and is the only file an evaluator needs to open to understand and execute the complete analytical project.

---

## Analysis Images

The notebook generates 27 analytical charts saved as high-resolution PNG files in the `analysis_images/` directory:

| Image | Description |
|-------|-------------|
| `sales_by_category.png` | Top 15 categories by sales |
| `sales_trend.png` | Monthly sales trend |
| `sales_by_region.png` | Sales by order region |
| `sales_by_market.png` | Sales by market |
| `profit_by_category.png` | Profit by category |
| `profit_trend.png` | Monthly profit trend |
| `profit_by_region.png` | Profit by region |
| `profit_by_market.png` | Profit by market |
| `customer_segment_distribution.png` | Customer segment breakdown |
| `customer_segment_sales.png` | Sales by segment |
| `customer_segment_profit.png` | Profit by segment |
| `top_products.png` | Top products by sales |
| `top_profitable_products.png` | Top products by profit |
| `low_profit_products.png` | Low/negative profit products |
| `shipping_mode_distribution.png` | Shipping mode distribution |
| `shipping_mode_performance.png` | Shipping mode vs delivery |
| `late_delivery_distribution.png` | Delivery status distribution |
| `late_delivery_by_region.png` | Late delivery rate by region |
| `late_delivery_by_market.png` | Late delivery rate by market |
| `correlation_heatmap.png` | Correlation heatmap |
| `discount_vs_profit.png` | Discount rate vs profit |
| `sales_vs_profit.png` | Sales vs profit |
| `shipping_cost_vs_profit.png` | Discount amount vs profit |
| `model_comparison.png` | ML model comparison |
| `confusion_matrix.png` | Best model confusion matrix |
| `feature_importance.png` | Random Forest feature importance |
| `roc_curve.png` | ROC curves — all models |

---

## Project Structure

```
SmartSupply-Insights/
│
├── HimaniMane_SmartSupply_Insights.ipynb       ← Main analysis notebook
├── HimaniMane_SmartSupply_ProjectReport.docx   ← Professional project report
├── requirements.txt                             ← Python dependencies
├── README.md                                    ← This file
├── .gitignore                                   ← Git ignore rules
│
├── data/                                        ← Dataset directory (not in repo)
│   ├── DataCoSupplyChainDataset.csv
│   └── DescriptionDataCoSupplyChain.csv
│
└── analysis_images/                             ← Generated chart images (27 files)
    ├── sales_by_category.png
    ├── profit_by_category.png
    ├── ...
    └── roc_curve.png
```

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Running the Project

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Ensure dataset is in data/ directory
# (see Dataset Setup above)

# 3. Launch Jupyter Notebook
jupyter notebook HimaniMane_SmartSupply_Insights.ipynb

# 4. Run all cells: Kernel → Restart & Run All
```

---

## Key Findings

*(All values are from the actual dataset — no fabrication)*

1. **Total Sales:** $36,784,735 | **Total Profit:** $3,966,903 | **Margin:** 10.78%
2. **Late Delivery Rate:** 54.8% — more than half of all orders are delayed
3. **Negative Profit Orders:** 18.7% — significant operational loss exposure
4. **Top Category:** Fishing (highest sales and highest profit)
5. **Top Market:** Europe (highest sales and highest profit)
6. **Discount-Profit:** Weak negative association (r = -0.019)
7. **ML Model:** Random Forest achieves AUC = 0.7481 for delivery risk prediction
8. **Top Delivery Risk Predictors:** Shipping Mode (41%) and Scheduled Days (38%)
9. **Central Africa:** Highest late delivery rate (58.0%)
10. **Canada:** Lowest late delivery rate (48.8%)

---

## Business Recommendations

1. Deploy delivery risk early warning system using the trained Random Forest model
2. Fix scheduling accuracy — actual days (3.50) consistently exceed scheduled (2.93)
3. Investigate and reduce the 18.7% negative-profit orders through pricing guardrails
4. Review discount policy for categories with high discount rates and low margins
5. Optimise shipping mode selection aligned with delivery SLA performance
6. Address regional delivery disparities, especially in Central Africa
7. Protect and grow the Fishing category as the highest-performing portfolio asset

---

## Limitations

- No direct shipping cost per order in the dataset
- Static historical data (2015–2018 only)
- PII fields are masked; individual customer analysis is limited
- Product Description is entirely missing (100% null)
- ML model AUC ~0.75 — some delivery risk variance is unexplained

---

## Future Scope

- Deploy prediction model as a REST API
- Incorporate carrier SLA and weather data for better ML accuracy
- Build Customer Lifetime Value models
- Add geospatial mapping with latitude/longitude data
- Develop demand forecasting for inventory planning

---

## Dataset Attribution

> Constante, F., Silva, F., & Pereira, A. (2019). *DataCo SMART SUPPLY CHAIN FOR BIG DATA ANALYSIS*. Mendeley Data, V5. DOI: [10.17632/8gx2fvg2k6.5](https://doi.org/10.17632/8gx2fvg2k6.5)
>
> License: Creative Commons Attribution 4.0 International (CC BY 4.0)

---

## GitHub Repository

After uploading:
- Repository: `https://github.com/YOUR_USERNAME/SmartSupply-Insights`
- Notebook: `https://github.com/YOUR_USERNAME/SmartSupply-Insights/blob/main/HimaniMane_SmartSupply_Insights.ipynb`

*(Replace `YOUR_USERNAME` with your actual GitHub username after upload)*

---

## Author

**Himani Mane**
AICTE | IBM SkillsBuild Data Analytics with AI — Academic Internship 2026
