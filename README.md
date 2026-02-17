# March Madness Predictive AI Model

An end-to-end Machine Learning pipeline designed to predict NCAA Tournament outcomes using historical performance data and ensemble learning techniques. This model achieved a **96th percentile finish** in national bracket challenges with an **84% individual matchup accuracy.**

## Performance Highlights
| Metric | Result |
| :--- | :--- |
| **Matchup Accuracy** | 84% |
| **National Percentile** | 96th |
| **Model Type** | Random Forest Classifier |
| **Validation Method** | 5-Fold Cross-Validation |

## The Tech Stack
* **Language:** Python
* **Data Science:** Pandas, NumPy, Scikit-Learn
* **Database:** PostgreSQL (Data centralization and querying)
* **Web Scraping:** BeautifulSoup4 (Acquiring 2023-2025 stats)

## Project Overview
The goal of this project was to move beyond "gut feeling" bracketology and build a system rooted in statistical probability. By combining historical data (2013–2022) with custom-scraped current season data, the model identifies the "DNA" of a winning team.

### Key Features:
* **Custom Data Pipeline:** Built a Python scraper to extract live stats from sports databases, bypassing the need for pre-formatted CSVs.
* **Feature Engineering:** Weighted key performance indicators (KPIs) like effective field goal percentage, strength of schedule, and defensive efficiency.
* **Ensemble Learning:** Utilized a **Random Forest** approach to reduce variance and prevent the overfitting common in single decision trees.
* **Robust Validation:** Implemented 5-fold cross-validation to ensure the model's predictive power held up across different "upset" scenarios and seasonal outliers.

## Methodology
1.  **Extraction:** Scraped and cleaned disparate data sources into a unified PostgreSQL schema.
2.  **Transformation:** Normalized statistics to account for varying conference strengths.
3.  **Training:** Trained the Random Forest model on 10 years of historical tournament results.
4.  **Prediction:** Ran 2024/2025 seasonal data through the model to generate the "Optimal Bracket."

---
*Note: Due to the seasonal nature of tournament hosting sites, live bracket visuals are currently unavailable during the off-season/reset period.*
