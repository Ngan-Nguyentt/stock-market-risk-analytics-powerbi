# Stock Market Risk Analytics — Power BI

An interactive **Power BI** dashboard that reads five mega-cap US stocks the way an analyst would —
combining price action, technical momentum indicators, volume anomalies, a simulated sentiment overlay,
and a transparent scoring model that turns signals into explainable **Buy / Hold / Sell** calls.

> Course: Data Visualization · Algonquin College · Business Intelligence Systems Infrastructure

---

## 🎯 Objective
Give an everyday investor an analyst-grade, one-screen view of momentum and risk across
**AAPL, AMZN, GOOG, MSFT, and TSLA**, with a per-ticker slicer and three linked report pages.

## 🗂️ Data & modelling
- **`raw-stock-market-data.csv`** — raw historical price/volume data (~50,350 rows).
- **`cleaned-stock-market-data.csv`** — modelled output (~2,568 records) after **Power Query** cleaning.
- Built on a **star schema** with **DAX** measures for the indicators and the scoring model.

## 📊 What's inside (3 report pages)
- **Technical analysis** — **MACD** (momentum), **RSI** (overbought / oversold), **OHLC** range, and a
  **volume-spike detector** that flags volume above **2× its average**.
- **Scoring & signals** — a transparent **DAX scoring model** converts the indicators into explainable
  Buy / Hold / Sell calls (every call can be justified, not just asserted).
- **Sentiment** — an honest overlay: simulated daily sentiment did **not** reliably predict the next day's price.

### Highlights
- 📈 Tesla shows a **~500% volume spike** against an almost-flat monthly price — a divergence worth investigating.
- 🔍 Indicators are combined into one explainable score rather than a black-box recommendation.

## 🛠️ Tech stack
`Power BI` · `Power Query` · `DAX` · star-schema data modelling · financial / technical analytics

## 📁 Repository structure
```
stock-market-analysis.pbix              # Power BI report (open in Power BI Desktop)
stock-market-analytics-dashboard.pdf    # static export of the dashboard
raw-stock-market-data.csv               # raw source data
cleaned-stock-market-data.csv           # cleaned / modelled data
README.md
```

## ▶️ How to view
- Quick look: open **`stock-market-analytics-dashboard.pdf`**.
- Interactive: open **`stock-market-analysis.pbix`** in **Power BI Desktop** (free) and use the ticker slicer.

## 👥 Authors
Team project — **Ngan Nguyen** · **Duc Anh Ngo** · **DongHwan Won**
Business Intelligence Systems Infrastructure, Algonquin College

🔗 Portfolio: **https://ngan-nguyentt.github.io/**
