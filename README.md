# ⛽ Gas Price Correlation Analysis

Exploratory data analysis of U.S. gas prices and their correlations with key economic indicators including crude oil, inflation, and unemployment.

Built with Python, pandas, seaborn, and scipy.

---

## 📊 Key Findings

### Crude Oil (WTI) vs Gas Price
Crude oil is the strongest predictor of gas prices. Historically, the two move together with a correlation of **r ≈ 0.90+**, meaning roughly 80–85% of gas price variance can be explained by crude oil prices alone. Every $10 increase in crude oil typically corresponds to about a **$0.25–$0.30 increase per gallon** at the pump.

> 📝 *Your result:* R² = `___`, slope = `$___ per barrel`

### Inflation (CPI) vs Gas Price
Gas prices show a **moderate positive correlation with CPI** (r ≈ 0.6–0.75). This relationship is partly direct (energy is a CPI component) and partly indirect — rising energy costs push up prices across the economy. The rolling correlation chart shows this relationship strengthens during inflationary periods like 2008 and 2021–2022.

> 📝 *Your result:* r = `___`

### Unemployment vs Gas Price
Unemployment shows a **weak to moderate negative correlation** with gas prices (r ≈ -0.3 to -0.5). When unemployment is high, economic activity slows, demand for fuel drops, and prices tend to fall. This counter-cyclical relationship is clearest during recessions (2008–2009, 2020).

> 📝 *Your result:* r = `___`

### Seasonal Patterns
Gas prices follow a consistent seasonal cycle — rising through spring into **peak summer driving season (May–August)**, then falling through fall and winter. The summer/winter spread is typically **$0.20–$0.40/gallon**. This is driven by summer-blend fuel requirements and higher demand.

> 📝 *Your result:* highest month = `___`, lowest month = `___`

---

## 📁 Project Structure
```
gas-price-analysis/
├── gas_price_correlations.ipynb   # Main analysis notebook
├── requirements.txt               # Python dependencies
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started
```bash
git clone https://github.com/YOUR_USERNAME/gas-price-analysis.git
cd gas-price-analysis
pip install -r requirements.txt
jupyter notebook gas_price_correlations.ipynb
```

Or open instantly in Google Colab:
[Open in Colab](https://colab.research.google.com/) → File → Open notebook → GitHub → paste your repo URL

---

## 🗂 Data Sources

The notebook ships with **simulated data** so it runs out of the box. To use real data, swap in CSVs from:

| Source | What You Get |
|---|---|
| [EIA](https://www.eia.gov/petroleum/gasdiesel/) | Weekly U.S. retail gas prices by region |
| [FRED](https://fred.stlouisfed.org/) | CPI, unemployment rate, WTI crude oil |
| [Kaggle](https://www.kaggle.com/search?q=gas+prices) | Various cleaned gas price datasets |

---

## 🔧 Requirements

- Python 3.8+
- pandas, numpy, matplotlib, seaborn, scipy, jupyter

Install all at once:
```bash
pip install -r requirements.txt
```

---

## 🗺 Next Steps

- [ ] Replace simulated data with real EIA/FRED datasets
- [ ] Add state-level regional breakdown
- [ ] Analyze lag effects (crude oil → pump price delay is typically 2–6 weeks)
- [ ] Build a simple price prediction model (linear regression or ARIMA)

---

## License

MIT
