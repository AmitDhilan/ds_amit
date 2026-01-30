# ds_amit
# Data Science Assignment – Web3 Trading Team

## Project Overview
This project analyzes the relationship between trader behavior and Bitcoin market sentiment
(Fear, Greed, Neutral) using historical trader-level data from Hyperliquid and the Bitcoin
Fear & Greed Index.

The objective is to understand how trader profitability, trading volume, trade count,
and directional bias (Buy/Sell) vary across different market sentiment conditions.

---

## Directory Structure
ds_<candidate_name>/
├── notebook_1.ipynb
├── csv_files/
├── outputs/
├── ds_report.pdf
└── README.md

---

## Notebooks
- **notebook_1.ipynb**  
  - Complete data pipeline including:
    - Data loading
    - Data cleaning and preprocessing
    - Daily aggregation of trader activity
    - Merging trader data with market sentiment
    - Exploratory Data Analysis (EDA)
    - Insight generation and visualization

> All analysis was performed using **Google Colab**  
> Colab link is provided inside the notebook.

---

## Data Understanding & Cleaning
- Selected relevant columns such as:
  - Timestamp, Direction (Buy/Sell), Size USD, Closed PnL, Account
- Converted timestamps to date format
- Removed invalid, zero, or missing trade values
- Standardized trade direction labels

---

## Feature Engineering & Aggregation
Trader-level data was aggregated on a **daily basis** to compute:
- Total number of trades
- Total USD trading volume
- Average PnL
- Buy/Sell trade counts
- Buy/Sell ratio

This aggregated dataset was then merged with the **Bitcoin Market Sentiment**
(Fear / Greed / Neutral) dataset using the date column.

---

## Exploratory Data Analysis (EDA)
The following analyses were performed across market sentiment categories:
- Average PnL per sentiment
- Total trading volume per sentiment
- Total trade count per sentiment
- Buy/Sell ratio comparison

All visualizations are saved in the `outputs/` directory.

---

## Key Insights
- **Greed days** show higher average PnL, indicating increased profitability during bullish sentiment.
- **Fear days** exhibit the highest trading volume and trade count, suggesting aggressive and active participation even during cautious market conditions.
- **Neutral sentiment** shows consistent and stable trading behavior with high overall activity.
- Buy/Sell ratio is highest during **Fear**, implying traders tend to buy more aggressively during fearful market phases.
- Overall, market sentiment has a clear impact on trader profitability, volume, and directional bias.

---

## Outputs
- Aggregated and processed CSV files stored in `csv_files/`
- Visualizations stored in `outputs/`
- Final summarized insights documented in `ds_report.pdf`

---

## Notes
- Folder structure strictly follows the assignment guidelines
- All results are reproducible
- No private or restricted data was used
