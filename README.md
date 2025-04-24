# AirBnB

# 🏡 Airbnb LA Insights: Forecasting Prices & Understanding Guest Satisfaction  
**DSO 574 Project – Spring 2025**  
**Tools:** Python | Pandas | NumPy | Statsmodels | Scikit-learn | Seaborn | Matplotlib | TextBlob

This project explores Airbnb listings in Los Angeles with the dual goal of forecasting average listing prices and identifying key factors that influence guest satisfaction. Leveraging a blend of time series modeling, regression analysis, and data visualization, we provide actionable insights for hosts and platforms alike.

---

## 🔍 Methodology

- Extracted **Month** and **Year** from the scrape date to support temporal trend analysis.
- Identified missing values in the `neighbourhood` column, where listings often had nulls in earlier months but valid values later.
- Removed rows with missing `neighbourhood` data (~17% of total) to maintain data quality.
- Grouped data by key attributes (`id`, `date`, `year`, `month`, `host_id`, `neighbourhood`, `latitude`, `longitude`, `room_type`) to compute:
  - Number of listings  
  - Average price  
  - Average minimum nights  
  - Average number of reviews  
  - Monthly review averages  
  - Annualized availability (out of 365 days)
- Enriched the dataset with a `Description` column from the detailed listing file. Removed rows containing **NaN**, **Inf**, or non-English descriptions.
- Applied **sentiment analysis** and measured **description length** as part of guest satisfaction modeling.

---

## 📌 Project Highlights

- Forecasted average prices across Los Angeles neighborhoods using **SARIMA**.
- Modeled guest satisfaction with **Multiple Linear Regression (MLR)**, employing **VIF** and **F-tests** for feature selection.
- Analyzed text sentiment from listing descriptions using **TextBlob**.
- Created clear, informative visualizations showcasing pricing trends, host profiles, and sentiment distributions.

---

## 📁 Deliverables

- `AirBnB Post Covid-Sentiment Analysis.pdf` – Final report  
- `AirBnB Pre & Post Covid Trend Findings.pdf` – Final report   

---

Feel free to explore the repository and reach out with any questions or feedback!
